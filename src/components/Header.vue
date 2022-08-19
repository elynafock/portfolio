<script>
import DownIcon from './Down.vue';
import Circle from "./Circle.vue"

  export default {
    components: {
      DownIcon,
      Circle
    }
  }

</script>

<template>
<header>
<div>
  <!-- <h1>I'm</h1> -->
  <h1>Elyna <div class="fock">Fock</div></h1>

  <!-- <h2>UI/UX Designer | Software Engineer Student</h2> -->
  </div>
<div>
  <img src="../assets/profile.jpg" alt="Profile Thumbnail">
</div>
</header>
<div class="down-container">
  <a href= "#about"><DownIcon/></a>
</div>
</template>

<style scoped>
header {
  display: flex;
  align-items:center;
  justify-content: space-between;
  padding: 5rem 8rem;
}

strong {
  font-weight: 500;
  font-size: 12rem;
}

img {
  width: 100%;
  max-width: 300px;
}

h1 {
  font-size: 14rem ;
  line-height: 1;
  color: #000000;
font-family: 'Poppins', sans-serif;
;
}

.fock {
  margin-left: 12rem;

}

.down-container {
  text-align: center;
  animation-name: down-arrow;
  animation-duration: 2s;
  animation-iteration-count: infinite;
}

@keyframes down-arrow {
  0% {
    transform: translateY(-10px);
  }
  50% {
    transform: translateY(10px);
  }
  100%{
    transform: translateY(-10px);
  }
}
</style>