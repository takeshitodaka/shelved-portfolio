<template>
  <div>
    <header>
      <h1>Welcome to Takeshi's Portfolilo</h1>
      <HeaderNav />
    </header>
  </div>
</template>

<script>
import HeaderNav from '@/components/headerNav.vue'
export default {
  components: {
    HeaderNav
  }
}
</script>

<style scoped>
    header{
        color: rgb(255, 255, 255);
        padding: 20px;
        background-color: #3100e1;
    }
</style>
