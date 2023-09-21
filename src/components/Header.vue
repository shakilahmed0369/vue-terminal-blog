<template>
  <header class="header">
    <div class="header__inner">
      <div class="header__logo">
        <a href="/">
          <div class="logo">Shakil's | Tech blog</div>
        </a>
      </div>
      <div class="menu-trigger" @click="menuToggle">menu</div>
    </div>

    <nav class="menu" v-show="menu">
      <ul class="menu__inner menu__inner--desktop">
        <li>
          <a href="https://github.com/creekorful/blog">Blog source code</a>
        </li>

        <li><a href="https://github.com/creekorful">Github</a></li>

        <li><a href="https://www.linkedin.com/in/creekorful">Linkedin</a></li>

        <li><a href="https://www.creekorful.org">Website</a></li>
      </ul>

      <ul class="menu__inner menu__inner--mobile">
        <li>
          <a href="https://github.com/creekorful/blog">Blog source code</a>
        </li>

        <li><a href="https://github.com/creekorful">Github</a></li>

        <li><a href="https://www.linkedin.com/in/creekorful">Linkedin</a></li>

        <li><a href="https://www.creekorful.org">Website</a></li>
      </ul>
    </nav>
  </header>
</template>

<script setup>
import { ref } from 'vue';

const menu = ref(false);

const menuToggle = () => {
    menu.value = !menu.value;
}
</script>

<style lang="css" scoped>
.menu-trigger {
    cursor: pointer;
}
</style>
