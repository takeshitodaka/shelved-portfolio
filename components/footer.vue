<template>
  <div>
    <footer>
      Contact me!
      <FooterNav />
    </footer>
  </div>
</template>

<script>
import FooterNav from '@/components/footerNav.vue'
export default {
  components: {
    FooterNav
  }
}
</script>
<style scoped>
    footer{
      font-size: 30px;
        color: rgb(255, 255, 255);
        padding: 20px;
        background-color: #3100e1;
    }
</style>
