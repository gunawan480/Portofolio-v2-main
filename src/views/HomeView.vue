<template>
  <main
    class="mt-10 md:mt-1 flex flex-col-reverse gap-8 items-center md:flex-row md:gap-16 md:justify-center min-h-[65vh] md:min-h-[80vh]">
    <div class="space-y-2 text-center md:text-left px-10">
      <p class="text-blue-500">Hello Everyone, I'm</p>
      <h1 class="text-4xl font-bold md:text-5xl text-white fadein-up">Ahmad Syah Gunawan</h1>
      <div class="py-2">
        <h1
          class="typewrite text-xl font-semibold text-transparent bg-clip-text bg-gradient-to-r from-slate-100 to-blue-500 md:text-2xl fadein-up"
          ref="typewriter">
          <span class="wrap">{{ txt }}</span>
        </h1>
      </div>
      <p class="text-white pr-4 fade-in-from-left">Welcome to My personal website. <span class="wave">👋🏼</span></p>
      <br>
      <!-- Ikon Sosial Media -->
       <div class="flex gap-4 mt-6 justify-center md:justify-start">
        <!-- Instagram -->
         <a href="https://instagram.com/gunsyh_" target="_blank" rel="noreferrer"
         class="text-blue-300 hover:text-blue-500 transition-colors duration-300">
         <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor" viewBox="0 0 24 24">
          <path d="M12 2.2c3.2 0 3.6 0 4.9.1 1.2.1 2 .3 2.5.5.6.2 1 .6 1.4 1.1.4.4.8.9 1.1 1.4.2.5.4 1.3.5 2.5.1 1.3.1 1.7.1 4.9s0 3.6-.1 4.9c-.1 1.2-.3 2-.5 2.5-.2.6-.6 1-1.1 1.4-.4.4-.9.8-1.4 1.1-.5.2-1.3.4-2.5.5-1.3.1-1.7.1-4.9.1s-3.6 0-4.9-.1c-1.2-.1-2-.3-2.5-.5-.6-.2-1-.6-1.4-1.1-.4-.4-.8-.9-1.1-1.4-.2-.5-.4-1.3-.5-2.5-.1-1.3-.1-1.7-.1-4.9s0-3.6.1-4.9c.1-1.2.3-2 .5-2.5.2-.6.6-1 1.1-1.4.4-.4.9-.8 1.4-1.1.5-.2 1.3-.4 2.5-.5 1.3-.1 1.7-.1 4.9-.1M12 0C8.7 0 8.3 0 7 .1c-1.4.1-2.4.3-3.3.7C2.8 1.3 2 2 1.4 2.7.7 3.5.3 4.5.1 5.9 0 7.2 0 7.7 0 12c0 4.3 0 4.8.1 6.1.1 1.4.3 2.4.7 3.3.6.8 1.4 1.4 2.1 2.1.9.4 1.9.6 3.3.7C8.3 24 8.7 24 12 24s3.7 0 5.1-.1c1.4-.1 2.4-.3 3.3-.7.8-.6 1.4-1.4 2.1-2.1.4-.9.6-1.9.7-3.3.1-1.3.1-1.8.1-6.1s0-4.8-.1-6.1c-.1-1.4-.3-2.4-.7-3.3-.6-.8-1.4-1.4-2.1-2.1C19.5.3 18.5.1 17.1 0 15.8 0 15.3 0 12 0z"/>
          <path d="M12 5.8c-3.4 0-6.2 2.8-6.2 6.2S8.6 18.2 12 18.2 18.2 15.4 18.2 12 15.4 5.8 12 5.8zm0 10.2c-2.2 0-4-1.8-4-4s1.8-4 4-4 4 1.8 4 4-1.8 4-4 4z"/>
          <circle cx="18.4" cy="5.6" r="1.4"/></svg>
        </a>
        <!-- TikTok -->
        <a href="https://www.tiktok.com/@j_freeeaaak" target="_blank" rel="noreferrer"
        class="text-blue-300 hover:text-blue-500 transition-colors duration-300">
        <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" width="24" height="24" viewBox="0 0 24 24">          <path d="M9.75 4.5v13.13a3.38 3.38 0 0 1-2.94-3.25A3.38 3.38 0 0 1 10.19 11V8.94a6.07 6.07 0 0 0-6 6.06 6 6 0 0 0 6 6h.19a6.1 6.1 0 0 0 6.06-6.06V9.75a8.81 8.81 0 0 0 3.75.75V6.94a5.6 5.6 0 0 1-3.75-1.5 5.63 5.63 0 0 1-1.5-3.75h-3a8.63 8.63 0 0 0 .75 3.75 5.66 5.66 0 0 0 2.25 2.25v7.5a3.38 3.38 0 0 1-3.38 3.38z" />
        </svg>
      </a>
      <!-- LinkedIn -->
      <a href="https://linkedin.com/in/ahmad-syah-gunawan" target="_blank" rel="noreferrer"
      class="text-blue-300 hover:text-blue-500 transition-colors duration-300">
      <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24"> 
        <path d="M4.98 3.5C4.98 4.88 3.87 6 2.49 6S0 4.88 0 3.5 1.11 1 2.49 1s2.49 1.12 2.49 2.5zM.48 8.99h3.99V24H.48zM7.4 8.99h3.83v2.05h.05c.53-1 1.82-2.05 3.76-2.05 4.02 0 4.76 2.64 4.76 6.07V24h-4v-7.9c0-1.88-.03-4.29-2.62-4.29-2.62 0-3.02 2.05-3.02 4.16V24h-4V8.99z"/>
      </svg>
    </a>
  </div>
      <!-- <button
        class="fadein-bot fade-500 flex items-center py-2 px-4 mx-auto text-sm font-medium rounded-lg border transition duration-300 md:py-2.5 md:px-5 md:mx-0 text-amber-200 border-amber-200 hover:bg-amber-200 hover:bg-opacity-10 bg-transparent focus:outline-none w-fit"><svg
          xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="mr-2 w-4 h-4">
          <path fill-rule="evenodd"
            d="M5.625 1.5H9a3.75 3.75 0 013.75 3.75v1.875c0 1.036.84 1.875 1.875 1.875H16.5a3.75 3.75 0 013.75 3.75v7.875c0 1.035-.84 1.875-1.875 1.875H5.625a1.875 1.875 0 01-1.875-1.875V3.375c0-1.036.84-1.875 1.875-1.875zm5.845 17.03a.75.75 0 001.06 0l3-3a.75.75 0 10-1.06-1.06l-1.72 1.72V12a.75.75 0 00-1.5 0v4.19l-1.72-1.72a.75.75 0 00-1.06 1.06l3 3z"
            clip-rule="evenodd"></path>
          <path
            d="M14.25 5.25a5.23 5.23 0 00-1.279-3.434 9.768 9.768 0 016.963 6.963A5.23 5.23 0 0016.5 7.5h-1.875a.375.375 0 01-.375-.375V5.25z">
          </path>
        </svg>Download Resume</button> -->
    </div>
    
    
    
    <div class="rounded-full border-4 border-blue-500 shadow-lg pict">
      <img
      :src="require('@/assets/animasi profil.jpg')"
      alt="avatar"
      fetchpriority="high"
      decoding="async"
      class="w-40 h-40 sm:w-52 sm:h-52 md:w-64 md:h-64 lg:w-80 lg:h-80 object-cover rounded-full"/>
    </div>
  </main>
</template>

<script>
export default {
  name: 'HomeView',
  data() {
    return {
      toRotate: ["Bachelor of Informatics Engineering","AR Engineer","Web Development", "Mobile Development"],
      period: 2000,
      txt: '',
      loopNum: 0,
      isDeleting: false,
    };
  },
  mounted() {
    this.$nextTick(() => {
      this.tick();
    });
  },
  methods: {
    tick() {
      let typewriter = this.$refs.typewriter;

      if (!typewriter) {
        return;
      }

      let i = this.loopNum % this.toRotate.length;
      let fullTxt = this.toRotate[i];

      this.txt = this.isDeleting ? fullTxt.substring(0, this.txt.length - 1) : fullTxt.substring(0, this.txt.length + 1);
      typewriter.innerHTML = `<span class="wrap">${this.txt}</span>`;

      let that = this;
      let delta = 200 - Math.random() * 100;

      if (this.isDeleting) {
        delta /= 2;
      }

      if (!this.isDeleting && this.txt === fullTxt) {
        delta = this.period;
        this.isDeleting = true;
      } else if (this.isDeleting && this.txt === '') {
        this.isDeleting = false;
        this.loopNum++;
        delta = 500;
      }

      setTimeout(() => {
        that.tick();
      }, delta);
    },
  }
}
</script>

<style>
body {
  overflow-y: scroll;
  overflow-x: hidden;
}

.typewrite>.wrap {
  border-right: 0.08em solid #fff;
}

.wave {
  animation-name: wave-animation;
  animation-duration: 2.5s;
  animation-iteration-count: infinite;
  transform-origin: 70% 70%;
  display: inline-block
}

@keyframes wave-animation {
  0% {
    transform: rotate(0deg)
  }

  10% {
    transform: rotate(14deg)
  }

  20% {
    transform: rotate(-8deg)
  }

  30% {
    transform: rotate(14deg)
  }

  40% {
    transform: rotate(-4deg)
  }

  50% {
    transform: rotate(10deg)
  }

  60% {
    transform: rotate(0deg)
  }

  to {
    transform: rotate(0deg)
  }
}

.pict {
  box-shadow: 0px 0px 73px -9px rgba(59, 130, 246, 0.44);
  -webkit-box-shadow: 0px 0px 73px -9px rgba(59, 130, 246, 0.44);
  -moz-box-shadow: 0px 0px 73px -9px rgba(59, 130, 246, 0.44);
}

.fadein-up {
  opacity: 0;
  animation-name: fadeInUp;
  animation-duration: 0.5s;
  animation-fill-mode: forwards;
  animation-delay: 500ms;
}

@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translate3d(0, 100%, 0);
  }

  to {
    opacity: 1;
    transform: translate3d(0, 0, 0);
  }
}

.fade-in-from-left {
  opacity: 0;
  animation: fadeInLeft 0.5s ease-out forwards;
  animation-delay: 500ms;
}

@keyframes fadeInLeft {
  0% {
    opacity: 0;
    transform: translateX(-100%);
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

.fadein-right {
  opacity: 0;
  animation: fadeInRight 0.5s ease-out forwards;
  animation-delay: 500ms;
}

@keyframes fadeInRight {
  0% {
    opacity: 0;
    transform: translateX(100%);
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

.fadein-bot {
  opacity: 0;
  animation: fadeInBot 0.5s forwards;
}

@keyframes fadeInBot {
  from {
    opacity: 0;
    transform: translate3d(0, -100%, 0);
  }

  to {
    opacity: 1;
    transform: translate3d(0, 0, 0);
  }
}

.fadein-1 {
  animation-delay: 200ms;
}
.fadein-2 {
  animation-delay: 400ms;
}
.fadein-3 {
  animation-delay: 600ms;
}
.fade-500 {
  animation-delay: 500ms;
}
</style>
