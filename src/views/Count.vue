<template>
    <div class="about">
        <h1>カウント</h1>
        <p>{{ count }}</p>
        <p>
            <button @click="increment">+</button>
            <button @click="decrement">-</button>
        </p>
    </div>
</template>

<script>
export default {
    data() {
        return {};// VueCLIを使って作るときはdataのなかにreturnをかく
    },
    methods:{
        increment() {
            this.$store.commit('increment')
        },
        decrement() {
            this.$store.commit('decrement')
        }
    },
    computed: {
        count() {
            return this.$store.getters.count;
        }
    }
};
</script>