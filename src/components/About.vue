<script>
import DownIcon from "./Down.vue";
import Circle from "./Circle.vue";

export default {
  components: {
    DownIcon,
    Circle,
  },
};
</script>

<template>
  <div class="container">
    <article>
      <h2 class="aboutme" id="about" >
        About
        <div class="me">Me</div>
      </h2>
      <h3 class="position">UI / UX Designer | Software Engineer Student</h3>
      <h4 class="description">
        I love blending technologies with art, hoping when it comes to telling
        about technologies, we don't only think about the sense of cold and stern
        touch. My work is about blending in technologies and designs, making them
        alive and warmth.
      </h4>
    </article>
    <div class="circle-wrapper">
      <Circle/>
    </div>
  </div>
  <div class="down-container">
    <a href="#skills">
      <DownIcon />
    </a>
  </div>
</template>

<style>
.circle-wrapper {
  display: flex;
  justify-content: center;
  width: 100%;
}
article {
  padding: 4rem 8rem;
  min-height: 100vh;
  font-family: "Playfair Display", serif;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.aboutme {
  font-size: 80px;
  line-height: 80px;
}
.me {
  margin-left: 12rem;
}
.position {
  margin-top: 4rem;
  font-size: 30px;
}
.description {
  font-size: 18px;
  width: 600px;
  padding: 12px 0px;
}
.down-container {
  text-align: center;
  animation-name: down-arrow;
  animation-duration: 2s;
  animation-iteration-count: infinite;
}
.container{
  display: flex;
  align-items: center;
}
@keyframes down-arrow {
  0% {
    transform: translateY(-10px);
  }
  50% {
    transform: translateY(10px);
  }
  100% {
    transform: translateY(-10px);
  }
}
</style>
