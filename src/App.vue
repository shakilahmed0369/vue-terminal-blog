<script setup>
import './assets/style.css'
import { RouterLink, RouterView } from "vue-router";
import Header from './components/Header.vue';

</script>

<template>
  <div class="container center headings--one-size">

    <Header />

    <RouterView />


    <footer class="footer">
      <div class="footer__inner">
        <div class="copyright">
          <span>© 2021 Powered by <a href="http://gohugo.io">Hugo</a></span>

          <span
            >:: Theme made by <a href="https://twitter.com/panr">panr</a></span
          >
        </div>
      </div>
    </footer>

    This website is open source. <br />
    Feel free to submit a PR if you spot a mistake :)<br /><br />

    <a href="https://github.com/creekorful/blog"
      >https://github.com/creekorful/blog</a
    >
  </div>

</template>
