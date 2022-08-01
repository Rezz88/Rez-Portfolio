<template>
  <!-- Nav bar -->
  <Navigation />
  <!-- Main content -->
  <Greeting/>
  <!-- Contact -->
  <SocialIcon />
</template>

<script setup lang="ts">
import SocialIcon from "../components/SocialIcons.vue";
import Navigation from "../components/Navigation.vue";
import Greeting from "../components/Greeting.vue";
</script>
