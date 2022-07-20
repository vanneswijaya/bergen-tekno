<template>
  <div class="overflow-hidden">
    <section class="bg-kuning w-screen h-screen flex">
      <div class="flex flex-nowrap fixed">
        <div class="w-screen flex flex-col justify-center pl-28 pb-40">
          <div
            ref="hey"
            class="font-thin text-kuning text-9xl absolute pl-90 z-50 flex flex-col"
          >
            <div>Bergen Tekno</div>
            <div class="text-5xl pt-10">We are IT. We are humans.</div>
            <div class="icon-scroll right-0"></div>
            <div class="scroll-down right-0 text-xl">SCROLL DOWN</div>
          </div>
          <div ref="letMe" class="waves"></div>
        </div>
        <div
          ref="intro"
          class="w-screen h-screen grid grid-cols-2 gap-x-5 py-20"
        >
          <div class="col-span-1 flex flex-col">
            <div class="font-black text-birutua text-9xl pt-16">
              Ready to help you!
            </div>
            <div class="font-light text-birutua text-5xl pt-10">
              We're <span class="font-extrabold">Bergen Tekno</span>,<br />
              We value human, organizational, and operational intelligence, not
              just artificial.
            </div>
          </div>
          <div class="col-span-1 pt-20">
            <div
              class="w-128 h-128 rounded-full bg-cover bg-center"
              :style="profpic"
            ></div>
          </div>
        </div>
      </div>
    </section>
    <section class="bg-kuning h-screen"></section>
    <section class="bg-kuning h-screen"></section>
    <section class="bg-kuning h-screen"></section>
    <section class="bg-kuning h-full w-screen pb-20 flex flex-col items-center">
      <div ref="works" class="font-black text-birutua text-9xl uppercase pt-20">
        Our Works &
      </div>
      <div ref="contrib" class="font-black text-birutua text-9xl uppercase">
        Contributions
      </div>
      <div
        class="bg-cover bg-center w-3/4 h-160 mt-20 rounded-3xl group"
        :style="dfdg"
      >
        <div
          class="group-hover:opacity-100 opacity-0 transition duration-500 ease-in-out relative flex flex-col items-center w-full h-full"
        >
          <div class="flex flex-col absolute z-50 items-center">
            <div class="font-black text-white text-8xl pt-20">DFDG</div>
            <div class="grid grid-cols-2 px-20 pt-20">
              <div class="font-thin text-4xl text-white">
                DFDG Architecture’s company website features a quality design
                that uses a large background photo on the homepage.
              </div>
              <div
                @click="goToFarma()"
                class="rotate bg-opacity-0 bg-white hover:bg-opacity-100 border-2 border-white rounded-full w-48 h-48 ml-40 mt-10 flex items-center text-white hover:text-black transition duration-500 ease-in-out cursor-pointer"
              >
                <div
                  class="font-black text-2xl pl-10 flex flex-col items-center"
                >
                  <div>VIEW</div>
                  <div>PROJECT</div>
                </div>
              </div>
            </div>
          </div>
          <div
            class="bg-black absolute opacity-50 w-full h-full inset-0 rounded-3xl"
          ></div>
          <div
            class="bg-gradient-to-b from-black via-transparent to-transparent absolute opacity-70 w-full h-full inset-0 rounded-3xl"
          ></div>
        </div>
      </div>
      <div
        class="bg-cover bg-center w-3/4 h-160 mt-20 rounded-3xl group"
        :style="prco"
      >
        <div
          class="group-hover:opacity-100 opacity-0 transition duration-500 ease-in-out relative flex flex-col items-center w-full h-full"
        >
          <div class="flex flex-col absolute z-50 items-center">
            <div class="font-black text-white text-8xl pt-20">PRCO</div>
            <div class="grid grid-cols-2 px-20 pt-20">
              <div class="font-thin text-4xl text-white">
                PRCO is a global PR agency and their homepage takes a bit of an
                unusual approach.
              </div>
              <div
                @click="goToArchio()"
                class="rotate bg-opacity-0 bg-white hover:bg-opacity-100 border-2 border-white rounded-full w-48 h-48 ml-40 mt-10 flex items-center text-white hover:text-black transition duration-500 ease-in-out cursor-pointer"
              >
                <div
                  class="font-black text-2xl pl-10 flex flex-col items-center"
                >
                  <div>VIEW</div>
                  <div>PROJECT</div>
                </div>
              </div>
            </div>
          </div>
          <div
            class="bg-black absolute opacity-70 w-full h-full inset-0 rounded-3xl"
          ></div>
        </div>
      </div>
      <div
        class="bg-cover bg-center w-3/4 h-160 mt-20 rounded-3xl group"
        :style="adam"
      >
        <div
          class="group-hover:opacity-100 opacity-0 transition duration-500 ease-in-out relative flex flex-col items-center w-full h-full"
        >
          <div class="flex flex-col absolute z-50 items-center">
            <div class="font-black text-white text-8xl pt-20">ADAM CHURCH</div>
            <div class="grid grid-cols-2 px-20 pt-20">
              <div class="font-thin text-4xl text-white">
                Adam Church offers property management services and their
                company website is an impressive example that could be used to
                inspire other businesses and designers.
              </div>
              <div
                @click="goToDuktiv()"
                class="rotate bg-opacity-0 bg-white hover:bg-opacity-100 border-2 border-white rounded-full w-48 h-48 ml-40 mt-10 flex items-center text-white hover:text-black transition duration-500 ease-in-out cursor-pointer"
              >
                <div
                  class="font-black text-2xl pl-10 flex flex-col items-center"
                >
                  <div>VIEW</div>
                  <div>PROJECT</div>
                </div>
              </div>
            </div>
          </div>
          <div
            class="bg-black absolute opacity-70 w-full h-full inset-0 rounded-3xl"
          ></div>
        </div>
      </div>
    </section>
    <div class="wrapper overflow-x-hidden overflow-y-hidden h-screen bg-fixed">
      <section
        class="parallax relative bg-cover bg-center h-full bg-fixed"
        :style="nypic"
      >
        <div class="absolute z-50 flex flex-col items-center w-full">
          <div class="font-black text-kuning text-9xl pt-20">Our Clients</div>
          <div
            ref="containerProg"
            class="progress mt-20 rounded-3xl transition-all duration-500 ease-in-out"
          >
            <div
              ref="progress"
              @click="langClick"
              class="progress-value flex items-center rounded-3xl cursor-pointer hover:bg-birutua group transition-all duration-500 ease-in-out"
            >
              <div
                :class="{ 'opacity-100': !langlong }"
                class="opacity-0 text-5xl font-black text-birutua pl-10 group-hover:text-kuning transition-all duration-500 ease-in-out"
              >
                IT Companies
              </div>
              <div
                :class="{ 'opacity-100': langlong }"
                class="opacity-0 text-5xl font-black text-birutua pl-20 group-hover:text-kuning transition-all duration-200 ease-in-out absolute grid grid-cols-3 gap-20"
              >
                <div class="flex flex-col gap-y-10">
                  <img
                    class="h-28 w-28"
                    src="https://cdn-icons-png.flaticon.com/512/732/732221.png"
                    alt=""
                  />
                  <img
                    class="h-28 w-28"
                    src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/99/Unofficial_JavaScript_logo_2.svg/2048px-Unofficial_JavaScript_logo_2.svg.png"
                    alt=""
                  />
                </div>
                <div class="flex flex-col gap-y-10">
                  <img
                    class="h-28 w-28"
                    src="https://www.redditinc.com/assets/images/site/reddit-logo.png"
                    alt=""
                  />
                  <img
                    class="h-28 w-28"
                    src="https://seeklogo.com/images/P/pinterest-logo-CA98998DCB-seeklogo.com.png"
                    alt=""
                  />
                </div>
                <div class="flex flex-col gap-y-10">
                  <img
                    class="max-h-28 max-w-28"
                    src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d5/Slack_icon_2019.svg/2048px-Slack_icon_2019.svg.png"
                    alt=""
                  />
                </div>
              </div>
            </div>
          </div>
          <div
            ref="containerProg2"
            class="progress mt-5 rounded-3xl transition-all duration-500 ease-in-out"
          >
            <div
              ref="progress2"
              @click="toolClick"
              class="progress-value flex items-center rounded-3xl hover:bg-birutua group transition-all duration-500 ease-in-out cursor-pointer"
            >
              <div
                :class="{ 'opacity-100': !toollong }"
                class="opacity-0 text-5xl font-black text-birutua pl-10 absolute z-50 group-hover:text-kuning transition duration-500 ease-in-out"
              >
                Open Source Projects
              </div>
              <div
                :class="{ 'opacity-100': toollong }"
                class="opacity-0 text-5xl font-black text-birutua pl-20 group-hover:text-kuning transition-all duration-200 ease-in-out grid grid-cols-3 gap-20"
              >
                <div class="flex flex-col gap-y-10">
                  <img
                    class="h-28 w-28"
                    src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/95/Vue.js_Logo_2.svg/2367px-Vue.js_Logo_2.svg.png"
                    alt=""
                  />
                  <img
                    class="h-28 w-28"
                    src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/17/GraphQL_Logo.svg/2048px-GraphQL_Logo.svg.png"
                    alt=""
                  />
                </div>
                <div class="flex flex-col gap-y-10">
                  <img
                    class="h-28 w-28"
                    src="https://static-00.iconduck.com/assets.00/strapi-icon-512x505-3hl7a1v3.png"
                    alt=""
                  />
                  <img
                    class="h-28 w-28"
                    src="https://cdn.worldvectorlogo.com/logos/tailwindcss.svg"
                    alt=""
                  />
                </div>
                <div class="flex flex-col gap-y-10">
                  <img
                    class="h-28 w-28"
                    src="https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png"
                    alt=""
                  />
                  <img
                    class="h-28 w-28"
                    src="https://img.icons8.com/color/480/mongodb.png"
                    alt=""
                  />
                </div>
              </div>
            </div>
          </div>
        </div>
        <div
          class="bg-birutua via-transparent to-transparent absolute opacity-70 w-full h-full inset-0"
        ></div>
      </section>
    </div>
    <section class="bg-birutua h-screen w-screen flex flex-col items-center">
      <div class="font-black text-kuning mt-20 text-9xl">HISTORY</div>
      <div class="grid grid-cols-2 justify-items-center py-20 gap-x-20">
        <div class="flex flex-col justify-center">
          <div class="h-32 w-32 mb-5">
            <img
              src="https://yt3.ggpht.com/-RZYi5isxH_M/AAAAAAAAAAI/AAAAAAAAAAA/rmWpoe2qZzI/s900-c-k-no/photo.jpg"
              alt=""
            />
          </div>
          <div class="font-thin text-kuning text-3xl">
            <div class="font-extrabold text-5xl">Founded in NYU</div>
            <div class="font-extrabold">2018 - 2021</div>
            <div class="pt-10">
              <ul>
                <li>- Founded by Bergen Schmidt</li>
                <li>- Received funding from NY TECH 300</li>
                <li>- Received Pedro Entrepreneurship Award</li>
              </ul>
            </div>
          </div>
        </div>
        <div class="flex flex-col justify-center">
          <div class="h-32 w-32 mb-5">
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b2/Y_Combinator_logo.svg/640px-Y_Combinator_logo.svg.png"
              alt=""
            />
          </div>
          <div class="font-thin text-kuning text-3xl">
            <div class="font-extrabold text-5xl">Y Combinator S21</div>
            <div class="font-extrabold">2021 - 2022</div>
            <div class="pt-10">
              <ul>
                <li>- Won an early seed funding round by Y Combinator</li>
                <li>- Accelerated to 40 employees in the company</li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="bg-kuning">
      <div class="flex flex-col px-20 pt-20 pb-28 text-birutua">
        <div class="text-9xl font-black">Get in touch.</div>
        <div class="w-3/4 h-4 mt-5 bg-birutua"></div>
        <div class="pt-20 font-extrabold flex flex-col">
          <div class="text-3xl">Email :</div>
          <div class="text-5xl z-50 cursor-pointer group w-128">
            <a href="mailto:example@gmail.com">bergentekno@gmail.com</a>
            <div
              class="group-hover:w-96 w-0 h-2 mt-2 bg-birutua transition-all duration-500 ease-in-out"
            ></div>
          </div>
        </div>
        <div class="flex flex-row gap-x-10 pt-20">
          <a
            target="_blank"
            rel="noopener noreferrer"
            href="https://example.com/"
            class="z-50"
          >
            <img
              class="h-20 w-20"
              src="https://www.edigitalagency.com.au/wp-content/uploads/new-linkedin-logo-white-black-png.png"
              alt=""
            />
          </a>
          <a
            target="_blank"
            rel="noopener noreferrer"
            href="https://example.com/"
            class="z-50"
          >
            <img
              class="h-20 w-20"
              src="http://assets.stickpng.com/images/5ecec78673e4440004f09e77.png"
              alt=""
            />
          </a>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import { ref, onMounted, onUnmounted, computed } from "vue";

export default {
  setup() {
    const hey = ref(null);
    const letMe = ref(null);
    const intro = ref(null);
    const works = ref(null);
    const contrib = ref(null);
    const progress = ref(null);
    const progress2 = ref(null);
    const containerProg = ref(null);
    const containerProg2 = ref(null);

    onMounted(() => {
      document.addEventListener("scroll", handleScroll);
    });

    onUnmounted(() => {
      document.removeEventListener("scroll", handleScroll);
    });

    const handleScroll = (evt) => {
      const scrollY = window.scrollY;
      console.log(scrollY);

      hey.value.style.transform = "translateY(" + -scrollY + "px)";
      letMe.value.style.transform = "translateY(" + -scrollY + "px)";
      intro.value.style.transform = "translateX(" + -scrollY + "px)";
      works.value.style.transform = "translateX(" + -(scrollY - 3100) + "px)";
      contrib.value.style.transform = "translateX(" + (scrollY - 3100) + "px)";
      if (((scrollY - 4600) / 1000) * 100 < 60) {
        progress.value.style.width = ((scrollY - 4400) / 1000) * 100 + "%";
        progress2.value.style.width = ((scrollY - 4400) / 1000) * 100 + "%";
      }
    };

    const langlong = ref(false);
    const toollong = ref(false);

    const langClick = () => {
      if (toollong.value) {
        toolClick();
      }
      langlong.value = !langlong.value;
      if (langlong.value == true) {
        progress.value.style.width = "100%";
        containerProg.value.style.height = "350px";
        progress.value.style.height = "320px";
      } else {
        progress.value.style.width = "54%";
        containerProg.value.style.height = "120px";
        progress.value.style.height = "90px";
      }
    };
    const toolClick = () => {
      if (langlong.value) {
        langClick();
      }
      toollong.value = !toollong.value;
      if (toollong.value == true) {
        progress2.value.style.width = "100%";
        containerProg2.value.style.height = "350px";
        progress2.value.style.height = "320px";
      } else {
        progress2.value.style.width = "54%";
        containerProg2.value.style.height = "120px";
        progress2.value.style.height = "90px";
      }
    };

    const profpic = computed(() => {
      return {
        backgroundImage: `url(https://media.istockphoto.com/photos/close-up-photo-of-charming-beautiful-attractive-lady-offering-her-picture-id1146651911?k=20&m=1146651911&s=612x612&w=0&h=daP21YWXx7ylqX8tt8NQEeF_usPu0T0_KULwnGgi-QU=)`,
      };
    });
    const nypic = computed(() => {
      return {
        backgroundImage: `url(https://wallpaperaccess.com/full/99173.jpg)`,
      };
    });
    const dfdg = computed(() => {
      return {
        backgroundImage: `url(https://www.vandelaydesign.com/wp-content/uploads/dfdg.jpg)`,
      };
    });
    const prco = computed(() => {
      return {
        backgroundImage: `url(https://www.vandelaydesign.com/wp-content/uploads/prco.jpg)`,
      };
    });
    const adam = computed(() => {
      return {
        backgroundImage: `url(https://www.vandelaydesign.com/wp-content/uploads/adam-church.jpg)`,
      };
    });

    const goToArchio = () => {
      location.href = "https://example.com/";
    };

    const goToDuktiv = () => {
      location.href = "https://example.com/";
    };

    const goToFarma = () => {
      location.href = "https://example.com/";
    };

    return {
      hey,
      letMe,
      intro,
      profpic,
      nypic,
      dfdg,
      adam,
      works,
      contrib,
      prco,
      progress,
      progress2,
      langClick,
      toolClick,
      langlong,
      toollong,
      containerProg,
      containerProg2,
      goToArchio,
      goToFarma,
      goToDuktiv,
    };
  },
};
</script>

<style scoped>
.icon-scroll,
.icon-scroll:before {
  position: absolute;
  bottom: -125%;
}

.scroll-down {
  position: absolute;
  bottom: -145%;
  right: -3%;
}

.icon-scroll {
  width: 80px;
  height: 140px;
  box-shadow: inset 0 0 0 1px #fca311;
  border-radius: 50px;
}

.icon-scroll:before {
  content: "";
  width: 16px;
  height: 16px;
  background: #fca311;
  margin-left: 32px;
  top: 28px;
  border-radius: 50px;
  animation-duration: 1.5s;
  animation-iteration-count: infinite;
  animation-name: scroll;
}

@keyframes scroll {
  0% {
    opacity: 1;
  }
  100% {
    opacity: 0;
    transform: translateY(46px);
  }
}

.waves {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 0px;
  box-shadow: inset 0 0 50px rgba(0, 0, 0, 0.5);
}

.waves::before,
.waves::after {
  content: "";
  position: absolute;
  width: 250vw;
  height: 250vw;
  top: -65vw;
  left: 50%;
  border-radius: 44%;
  transform: translate(-50%, -75%);
}

.waves::before {
  background: rgba(51, 51, 51, 1);
  animation: waves 8s linear infinite;
}

.waves::after {
  background: #14213d;
  animation: waves 15s linear infinite;
}

@keyframes waves {
  0% {
    transform: translate(-50%, -75%) rotate(0deg);
  }
  100% {
    transform: translate(-50%, -75%) rotate(360deg);
  }
}

.rotate {
  animation: rotation 8s infinite linear;
}

@keyframes rotation {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(359deg);
  }
}

.fading {
  background: #fca311;
  animation: fading 5s infinite;
  -webkit-animation: fading 5s infinite;
}

@keyframes fading {
  0% {
    background: #fca311;
  }
  50% {
    background: #14213d;
  }
  100% {
    background: #fca311;
  }
}

@-webkit-keyframes fading {
  0% {
    background: #fca311;
  }
  50% {
    background: #14213d;
  }
  100% {
    background: #fca311;
  }
}
@keyframes opacityfading {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}

@-webkit-keyframes opacityfading {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}

.progress {
  background: rgba(255, 255, 255, 0.1);
  justify-content: flex-start;
  align-items: center;
  position: relative;
  padding-left: 15px;
  padding-right: 15px;
  display: flex;
  height: 120px;
  width: 1200px;
}

.progress-value {
  background: #fca311;
  height: 90px;
}

.wrapper {
  perspective: 2px;
}

.parallax::after {
  content: " ";
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  transform: translateZ(-1px) scale(1.5);
  background-size: 100%;
  z-index: -1;
}
</style>
