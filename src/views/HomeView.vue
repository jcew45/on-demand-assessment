<script setup lang="ts">
</script>

<template>
  <main>
    <div class="service-item">
      <div class="item-text">
        <p>Wordpress</p>
        <p>Development</p>
        <p>Webflow</p>
        <p>Development</p>
        <p>CMS Development</p>
      </div>
      <div class="img-wrapper">
        <img src="../assets/images/web-dev-img.png" alt="animated browser image">
      </div>
    </div>
  </main>
</template>
<style lang="scss" scoped>
.service-item {
  background-color: #6274ED;
  border-radius: 8px;
  overflow: hidden;
  position: relative;
  margin: 1rem;
  width: 360px;
  height: 240px;
  &:hover {
    .img-wrapper {
      transform: translate(50%);
    }
    .item-text {
      opacity: 1;
    }
  }
  .item-text {
    padding: 1rem;
    font-size: 1.4rem;
    font-weight: 800;
    color: white;
    opacity: 0;
    transition: .8s;
  }
  .img-wrapper {
    position: absolute;
    right: -4px;
    bottom: -6px;
    transform: translate(0);
    transition: .5s cubic-bezier(0.53, -0.19, 0.53, 1.27);
  }
}
</style>