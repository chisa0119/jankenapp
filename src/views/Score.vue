<template>
  <div class="about">
    <h1>スコア表示</h1>
  </div>
</template>

<script>
export default {
    computed: {
        count() {
            return this.$store.getters.count;
        }
    }
};
</script>