<template>
  <div>
    <nav>
      <ul>
        <li>
          <a href="https://github.com/bichoamant?tab=repositories" target="_blank">
            <img src="@/assets/image/github.png">
          </a>
          <a href="https://twitter.com/0vKXFvw2uUeDITn" target="_blank">
            <img src="@/assets/image/twitter.png">
          </a>
          <a href="https://www.instagram.com/takeshivancouver1983/" target="_blank">
            <img src="@/assets/image/instagram.png">
          </a>
          <a href="https://bichoamant.livedoor.blog/" target="_blank">
            <img src="@/assets/image/blog.png">
          </a>
          <nuxt-link to="/message">
            <img src="@/assets/image/message.png">
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

<style>
nav {
text-align: center;
}
nav ul{
  list-style-type: none;
}
nav ul li img{

  width: 70px;
  height: auto;
  margin-right: 20px;
  margin-left: 20px;
}

</style>
