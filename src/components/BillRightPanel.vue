<template>
    <h2>New</h2>
    <BillTopics :topics = "topics"/>
</template>

<script setup>
    import { ref } from 'vue';
    import BillTopics from './BillTopics.vue';

    const topics = ref([
        {
            id: 1,
            title: "Hydrogen VS Electric Cars",
            text: "Will hydrogen-fueled cars ever catch up to EVs?"
        },
        {
            id: 2,
            title: "The Downsides of AI Artistry",
            text: "What are the possible adverse effects of on-demand AI image generation?"
        },
        {
            id: 3,
            title: "Is VC Funding Drying Up?",
            text: "Private funding by VC firms is down 50% YOY. We take a look at what that means"
        }
    ]);
</script>

<style scoped>
    .right-panel h2 {
        color: var(--soft-orange);
        font-family: 'Inter-ExtraBold';
        letter-spacing: 2px;
        padding: 2rem 0 .6rem 0;
        font-size: 30px;
    }
</style>