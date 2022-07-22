<template>
  <div>
    <header>
      <h1>header</h1>
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
        color: #fff;
        padding: 20px;
        background-color: #527b8e;
    }
</style>
