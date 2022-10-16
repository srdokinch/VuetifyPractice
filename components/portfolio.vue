<template>
  <v-container>
    <div id="component-profile" class="d-flex flex-column justify-center align-center">
      <img src="~assets/img/panko.jpg" alt="">
      <h1 class="my-5">{{ name }}</h1>
      <p>{{ description }}</p>
      <ul class="sns d-flex px-0">
        <li class="mx-2"><a href="https://twitter.com/fatfatpankocat"><i class="fab fa-twitter fa-lg"></i></a></li>
        <li class="mx-2"><a href="https://www.instagram.com/fatfatpankocat/"><i class="fab fa-instagram fa-lg"></i></a></li>
      </ul>
    </div>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      name: 'Panko',
      description: 'A professional cat'
    }
  }
}
</script>

<style lang="scss" scoped>
  #component-profile {
    height: 100vh;
    img {
      border-radius: 50px;
      object-fit: cover;
      height: 300px;
      width: 300px;
    }
    .sns {
      list-style: none;
      i {
        color: #fff;
      }
    }
  }
</style>