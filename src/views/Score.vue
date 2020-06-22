<template>
  <div class="about">
    <h1>スコア表示</h1>
    <p>{{ count }}</p>
  </div>
</template>

<script>
export default {
    data() {
        return {};// VueCLIを使って作るときはdataのなかにreturnをかく
    },
    computed: {
        count() {
            return this.$store.getters.count;
        }
    }
};
</script>