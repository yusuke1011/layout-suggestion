<template>
  <div id="app">
    <h1>レイアウト提案</h1>
    <p class="margin"></p>
    <b-button
      type="button"
      size="lg"
      variant="outline-primary"
      v-on:click="start"
    >開始する</b-button>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: "App",
  methods: {
    start() {
      //mode_options画面へ遷移
      this.$router.push("/mode_options");
    }
  }
};
</script>
