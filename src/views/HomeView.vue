<script setup>
import IconButton from '../components/IconButton.vue';
import config from '../config';
</script>

<template>
  <div class="home-wrapper">
    <IconButton label="fas fa-chevron-up" color="var(--color-on-main-card-secondary)"></IconButton>
    <div class="ui-tips">Scroll to see more</div>
    <div class="bio">{{ config.BIO }}</div>
  </div>
</template>

<style scoped>
.home-wrapper {
  position: absolute;
  top: 0;
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding-top: 20px;
}

.ui-tips {
  color: var(--color-on-main-card-secondary);
  font-size: 20px;
}

.bio {
  color: var(--color-on-main-card-primary);
  font-size: 25px;
  margin-top: 20px;
  text-align: center;
}
</style>
