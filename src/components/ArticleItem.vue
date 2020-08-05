<template>
  <b-card
    title="Card 1"
    img-src="https://via.placeholder.com/318x159"
    img-alt="Image"
    img-top
    tag="article"
    class="mb-2"
  >
    <b-card-text>{{post.content}}</b-card-text>
  </b-card>
</template>

<script>
export default {
  name: "ArticleItem",
  props: {
    post: Object,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
</style>