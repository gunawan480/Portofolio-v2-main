<template>
<div class="container mx-auto p-3 md:p-8">
  <div class="flex flex-col md:flex-row relative">
      <div class="w-full md:w-1/3 h-fit p-4 md:p-8 md:sticky md:top-24">
        <div class="flex flex-col gap-4 md:px-20 fade-zoom-up">
          <article v-for="article in articles" :key="article.id">
            <router-link
              :to="`/read/${article.slug}/${article.id}`"
              class="flex w-full bg-[#1e1e1f] border-[#383838] rounded-xl text-left text-white p-5 md:py-7 md:px-8 cursor-pointer hover:bg-[#282828] items-center"
            >
              <div class="w-full pr-4">
                <!-- ✅ Tanggal tetap abu-abu -->
                <div class="text-xs mb-1 text-slate-400 flex items-center italic">
                  <div class="h-[1px] w-20 bg-blue-300 md:w-5 aos-init aos-animate mr-2"></div>
                  {{ article.date }}
                </div>

                <!-- ✅ Judul berwarna biru -->
                <h1 class="text-sm md:text-md text-blue-400 font-bold mb-2 paraf">
                  {{ article.title }}
                </h1>

                <!-- ✅ Deskripsi berwarna biru -->
                <div class="text-sm hidden md:block text-blue-200 paraf">
                  {{ article.desc }}
                </div>
              </div>

              <div>
                <div class="w-20 h-20 md:w-28 flex items-center md:h-28">
                  <img :src="article.image" class="rounded-lg md:rounded-xl" alt="" />
                </div>
              </div>
            </router-link>
          </article>
        </div>
      </div>

      <!-- Sidebar -->
      <div class="w-full md:w-1/3 h-fit p-8 md:sticky md:top-24">
        <div class="flex flex-col text-left">
          <div class="bg-clip-text bg-gradient-to-r from-blue-200 to-blue-500 text-transparent">
            Mari berbagi pengalaman, cerita, dan pengetahuan bersama.
          </div>
          <div class="h-[1px] mt-7 mb-7 w-20 bg-blue-300 aos-init aos-animate mr-2"></div>
          <div class="hidden md:block">
            <div class="text-blue-300 text-md font-semibold">Pembahasan</div>
            <div class="mt-3 flex flex-wrap gap-1">
              <span class="py-2 px-3 rounded-2xl bg-[#1e1e1f] hover:bg-white/20 text-blue-200 text-xs cursor-pointer">
                Sosial
              </span>
              <span class="py-2 px-3 rounded-2xl bg-[#1e1e1f] hover:bg-white/20 text-blue-200 text-xs cursor-pointer">
                Technology
              </span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <ArticleList />
</template>


  
<script>
import axios from 'axios';

export default {
  data() {
    return {
      articles: []
    }
  },
  mounted() {
    this.getArticles(); // ✅ Ambil semua data
  },
methods: {
  async getArticles() {
    try {
      const response = await axios.get('https://686b6266e559eba908724bef.mockapi.io/articles');
      console.log("Data dari API:", response.data); // 👈 DEBUG
      this.articles = response.data;
    } catch (error) {
      console.error("Gagal mengambil artikel:", error); // 👈 DEBUG
    }
  }
}
}
</script>
