<template>
  <div class="container">
    <h1>Welcome!</h1>
    <p><nuxt-link to="/first">First page</nuxt-link></p>
    <p><nuxt-link to="/second">Second page</nuxt-link></p>
  </div>
</template>

<style>
/*https://coolors.co/4542e5-3625d3-7275ff-b6bee2-6fd2ff*/
html, body {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  background: #3625D3;
  color: #ffffff;
  width: 100vw;
  height: 100vh;
}

a {
  color: #7275FF;
  text-decoration: none;
}
a:hover {
  color: #B6BEE2;
  text-decoration: underline;
}

.container {
  padding: 60px;
  width: 100vw;
  height: 100vh;
  background: #3625D3;
}
.page-enter-active {
  animation: acrossIn .45s ease-out both;
} 

.page-leave-active {
  animation: acrossOut .65s ease-in both;
} 

@keyframes acrossIn {
  0% {
    transform: translate3d(-100%, 0, 0);
  }
  100% {
    transform: translate3d(0, 0, 0);
  }
}

@keyframes acrossOut {
  0% {
    transform: translate3d(0, 0, 0);
    transform-origin: left top 0px; transform: matrix(1, 0, 0, 1, 0, 0);
  }
  100% {
    transform: translate3d(100%, 0, 0);
  }
}
</style>