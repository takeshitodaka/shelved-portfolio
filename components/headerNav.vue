<template>
  <div>
    <nav>
      <ul>
        <li class="header-links">
          <nuxt-link to="/">
            TOP
          </nuxt-link>
          <nuxt-link to="/">
            Resume
          </nuxt-link>
          <nuxt-link to="/">
            Experience
          </nuxt-link>
          <nuxt-link to="/">
            Skills
          </nuxt-link>
          <nuxt-link to="/">
            About
          </nuxt-link>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  components: {}
}
</script>
<style scoped>
.header-links a{
  font-size: 40px;
    margin-left: 20px;
    margin-right: 20px;
}

</style>
