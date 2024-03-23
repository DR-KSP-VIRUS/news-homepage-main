<template>
    <div class="services">
        <Service :services="services"/>
    </div>
</template>

<script setup>
    import { ref } from 'vue';
    import Service from './Service.vue';

    const services = ref([
        {
            id: 1,
            title: "Reviving Retro PCs",
            text: "What happens when old PCs are given modern upgrades",
            image: "/images/image-retro-pcs.jpg"
        },
        {
            id: 2,
            title: "Top 10 Laptops of 2022",
            text: "Our best picks for various needs and budgets",
            image: "/images/image-top-laptops.jpg"
        },
        {
            id: 3,
            title: "The Growth of Gaming",
            text: "How the pandemic has sparked fresh opportunities",
            image: "/images/image-gaming-growth.jpg"
        }
    ]);
</script>