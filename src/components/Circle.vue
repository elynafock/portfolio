<script>
const title = "about-me".toUpperCase();
export default {
  data() {
    return {
      title,
    };
  },
};
</script>

<template>
  <div class="circle-container">
    <h3>
      <span v-for="(char, index) in title" :class="'w' + (index + 1)" >
        {{ char }}
      </span>
    </h3>
  </div>
</template>

<style>
.circle-container {
  position: relative;
  border-radius: 50%;
  transform: translateX(200px);
  animation-name: spin;
  animation-duration: 5s;
  animation-iteration-count: infinite;
}
h3 span {
  --deg: 22.5deg;
  height: 200px;
  position: absolute;
  width: 20px;
  left: 0;
  bottom: 0;
  transform-origin: bottom center;
}
.w1 {
  transform: rotate(calc(var(--deg) * 1));
}
.w2 {
  transform: rotate(calc(var(--deg) * 2));
}
.w3 {
  transform: rotate(calc(var(--deg) * 3));
}
.w4 {
  transform: rotate(calc(var(--deg) * 4));
}
.w5 {
  transform: rotate(calc(var(--deg) * 5));
}
.w6 {
  transform: rotate(calc(var(--deg) * 6));
}
.w7 {
  transform: rotate(calc(var(--deg) * 7));
}
.w8 {
  transform: rotate(calc(var(--deg) * 8));
}

@keyframes spin {
  0% {
    transform: rotate(0deg);
  }

  50% {
    transform: rotate(180deg);
  }

  100% {
    transform: rotate(360deg);
  }
}

</style>
