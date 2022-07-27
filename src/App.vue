<template>
  <div class="app">
    <post-form @create="createPost"></post-form>
    <post-list :posts="posts"></post-list>
  </div>
</template>

<script>
import PostForm from "./components/PostForm.vue";
import PostList from "./components/PostList.vue";

export default {
  components: {
    PostForm,
    PostList,
  },

  data() {
    return {
      posts: [
        { id: 1, title: "JS 1", body: "Описание поста" },
        { id: 2, title: "JS 2", body: "Описание поста" },
        { id: 3, title: "JS 3", body: "Описание поста" },
      ],
    };
  },
  methods: {
    createPost(post) {
      this.posts.push(post);
    },
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.app {
  padding: 20px;
}
</style>
