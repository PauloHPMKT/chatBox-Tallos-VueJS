<template>
  <main>
    <ChatBox />
    <img src="img/user.svg" alt="">
  </main>
</template>

<script>
import ChatBox from '@/components/ChatBox.vue';

export default {
  name: 'home',
  components: {
    ChatBox,
  }
}
</script>

<style>
  img {
    width: 100px;
  }
</style>
