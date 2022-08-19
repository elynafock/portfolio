<template>
  <div class="contact-container">
    <a href="mailto:elinayen2000@gmail.com" style="text-decoration: none;"
      ><span class="contact"><h5 id="contact">Email Me!</h5></span></a
    >
  </div>
</template>

<style>
.contact-container {
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
}
.contact {
  height: 20rem;
  width: 20rem;
  padding: 5px;
  text-align: center;
  border-radius: 50%;
  display: inline-block;
  color: black;
  font-size: 2.5rem;
  font-weight: 600;
  background: transparent;
  border: 1px solid black;
  animation-name: floating-circle;
  animation-duration: 2s;
  animation-iteration-count: infinite;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: 0.5s all ease-in-out;
}
.contact:hover {
  background-color: black;
  color: white;
  box-shadow: 0 16px 20px rgba(0, 0, 0, 0.3);
}

h5 {
  font-family: "Playfair Display", serif;
  text-decoration: none;
}

@keyframes floating-circle {
  0% {
    transform: scale(1.1);
  }
  50% {
    transform: scale(0.8);
  }
  100% {
    transform: scale(1.1);
  }
}
</style>
