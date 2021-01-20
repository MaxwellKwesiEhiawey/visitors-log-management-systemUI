<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png" /> -->
    <h3 class="welcome-msg">Welcome to Amalitech Front-desk</h3>
    <HelloWorld msg="" />
  </div>
  <div></div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
export default {
  name: "Home",
  components: {
    HelloWorld
  }
};
</script>
<style scoped>
.welcome-msg {
  position: relative;
  padding-top: 40px;
  font-family: sans-serif;
  text-transform:capitalize;
  font-size: 2em;
  font-style: italic;
  letter-spacing: 4px;
  overflow: hidden;
  background: linear-gradient(90deg, rgb(233, 31, 31), rgb(243, 189, 10), rgb(253, 62, 62));
  background-repeat: no-repeat;
  background-size: 80%;
  animation: animate 10s linear infinite;
  -webkit-background-clip:text;
  -webkit-text-fill-color: rgba(197, 48, 73, 0);
}

@keyframes animate {
  0% {
    background-position: -500%;
  }
  100% {
    background-position: 500%;
  }
}
.home{
  height: 400px;
 width:100vw;
}
</style>
