<template>
  <div>
    <h3 :class="$attrs.class.split(' ')[1]">{{ title }}</h3>
    <p>Likes : {{ likes }}</p>
    <small>Published: {{ isPublished ? "Yes" : "No" }} </small>
    <hr />
  </div>
</template>

<script>
export default {
  name: "ArticleComponent",
  data(){
    return {
    }
  },
  props: {
    title: {
      type: String,
      required: true,
      default: "Article Title",
    },
    likes: {
      type: Number,
      default: 0,
    },
    isPublished: {
      type: Boolean,
      default: false,
    },
  },
  methods: {
  },
  inheritAttrs: false,
};
</script>

<style>
</style>