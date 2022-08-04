<template>
  <div class="greetings">
    <div class="greetings-text">
      <h5>Hi, my name is</h5>
      <h1>Emmanuel Perez</h1>
      <h3>I'm a front-end <span class="highlight">web developer</span></h3>
    </div>
  </div>
  <span class="scroll">▽ SCROLL ▽</span>
  <div class="about">
    <p class="about-text">
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. Inventore sed
      veniam illo praesentium exercitationem enim sequi, dolorem, consequatur
      ducimus doloribus deserunt, minima maiores. Voluptates amet cumque omnis,
      dolore in ut? lorem ipsum dolor sit amet consectetur adipisicing elit.
      Inventore sed veniam illo praesentium exercitationem enim sequi, dolorem,
      consequatur ducimus doloribus deserunt, minima maiores. Voluptates amet
      cumque omnis, dolore in ut? Lorem ipsum, dolor sit amet consectetur
      adipisicing elit. Maxime similique nemo cupiditate maiores reprehenderit
      sunt repellendus autem animi, atque ullam reiciendis dolores ipsam illo
      nisi ducimus quasi dolore aut! Deserunt. Tempore aspernatur magnam numquam
      natus dolores illum quos, sunt rem, pariatur optio excepturi. Nam
      repudiandae, voluptatem totam fugiat aliquid fuga eligendi vitae, est
      ducimus magnam voluptatum, optio quidem earum unde. Qui esse fuga magnam,
      ut blanditiis iusto incidunt. Accusantium ipsum, eligendi ipsa ad iusto
      similique veniam provident minus reprehenderit, officiis tenetur, et
      architecto explicabo quod libero adipisci? Iure, placeat fuga?
    </p>
  </div>
</template>

<script setup lang="ts"></script>

<style>
.greetings {
  animation-fill-mode: forwards;
  animation-iteration-count: 1;
  animation: fadeInAnimation ease 4s;
  display: flex;
  font-size: 3rem;
  justify-content: center;
  padding-right: 10%;
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
  animation: fadeInRight ease 4s;
  padding-top: 6rem;
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
  animation: scroll 3s ease infinite;
  display: flex;
  justify-content: center;
  padding-top: 8rem;
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

.fadeOut {
  animation: fadeOut ease 2s;
  display: flex;
  justify-content: center;
}

@keyframes fadeOut {
  0% {
    opacity: 1;
  }
  100% {
    opacity: 0;
  }
}

.about {
  display: flex;
  justify-content: center;
  padding-top: 3rem;
}

.about-text {
  width: 60%;
  line-height: 2rem;
}

/* MEDIA QUERY */

@media (max-width: 940px) {
  .greetings {
    font-size: 2.5rem;
    padding-right: 0;
  }
  .greetings-text {
    padding-top: 4rem;
  }
}

@media (max-width: 840px) {
  .greetings {
    font-size: 1.5rem;
    padding-right: 0;
  }
  .greetings-text {
    padding-top: 2rem;
  }
}
</style>
