<template>
  <div class="container article-tab">
    <div class="tab-content" id="nav-tabContent">
      <div
        class="tab-pane fade show active"
        id="nav-for-you"
        role="tabpanel"
        aria-labelledby="nav-for-you-tab"
        tabindex="0"
      >
        <ArticleList></ArticleList>
      </div>
      <div
        class="tab-pane fade"
        id="nav-following"
        role="tabpanel"
        aria-labelledby="nav-following-tab"
        tabindex="0"
      >
        <ArticleList></ArticleList>
      </div>
      <div
        class="tab-pane fade"
        id="nav-bookmark"
        role="tabpanel"
        aria-labelledby="nav-bookmark-tab"
        tabindex="0"
      >
        <ArticleList></ArticleList>
      </div>
    </div>
  </div>
</template>

<script>
import ArticleList from "./ArticleList.vue";

export default {
  name: "App",
  components: {
    ArticleList,
  },
};
</script>

<style scoped>
.article-tab {
  position: relative;
  left: 2%;
  top: 3%;
}
</style>