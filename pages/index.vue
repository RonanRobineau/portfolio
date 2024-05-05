<template>
  <div class="first">
    <NuxtParticles id="tsparticles" :options="options" />
    <div class="welcome">
      <span>Welcome to my place</span>
      <span>Web developer, Nuxt & Vue specialist</span>
    </div>
  </div>
  <div class="second">
    <div class="appreciation">
      <UAvatar
        src="https://avatars.githubusercontent.com/u/904724?v=4"
        alt="benjamincanac"
        size="3xl"
      />
      <div class="text">
        <i>what a man</i>
        <div>Atinux</div>
      </div>
    </div>
    <div class="appreciation">
      <UAvatar
        src="https://avatars.githubusercontent.com/u/904724?v=4"
        alt="benjamincanac"
        size="3xl"
      />
      <div class="text">
        <i>what a man</i>
        <div>Atinux</div>
      </div>
    </div>
    <div class="appreciation">
      <UAvatar
        src="https://avatars.githubusercontent.com/u/904724?v=4"
        alt="benjamincanac"
        size="3xl"
      />
      <div class="text">
        <i>what a man</i>
        <div>Atinux</div>
      </div>
    </div>
    <div class="appreciation">
      <UAvatar
        src="https://avatars.githubusercontent.com/u/904724?v=4"
        alt="benjamincanac"
        size="3xl"
      />
      <div class="text">
        <i>what a man</i>
        <div>Atinux</div>
      </div>
    </div>
  </div>
</template>

<script setup>
// import { curvesPathName } from "@tsparticles/path-curves";
import "./index.css";
const options = {
  fpsLimit: 120,
  fullScreen: false,
  particles: {
    color: {
      value: "#FF0000",
    },
    move: {
      direction: "none",
      enable: true,
      outModes: {
        default: "destroy",
      },
      path: {
        clamp: false,
        enable: true,
        delay: {
          value: 0,
        },
        // generator: curvesPathName,
      },
      random: false,
      speed: 2,
      straight: false,
      trail: {
        fill: {
          color: "#000",
        },
        length: 30,
        enable: true,
      },
    },
    number: {
      value: 0,
      limit: { value: 300 },
    },
    opacity: {
      value: 1,
    },
    shape: {
      type: "circle",
    },
    size: {
      value: { min: 1, max: 10 },
      animation: {
        count: 1,
        startValue: "min",
        enable: true,
        speed: 10,
        sync: true,
      },
    },
  },
  background: {
    color: "#000",
  },
  detectRetina: true,
  emitters: {
    direction: "none",
    rate: {
      quantity: 10,
      delay: 0.3,
    },
    size: {
      width: 0,
      height: 0,
      mode: "precise",
    },
    spawnColor: {
      value: "#ff0000",
      animation: {
        h: {
          enable: true,
          offset: {
            min: -1.4,
            max: 1.4,
          },
          speed: 5,
          sync: false,
        },
        l: {
          enable: true,
          offset: {
            min: 20,
            max: 80,
          },
          speed: 0,
          sync: false,
        },
      },
    },
    position: {
      x: 50,
      y: 50,
    },
  },
};
// const onLoad = (container) => {
//   // Do something with the container
//   container.pause();
//   setTimeout(() => container.play(), 2000);
// };
</script>
