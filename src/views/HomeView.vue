<script setup>
import Post from '../components/Post.vue';
</script>

<template>
  <div class="content">
    <div class="posts">

      <Post />

      <div class="pagination">
        <div class="pagination__buttons">
          <span class="button next">
            <a href="/page/2/">
              <span class="button__text">Older posts</span>
              <span class="button__icon">→</span>
            </a>
          </span>
        </div>
      </div>
    </div>
  </div>
</template>
