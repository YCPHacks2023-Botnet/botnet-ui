<script setup>
import Index from './components/Index.vue'
import BotsList from './components/BotsList.vue'
</script>

<template>
  <header>
    <img alt="Logo" class="logo" src="./assets/ForkPepe.jpg" width="125" height="125" />

    <div class="wrapper">
      <Index msg="Dotnetbotnet Overview" />
    </div>
  </header>

  <main>
    <BotsList />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  
}

@media (min-width: 1024px) {
  header {

  }

  .logo {
  
  }

  header .wrapper {
  
  }
}
</style>
