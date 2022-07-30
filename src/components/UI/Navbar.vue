<template>
  <div class="navbar">
    <div class="navbar__btns">
      <my-button @click="$router.push('/')">Главная</my-button>
      <my-button @click="$router.push('/posts')" style="margin: 0 15px"
        >Посты</my-button
      >
      <my-button @click="$router.push('/about')">О сайте</my-button>
      <my-button @click="$router.push('/store')" style="margin-left: 15px">Хранилище</my-button>
    
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.navbar {
  display: flex;
  height: 50px;
  background-color: lightgray;
  box-shadow: 2px 2px 4px black;
  align-items: center;
  padding: 0 15px;
}
.navbar__btns {
  margin-left: auto;
}
</style>
