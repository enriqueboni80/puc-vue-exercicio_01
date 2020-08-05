<template>
  <div class="Articles">
    <b-container>
      <b-row class="mt-4">
        <b-col v-for="post in posts" v-bind:key="post.content" cols="4">
          <ArticleItem :post="post" />
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import ArticleItem from "./ArticleItem.vue";

export default {
  name: "Articles",
  components: {
    ArticleItem,
  },
  props: {
    posts: Array,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
</style>