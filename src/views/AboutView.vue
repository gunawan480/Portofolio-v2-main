<script>
export default {
  data() {
    return {
      activeTab: 1,
      tech: [
      {
          id: 1,
          name: 'HTML',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/1051/1051277.png',
          status: 'Intermediate'
        },
        {
          id: 2,
          name: 'CSS',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/732/732190.png',
          status: 'Intermediate'
        },
        {
          id: 3,
          name: 'PHP',
          imageUrl: 'https://cdn.iconscout.com/icon/free/png-256/free-php-2038871-1720084.png',
          status: 'Intermediate'
        },
        {
          id: 4,
          name: 'Javascript',
          imageUrl: 'https://cdn.icon-icons.com/icons2/2415/PNG/512/javascript_original_logo_icon_146455.png',
          status: 'Intermediate'
        },

        {
          id: 5,
          name: 'Codeigniter',
          imageUrl: 'https://img.icons8.com/?size=100&id=r4UrHt1gLC2t&format=png&color=000000',
          status: 'Intermediate'
        },
        {
          id: 6,
          name: 'NodeJS',
          imageUrl: 'https://cdn.iconscout.com/icon/free/png-256/free-node-js-1174925.png',
          status: 'Beginner'
        },
        {
          id: 7,
          name: 'Bootstrap',
          imageUrl: 'https://getbootstrap.com/docs/5.2/assets/brand/bootstrap-logo-shadow.png',
          status: 'Intermediate'
        },
        {
          id: 8,
          name: 'ReactJS',
          imageUrl: 'https://cdn4.iconfinder.com/data/icons/logos-3/600/React.js_logo-512.png',
          status: 'Intermediate'
        },
        {
          id: 9,
          name: 'C#',
          imageUrl: 'https://img.icons8.com/?size=100&id=11933&format=png&color=000000',
          status: 'Intermediate'
        },
        {
          id: 10,
          name: 'C++',
          imageUrl: 'https://img.icons8.com/?size=100&id=40669&format=png&color=000000',
          status: 'Beginner'
        },
        {
          id: 11,
          name: 'Java',
          imageUrl: 'https://img.icons8.com/?size=100&id=13679&format=png&color=000000',
          status: 'Beginner'
        },
        {
          id: 12,
          name: 'Python',
          imageUrl: 'https://img.icons8.com/?size=100&id=13441&format=png&color=000000',
          status: 'Beginner'
        }
      ],
      tools: [
        {
          id: 1,
          name: 'GitHub',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/25/25231.png',
          status: 'Git Hosting'
        },
        {
          id: 2,
          name: 'MySQL',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/5968/5968313.png',
          status: 'Database'
        },
        {
          id: 3,
          name: 'Unity',
          imageUrl: 'https://img.icons8.com/?size=100&id=39848&format=png&color=000000',
          status: 'Game Engine'
        },
        {
          id: 4,
          name: 'Android Studio',
          imageUrl: 'https://img.icons8.com/?size=100&id=EgOU93v1DHjU&format=png&color=000000',
          status: 'Debugging'
        },
        {
          id: 5,
          name: 'CorelDRAW',
          imageUrl: 'https://img.icons8.com/?size=100&id=tGW1lN11LBlx&format=png&color=000000',
          status: 'Desain Grafis Vektor'
        },
        {
          id: 6,
          name: 'Adobe Photoshop',
          imageUrl: 'https://img.icons8.com/?size=100&id=13677&format=png&color=000000',
          status: 'Desain Grafis'
        },
        {
          id: 7,
          name: 'Canva',
          imageUrl: 'https://img.icons8.com/?size=100&id=iWw83PVcBpLw&format=png&color=000000',
          status: 'Desain Grafis'
        },
        {
          id: 8,
          name: 'Figma',
          imageUrl: 'https://img.icons8.com/?size=100&id=snB4bDeuO6gJ&format=png&color=000000',
          status: 'Desain UI/UX'
        },
        {
          id: 9,
          name: 'Blender',
          imageUrl: 'https://img.icons8.com/?size=100&id=KDGdN57NLSJa&format=png&color=000000',
          status: 'Desain Animasi, rendering'
        },
        {
          id: 10,
          name: '3ds Max',
          imageUrl: 'https://img.icons8.com/?size=100&id=RCn6GKjgxJL0&format=png&color=000000',
          status: 'Pemodelan Animasi 3D'
        },
        {
          id: 11,
          name: 'SketchUp',
          imageUrl: 'https://img.icons8.com/?size=100&id=kDvZSDryG0yf&format=png&color=000000',
          status: ' Desain Arsitektur '
        },
        {
          id: 12,
          name: 'Microsoft Office',
          imageUrl: 'https://img.icons8.com/?size=100&id=6kZdxe7t8OL1&format=png&color=000000',
          status: ' produktivitas  '
        },
      ]
    };
  }
}
</script>
<template>
  <div
    class="bg-[#1e1e1f] px-5 py-5 md:px-12 md:py-10 text-left border border-[#383838] rounded-3xl text-amber-50 mx-3 mb-5">
    <article data-page="about">

      <header>
        <div class="text-2xl font-bold text-white mb-5 fadein-bot title-section flex items-center">
          Tentang Saya &nbsp;
          <div class="h-[1px] w-32 bg-primary-blue md:w-96 aos-init aos-animate" data-aos="zoom-in-left" data-aos-duration="600"></div>
        </div>
      </header>

      <section
        class="text-sm md:text-lg text-justify flex flex-col gap-4 md:flex-row md:gap-8 md:justify-left md:items-center">
      <div class="h-[500px] overflow-y-auto space-y-4 fadein-right">
        <!-- Frame 1 -->
        <div class="w-[450px] h-[300px] border-4 border-primary-blue overflow-hidden mx-auto">
          <img
            :src="require('@/assets/about me.jpg')"
            alt="Foto 1"
            class="w-full h-full object-cover"
          />
        </div>

        <!-- Frame 2 -->
        <div class="w-[450px] h-[300px] border-4 border-primary-blue overflow-hidden mx-auto">
          <img
            :src="require('@/assets/about me2.jpg')"
            alt="Foto 2"
            class="w-full h-full object-cover"
          />
        </div>

        <!-- Frame 3 -->
        <div class="w-[450px] h-[300px] border-4 border-primary-blue overflow-hidden mx-auto">
          <img
            :src="require('@/assets/about me3.jpg')"
            alt="Foto 3"
            class="w-full h-full object-cover"
          />
        </div>
      </div>
        <div class="md:w-7/12 ml-10">
          <p class="mb-3 md:mb-7 fadein-left fadeins-1">
            &nbsp; &nbsp; &nbsp; Hai! Nama saya Ahmad Syah Gunawan, seorang AR Engineer asal Brebes, Jawa Tengah.
            Saya lulusan S1 Teknik Informatika dari Universitas Muhammadiyah Purwokerto dengan IPK 3,65 dan memiliki
            pengalaman 1 tahun dalam pengembangan aplikasi Augmented Reality berbasis mobile. 
            Saya memiliki minat besar dalam menciptakan karya yang inovatif, kreatif, dan fungsional, 
            serta terus mengikuti perkembangan teknologi terbaru untuk meningkatkan kemampuan saya.
          </p>
            <p class="mb-3 md:mb-7 fadein-left fadeins-2">
            &nbsp; &nbsp; &nbsp; Saya memiliki keahlian dalam pengembangan aplikasi web dan mobile, serta tertarik pada animasi dan inovasi digital. Selain itu,
            saya aktif dalam kegiatan organisasi, pernah menjadi pengurus IPM saat SMA dan mentor AIK saat kuliah. 
            Saya juga menyukai olahraga, khususnya bola voli, dan telah meraih juara di tingkat fakultas (2021) dan prodi (2024),
             yang mengasah kemampuan kerja tim dan semangat kompetitif saya.
          </p>
          <p class="mb-3 fadein-left fadeins-3">
            &nbsp; &nbsp; &nbsp; Sebagai AR Engineer, saya berfokus pada pembuatan aplikasi yang tidak hanya fungsional dan mudah digunakan,
            tetapi juga menarik secara visual dan interaktif. Saya berkomitmen untuk selalu memberikan solusi terbaik dalam setiap proyek yang saya tangani,
            serta siap menjadi bagian dari tim yang dinamis dan inovatif.
          </p>

        </div>

      </section>

    </article>
  </div>

  <div class="px-5 py-5 md:px-12 md:py-10 text-left text-amber-50 mx-3">
    <article data-page="about">
      <header>
        <div class="text-2xl font-bold text-white mb-5 fadein-bot title-section flex items-center">
          <div class="h-[1px] w-10 bg-blue-500 shadow-[0_0_10px_#3B82F6] md:w-20 aos-init aos-animate" 
          data-aos="zoom-in-left" data-aos-duration="600"></div>
          &nbsp; Skills
        </div>
      </header>
      <section>
        <div>
           <ul class="flex flex-wrap text-sm font-medium text-center text-gray-500 dark:text-gray-400 mb-5">
            <li class="mr-2">
              <button class="inline-block px-4 py-3 rounded-lg hover:text-white" 
              :class="{ 'text-blue-500 bg-blue-500 bg-opacity-10': activeTab === 1 }" @click="activeTab = 1">Tech Stack
            </button>
          </li>
          <li class="mr-2">
            <button class="inline-block px-4 py-3 rounded-lg hover:text-white"
            :class="{ 'text-blue-500 bg-blue-500 bg-opacity-10': activeTab === 2 }" @click="activeTab = 2">Tools
          </button>
        </li>
      </ul>
    </div>
<div v-show="activeTab === 1">
  <div class="grid grid-cols-2 gap-4 pb-32 md:grid-cols-3 md:gap-8 xl:grid-cols-4 xl:gap-10 2xl:gap-12">
    <div v-for="item in tech" :key="item.id">
      <div
        class="item-tech flex cursor-pointer items-center gap-2 rounded border border-blue-300 px-2 py-2 hover:bg-blue-300 hover:bg-opacity-10 md:gap-3 lg:px-3">
        <div class="flex h-12 w-12 items-center justify-center p-0 lg:h-16 lg:w-16 lg:p-2 zoom-in">
          <img alt="HTML" loading="lazy" width="32" height="32" decoding="async" data-nimg="1"
            class="img-tech drop-shadow-xl transition-all duration-300 h-[65%] w-[65%] lg:h-[85%] lg:w-[85%]"
            :src="item.imageUrl" style="color: transparent;">
        </div>
        <div class="flex items-center text-sm md:text-base lg:text-lg">
          <div class="tech font-medium text-secondary transition-all duration-300 translate-y-0">
            {{ item.name }}
          </div>
          <div
            class="status-tech opacity-0 absolute mt-5 text-[10px] text-blue-300 transition-all duration-300 md:text-xs lg:text-sm">
            {{ item.status }}
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
        
<div v-show="activeTab === 2">
  <div class="grid grid-cols-2 gap-4 pb-32 md:grid-cols-3 md:gap-8 xl:grid-cols-4 xl:gap-10 2xl:gap-12">
    <div v-for="item in tools" :key="item.id">
      <div
        class="item-tech flex cursor-pointer items-center gap-2 rounded border border-blue-300 px-2 py-2 hover:bg-blue-300 hover:bg-opacity-10 md:gap-3 lg:px-3">
        <div class="flex h-12 w-12 items-center justify-center p-0 lg:h-16 lg:w-16 lg:p-2 zoom-in">
          <img alt="HTML" loading="lazy" width="32" height="32" decoding="async" data-nimg="1"
            class="img-tech drop-shadow-xl transition-all duration-300 h-[65%] w-[65%] lg:h-[85%] lg:w-[85%]"
            :src="item.imageUrl" style="color: transparent;">
        </div>
        <div class="flex items-center text-sm md:text-base lg:text-lg">
          <div class="tech font-medium text-secondary transition-all duration-300 translate-y-0">
            {{ item.name }}
          </div>
          <div
            class="status-tech opacity-0 absolute mt-5 text-[10px] text-blue-300 transition-all duration-300 md:text-xs lg:text-sm">
            {{ item.status }}
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

      </section>
    </article>
  </div>
</template>

<style>
.fadein-left {
  opacity: 0;
  animation: fadeInLeft 0.5s ease-out forwards;
}

@keyframes fadeInLeft {
  0% {
    opacity: 0;
    transform: translateX(100%);
  }

  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

.fadeins-1 {
  animation-delay: 500ms;
}

.fadeins-2 {
  animation-delay: 800ms;
}

.img-tech,
.tech {
  transition: transform 0.3s ease;
}

.item-tech:hover .img-tech {
  transform: scale(1.3);
}

.item-tech:hover .tech {
  transform: translateY(-12px);
}

.item-tech:hover .status-tech {
  opacity: 1;
}
</style>
