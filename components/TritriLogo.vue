<template>
  <img
    class="TritriLogo"
    alt="TritriLogo"
    src="/tritrilogo.png"
  >
</template>

<style>
.TritriLogo {
  height: 180x;
  width: 180px;
  transform: rotateY(560deg);
  animation: turn 3.5s ease-out forwards 1s;
}

@keyframes turn {
  100% {
    transform: rotateY(0deg);
  }
}
</style>
