<script>
import DownIcon from './Down.vue'
export default {
    components: {
      DownIcon,
    }
  }

</script>

<template>
  <article>
    <h1 id="skills" >Skills</h1>
    <div class="grid">
      <div class="grid1">Photoshop</div>
      <div class="grid2">Illustrator</div>
      <div class="grid3">Figma</div>
      <div class="grid4">Vue</div>
      <div class="grid5">React</div>
      <div class="grid6">HTML, CSS, Javascript</div>
    </div>
    <div class="down-container">
    <a href="#contact"><DownIcon/></a>
    </div>
  </article>
</template>

<style>
article {
  padding: 4rem 8rem;
  min-height: 100vh;
  font-family: "Playfair Display", serif;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
h1 {
  font-size: 80px;
  line-height: 80px;
}
.grid{
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(500px, 1fr));
}
.grid div {
  padding: 50px;
  margin: 30px;
  border-radius: 1rem;
  font-size: 30px;
  text-align: right;
}

.grid1{
    background: #f5ebe0;
}
.grid2{
    background: #d6ccc2;

}
.grid3{
    background: #edede9;

}
.grid4{
    background: #e3d5ca;

}
.grid5{
    background: #d5bdaf;

}
.grid6{
    background: #f5ebe0;

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
