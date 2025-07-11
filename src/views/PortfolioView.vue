<script>
export default {
  data() {
    return {
      activeTab: 1,
      activeExperience: null,

      items: [
        {
          id: 1,
          name: 'AMTI AR',
          imageUrl: 'portfolio_ar',
          status: 'Saya merancang sebuah aplikasi pembelajaran siswa berbasis Android. Selain itu, saya juga memantau kinerja aplikasi dan memperbaiki berbagai kesalahan (error) yang ditemukan selama penggunaan. Hasilnya, saya berhasil menciptakan aplikasi Augmented Reality (AR) berbasis Android yang dapat membantu guru dalam proses pembelajaran siswa.',
          tech: 'C#, Unity, Blender, Vuforia, Canva, Figma',
          github: 'https://github.com/gunawan480/aplikasi-AR-alat-musik-tradisional-SDN-MENDALA-02',
          demo: 'https://ahmadsyahgunawan/'
        },
        {
          id: 2,
          name: 'ARNK',
          imageUrl: 'portfolio_ar2',
          status: 'Proyek ini merupakan hasil kolaborasi dengan staf pengajar di Fakultas Keguruan. Aplikasi ini dirancang untuk memudahkan siswa dalam mengenal cerita rakyat tentang Nyi Roro Kidul.',
          tech: 'C#, Unity, Blender, Vuforia, Canva, Figma',
          github: 'null',
          demo: 'null'
        },
        {
          id: 3,
          name: 'ARPS',
          imageUrl: 'portfolio_ar3',
          status: 'Proyek ini dibuat untuk memudahkan siswa memahami materi psikologi sastra.',
          tech: 'C#, Unity, Blender, Vuforia, Canva, Figma',
          github: 'null',
          demo: 'null'
        },
        {
          id: 4,
          name: 'Web Balai P3KB KEC.Sirampog KAB.Brebes',
          imageUrl: 'portfolio_web1',
          status: 'Proyek ini merupakan bagian dari kerja praktik di Balai Pemberdayaan Perempuan, Perlindungan Anak, Pengendalian Penduduk, dan Keluarga Berencana.',
          tech: 'Figma, PHP, HTML, JavaScript',
          github: 'null',
          demo: 'null'
        }
      ],

      certificates: [
        {
          id: 1,
          name: 'Beckend Development',
          provider: 'MySkill',
          date: 'September 2023',
          link: 'https://example.com/cert1',
          imageUrl: '/img/sertifikat-sertifikat_beckend.png'
        },
        {
          id: 2,
          name: 'UX Writing Fundamental',
          provider: 'MySkill',
          date: 'Oktober 2023',
          link: 'https://example.com/cert2',
          imageUrl: '/img/sertifikat-sertifikat_uxwritingfundamental.png'
        },
        {
          id: 3,
          name: 'Designing Using Canva',
          provider: 'MySkill',
          date: 'Oktober 2023',
          link: 'https://example.com/cert2',
          imageUrl: '/img/sertifikat-sertifikat_designingusingcanva.png'
        },
        {
          id: 4,
          name: 'Mini Bootcamp Super Admin',
          provider: 'YEC (Yureka Edukasi Cipta)',
          date: 'Februari 2025',
          link: 'https://example.com/cert2',
          imageUrl: '/img/sertifikat-sertifikat_superadmin.png'
        }
      ],

      awards: [
        {
          id: 1,
          title: 'Mentor Program Pendampingan Agama Islam (Mentoring)',
          organizer: 'LPPI Universitas Muhammadiyah Purwokerto',
          year: '2022',
          imageUrl: '/img/sertifikat-penghargaan-mentor.png',
          link: 'https://link-ke-detail-award1.com'
        },
        {
          id: 2,
          title: 'Common European Framework of Reference (CEFR)',
          organizer: 'Universitas Muhammadiyah Purwokerto',
          year: '2022',
          imageUrl: '/img/sertifikat-penghargaan-CEFR.png',
          link: 'https://link-ke-detail-award2.com'
        },
        {
          id: 3,
          title: 'Juara 2 Bola Voli Liga UMP',
          organizer: 'BKA Universitas Muhammadiyah Purwokerto',
          year: '2021',
          imageUrl: '/img/sertifikat-penghargaan-volijuara2.jpeg',
          link: 'https://link-ke-detail-award2.com'
        }
      ],

      jobs: [
        {
          id: 1,
          title: 'Web Development',
          company: 'Balai P3KB Kecamatan Sirampog Kabupaten Brebes',
          year: '2023',
          desc: 'Sebagai Web Developer di Balai P3KB Sirampog, saya bertanggung jawab dalam pengembangan, pembaruan konten, penambahan fitur, dan peningkatan performa situs web resmi. Saya juga terlibat dalam strategi digital untuk meningkatkan visibilitas lembaga.'
        },
      ],

      organizations: [
        {
          id: 1,
          role: 'Mentor dalam Program AIK (Al-Islam dan Kemuhammadiyahan)',
          org: 'AIK (Al-Islam dan Kemuhammadiyahan)',
          year: '2021-2022',
          desc: 'Membimbing peserta AIK dalam memahami dan menerapkan nilai-nilai Islam dan Kemuhammadiyahan melalui pembinaan, kegiatan edukatif, dan evaluasi rutin.'
        },
        {
          id: 2,
          role: 'Atlet Divisi Voli',
          org: 'UKM (Unit Kegiatan Mahasiswa)',
          year: '2020-2021',
          desc: 'Mewakili tim dalam kejuaraan voli, mengikuti latihan rutin, dan berkontribusi dalam strategi serta kekompakan tim untuk mencapai prestasi optimal.'
        },
        {
          id: 3,
          role: 'Divisi Umum',
          org: 'HMTI Anggota Muda',
          year: '2020-2021',
          desc: 'Mendukung operasional HMTI, mengoordinasikan kegiatan, serta membangun relasi internal dan eksternal untuk pengembangan organisasi dan anggota.'
        },
        {
          id: 4,
          role: 'ASBO (Anggota Bidang Apresiasi Seni Budaya dan Olahraga)',
          org: 'IPM (Ikatan Pelajar Muhammadiyah)',
          year: '2018-2020',
          desc: 'Mengorganisir kegiatan seni, budaya, dan olahraga serta mendorong apresiasi dan pengembangan bakat masyarakat, khususnya generasi muda.'
        }
      ]
    };
  },

  computed: {
    sertifikatChunk() {
      const chunkSize = 2;
      const result = [];
      for (let i = 0; i < this.certificates.length; i += chunkSize) {
        result.push(this.certificates.slice(i, i + chunkSize));
      }
      return result;
    }
  },

  methods: {
    setActiveExperience(type) {
      this.activeExperience = this.activeExperience === type ? null : type;
    }
  }
};
</script>


<template>
<section
  id="pengalaman"
  class="relative z-10 py-16 px-6 text-white bg-gradient-to-br from-[#1f1f1f]/80 via-[#111]/90 to-[#1f1f1f]/80 rounded-[2rem] shadow-xl shadow-black/30 backdrop-blur-md overflow-hidden mx-4 md:mx-16 lg:mx-24"
>

  <div
  class="max-w-5xl mx-auto space-y-12 rounded-[32px] backdrop-blur-md bg-white/5 ring-1 ring-white/10 p-6 shadow-lg shadow-black/20 overflow-hidden">
    
    <!-- PEKERJAAN -->
    <div>
      <div class="flex justify-between items-center border-b border-white/10 pb-2 mb-4">
        <h3 class="text-xl font-semibold">PEKERJAAN</h3>
        <button @click="setActiveExperience('jobs')"
                class="text-sm border border-gray-400 px-4 py-1 rounded-full hover:bg-blue-600 hover:text-white transition">
          LIHAT
        </button>
      </div>

      <transition name="fade">
        <div v-if="activeExperience === 'jobs'" class="space-y-4">
          <div v-for="job in jobs" :key="job.id"
               class="bg-white/10 rounded-2xl p-5 hover:bg-white/20 transition-all">
            <h4 class="text-lg font-semibold text-white">{{ job.title }}</h4>
            <p class="text-sm text-blue-300">{{ job.company }} - {{ job.year }}</p>
            <p class="text-sm text-gray-300 mt-2">{{ job.desc }}</p>
          </div>
        </div>
      </transition>
    </div>

    <!-- ORGANISASI -->
    <div>
      <div class="flex justify-between items-center border-b border-white/10 pb-2 mb-4 mt-10">
        <h3 class="text-xl font-semibold">ORGANISASI</h3>
        <button @click="setActiveExperience('organizations')"
                class="text-sm border border-gray-400 px-4 py-1 rounded-full hover:bg-blue-600 hover:text-white transition">
          LIHAT
        </button>
      </div>

      <transition name="fade">
        <div v-if="activeExperience === 'organizations'" class="space-y-4">
          <div v-for="org in organizations" :key="org.id"
               class="bg-white/10 rounded-2xl p-5 hover:bg-white/20 transition-all">
            <h4 class="text-lg font-semibold text-white">{{ org.role }}</h4>
            <p class="text-sm text-blue-300">{{ org.org }} - {{ org.year }}</p>
            <p class="text-sm text-gray-300 mt-2">{{ org.desc }}</p>
          </div>
        </div>
      </transition>
    </div>
  </div>
</section>

      <!-- Bagian Sertifikat -->
<section class="mt-16">
  <div class="text-2xl font-bold text-white mb-10 title-section flex flex-col items-center justify-center w-full">
    <h4>Sertifikat</h4>
    <div class="h-[1px] w-16 bg-primary-blue md:w-32" data-aos="zoom-in-left" data-aos-duration="600"></div>
    <div class="h-[1px] w-10 bg-blue-300 md:w-0"></div>
    <h4 class="text-center w-full text-base font-normal text-transparent bg-clip-text bg-gradient-to-r from-slate-100 to-blue-400">
      Koleksi sertifikat yang telah saya capai
    </h4>
  </div>

<!-- Sertifikat Scrollable -->
<div class="flex overflow-x-auto gap-4 px-4 py-4 scrollbar-thin scrollbar-thumb-black-600 scrollbar-track-gray-800">
  <div v-for="cert in certificates" :key="cert.id"
       class="min-w-[280px] max-w-[300px] bg-[#2b2b2b] rounded-xl p-4 text-white border border-[#444] flex-shrink-0 flex flex-col">
    
    <!-- Gambar proporsional -->
    <img :src="cert.imageUrl"
         alt="certificate"
         class="w-full h-44 object-contain rounded mb-3 bg-white" />

    <!-- Info -->
    <h3 class="font-semibold text-base leading-tight">{{ cert.name }}</h3>
    <p class="text-xs text-gray-400 mb-1">{{ cert.provider }} - {{ cert.date }}</p>
    <a :href="cert.link"
       target="_blank"
       class="text-blue-400 text-xs underline mt-auto">Lihat Sertifikat</a>
  </div>
  </div>
</section>
<!-- Bagian Penghargaan -->
<section class="mt-16">
  <div class="text-2xl font-bold text-white mb-10 title-section flex flex-col items-center justify-center w-full">
    <h4>Penghargaan</h4>
    <div class="h-[1px] w-16 bg-primary-blue md:w-32" data-aos="zoom-in-left" data-aos-duration="600"></div>
    <div class="h-[1px] w-10 bg-blue-300 md:w-0"></div>
    <h4 class="text-center w-full text-base font-normal text-transparent bg-clip-text bg-gradient-to-r from-slate-100 to-blue-400">
      Penghargaan yang pernah saya raih
    </h4>
  </div>

  <!-- Penghargaan Scrollable -->
  <div class="flex overflow-x-auto gap-4 px-4 py-4 scrollbar-thin scrollbar-thumb-black scrollbar-track-[#1a1a1a]">
    <div v-for="award in awards" :key="award.id"
         class="min-w-[280px] max-w-[300px] bg-[#2b2b2b] rounded-xl p-4 text-white border border-[#444] flex-shrink-0 flex flex-col">
      
      <!-- Gambar proporsional -->
      <img :src="award.imageUrl"
           alt="award"
           class="w-full h-44 object-contain rounded mb-3 bg-white" />

      <!-- Info -->
      <h3 class="font-semibold text-base leading-tight">{{ award.title }}</h3>
      <p class="text-xs text-gray-400 mb-1">{{ award.organizer }} - {{ award.year }}</p>
      <a :href="award.link"
         target="_blank"
         class="text-blue-400 text-xs underline mt-auto">Lihat Detail</a>
    </div>
  </div>
</section>
  <div class="px-5 py-5 md:px-12 md:py-10 text-left text-amber-50 mx-3">
    <article data-page="about">
      <header>
        <div class="text-2xl font-bold text-white mb-10 fadein-bot title-section flex items-center justify-center flex-col">
           <h4>Pengalaman Proyek</h4>
           <div class="h-[1px] w-16 bg-primary-blue md:w-32" data-aos="zoom-in-left" data-aos-duration="600"></div>
           <div class="h-[1px] w-10 bg-blue-300 md:w-0 aos-init aos-animate"></div>
            <h4 class="text-center text-base font-normal text-transparent bg-clip-text bg-gradient-to-r from-slate-100 to-blue-400">
              Jelajahi proyek yang telah saya kerjakan sejauh ini
            </h4>
        </div>
      </header>
      <section>
<div>
  <div class="grid grid-cols-1 gap-6 pb-6 md:pb-10 md:grid-cols-2 xl:grid-cols-2 fade-zoom-in">
    <div v-for="item in items" :key="item.id">
      <div
        class="item-card flex flex-col items-center gap-2 rounded bg-[#1e1e1f] hover:bg-[#282828] border border-[#383838] rounded-xl text-blue-50 md:gap-3 px-5 py-5 lg:px-5">
        <div class="flex h-12 w-12 items-center justify-center p-0 h-full w-full lg:p-0 zoom-in">
          <img alt="HTML" loading="lazy" decoding="async" data-nimg="1" class="drop-shadow-xl rounded rounded-xl"
            :src="'/img/portfolio-' + item.imageUrl + '.png'">
        </div>
        <div class="w-full flex flex-col gap-2 items-center text-sm md:text-base lg:text-lg">
          <div class="title-text font-medium text-secondary">{{ item.name }}</div>
          <div class="w-full text-left text-[10px] text-[#c1c1c1] md:text-xs lg:text-sm">
            {{ item.status }}
          </div>
          <div class="w-full mt-4 text-normal text-sm text-left text-blue-300">
            {{ item.tech }}
          </div>
          <div class="w-full flex justify-end">
            <div class="flex cursor-pointer items-end gap-2 text-primary">
              <a v-if="item.github !== 'null'"
                :href="item.github" target="_blank" rel="noreferrer"
                title="View github repository" class="transition-all hover:text-accent">
                <svg stroke="currentColor"
                  fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round"
                  height="16" width="16" xmlns="http://www.w3.org/2000/svg">
                  <path
                    d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22">
                  </path>
                </svg>
              </a>
              <a v-if="item.demo !== 'null'" :href="item.demo" target="_blank" rel="noreferrer"
                title="View finished project" class="transition-all hover:text-accent">
                <svg stroke="currentColor"
                  fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round"
                  height="18" width="18" xmlns="http://www.w3.org/2000/svg">
                  <path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"></path>
                  <polyline points="15 3 21 3 21 9"></polyline>
                  <line x1="10" y1="14" x2="21" y2="3"></line>
                </svg>
              </a>
            </div>
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
.experience-box {
  background-color: #262626; /* lebih terang dari latar */
  border: 1px solid #444;
  border-radius: 12px;
  padding: 1rem;
  transition: all 0.3s ease;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}

.experience-box:hover {
  transform: translateY(-3px);
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3);
}

.experience-title {
  font-weight: 600;
  font-size: 1rem;
}

.experience-sub {
  font-size: 0.85rem;
  color: #9ca3af; /* abu-abu terang */
}

.experience-desc {
  margin-top: 0.3rem;
  font-size: 0.9rem;
  color: #e5e7eb;
}

.scrollbar-thin::-webkit-scrollbar {
  width: 8px;
  height: 8px; /* untuk horizontal scrollbar jika ada */
}

.scrollbar-thumb-gray-600::-webkit-scrollbar-thumb {
  background-color: #3B82F6; /* Biru */
  border-radius: 10px;
  border: 2px solid #1f2937; /* Sesuaikan dengan warna track */
}

.scrollbar-track-gray-800::-webkit-scrollbar-track {
  background-color: #1f2937; /* Hitam abu-abu gelap */
}

.item-card:hover {
  transition: transform 0.3s ease;
  transform: translateY(-8px);
}
svg:hover{
  stroke: #3B82F6;
}
@keyframes fadeZoomIn {
  0% {
    opacity: 0;
    transform: scale(0.5);
  }
  100% {
    opacity: 1;
    transform: scale(1);
  }
}

/* Menggunakan animasi pada elemen yang diinginkan */
.fade-zoom-in {
  animation: fadeZoomIn 1s ease-in-out;
}
#pengalaman {
  background-color: #1e1e1f; /* Sesuaikan dengan box lainnya */
  color: white;
  padding: 2.5rem 1rem;
}


#pengalaman h2 {
  text-align: center;
  font-size: 2rem;
  color: #818cf8; /* Ungu/Biru sesuai gambar */
  margin-bottom: 2rem;
}

#pengalaman .entry {
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-bottom: 1px dotted gray;
  padding-bottom: 0.5rem;
  margin-bottom: 1rem;
}

#pengalaman .entry h3 {
  font-size: 1.2rem;
  font-weight: bold;
}

#pengalaman .entry button {
  padding: 0.25rem 1rem;
  border: 1px solid gray;
  border-radius: 5px;
  background: transparent;
  cursor: pointer;
  transition: all 0.3s;
}

#pengalaman .entry button:hover {
  background-color: #6366f1; /* Biru hover */
  color: white;
}

</style>