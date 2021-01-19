<template>
<div  id="warning" light>   <a href="/"><img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQWdYrYoPZbkz2o-Cvb9cpnqVRTgYozkj4gyg&usqp=CAU" alt="" class="logo-img"></a>
Amalitech Front-Desk Portal
</div>
  <div id="nav">
    <router-link to="/"><button class="btn">Home</button></router-link>
    <router-link to="/about"><button class="btn">About</button></router-link>
<router-link to="/SignOut"><button class="btn">SignOut</button></router-link>
    </div>
  <router-view />
</template>

<style>
.logo-img{
  padding: 0 4rem;
  margin: 3px;
  width: 10%;
  height: 60%;
}
#app {
  font:montserrat;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding-bottom: 10px;
  margin: 10px;
  display: flex;
  padding: 0 2px;
  margin: 0px;
  justify-content: space-between;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>

<style scoped>
#warning {
  display: inline-block;
  background-color: #690009;
  height: 35px;
  width: 1200%;
  padding: 10px 0 0 30px;
  padding-right: 90px;
  color: #eb8818;
  align-items: left;
  max-width: 120%;
}
#warning{
  font-size: 25px;
  color: rgb(243, 151, 13);
  text-align: justify;
  -webkit-animation: glow 2s ease-in-out infinite alternate;
  -moz-animation: glow 1s ease-in-out infinite alternate;
  animation: glow 3s ease-in-out infinite alternate;
}

/* @-webkit-keyframes glow {
  from {
    text-shadow: 0 0 10px rgb(240, 157, 48), 0 0 20px rgb(53, 50, 21), 0 0 30px #e69600, 0 0 40px #e68200, 0 0 50px #e4850a, 0 0 60px #e69600, 0 0 70px #d67e13;
  }
  to {
    text-shadow: 0 0 20px rgb(214, 159, 8), 0 0 30px #c5a40f, 0 0 40px #f1a007, 0 0 50px hsl(34, 89%, 51%), 0 0 60px #ff4da6, 0 0 70px #ff4da6, 0 0 80px #ff4da6;
  }
} */

.btn {
  display: inline-block;
  padding: 0.8rem 2rem;
  text-decoration: none;
  font: inherit;
  font-size: 20px;
  font-weight: bold;
  border: 2.5px solid #690009;
  color: #a7082f;
  background: rgb(245, 213, 176);
  border-radius: 40px 5px;
  cursor: pointer;
  outline: none;
}

.btn:hover,
.btn:active {
  background-color: #ffa33b;
  color: rgb(252, 250, 180);
}

.btn.danger {
  color: red;
  border-color: red;
}

.btn.danger:hover,
.btn.danger:active {
  background: red;
  color: rgb(255, 255, 255);
}
</style>
