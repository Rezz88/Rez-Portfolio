<template>
  <div class="greetings">
    <div class="greetings-text">
      <h5>Hi, my name is</h5>
      <h1>Emmanuel Perez</h1>
      <h3>I'm a front-end <span class="highlight">web developer</span></h3>
    </div>
  </div>
  <span class="scroll">▽ SCROLL ▽</span>
</template>

<style>
.greetings {
  display: flex;
  justify-content: center;
  font-size: 3rem;
  padding-right: 10%;
  animation: fadeInAnimation ease 4s;
  animation-iteration-count: 1;
  animation-fill-mode: forwards;
}

@keyframes fadeInAnimation {
  0% {
    opacity: 0;
    transform: translateX(-20px);
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

.highlight {
  color: gold;
  text-shadow: -2px -1px white;
}

.greetings-text {
  padding-top: 6rem;
  animation: fadeInRight ease 4s;
}

@keyframes fadeInRight {
  0% {
    opacity: 0;
    transform: translateX(50px);
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

h1,
h3,
h5 {
  margin: 0;
}

.scroll {
  display: flex;
  justify-content: center;
  padding-top: 8rem;
  animation: scroll 3s ease infinite;
}

@keyframes scroll {
  0% {
    opacity: 0;
    transform: translateY(-20px);
  }
  70% {
    transform: translateY(0%);
  }
  80% {
    opacity: 1;
    transform: translateY(-6%);
  }
  90% {
    transform: translateY(0%);
  }
  95% {
    transform: translateY(-4%);
  }
  97% {
    transform: translateY(0%);
  }
  99% {
    transform: translateY(-2%);
  }
  100% {
    opacity: 0;
    transform: translateY(0);
  }
}
</style>
