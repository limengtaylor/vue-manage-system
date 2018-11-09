<template>
  <div class="flex">
    <top></top>
    <left></left>
    <div class="center">
      <tag></tag>
      <div class="content">
        <keep-alive>
          <router-view></router-view>
        </keep-alive>
      </div>
    </div>
  </div>
</template>
<script>
import bus from './bus';
import top from './Top.vue';
import left from './Left.vue';
import tag from './tag.vue';
export default {
  components: {
    top,
    left,
    tag
  }
};
</script>

