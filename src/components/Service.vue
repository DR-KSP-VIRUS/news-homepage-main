<template>
    <div class="service" v-for="service in services" :key="service.id">
        <img :src="service.image" alt="img">
        <div>
            <p>0{{ service.id }}</p>
            <a href="#">{{ service.title }}</a>
            <p>{{ service.text }}</p>
        </div>
    </div>
</template>

<script setup>
    const props = defineProps({
        services: {
            type: Array,
            required: true
        }
    });

</script>

<style>
    .service {
        display: flex;
        align-items: flex-start;
        justify-content: center;
        flex-direction: row;
        margin: 1.2rem 0;
    }
    .service img {
        width: 100px;
        height: 100%;
    }
    .service p:first-of-type {
        font-size: 25px;
        font-family: 'Inter-ExtraBold';
        color: var(--grayish-blue);
        margin: 0 1rem .5rem;
    }
    .service a {
        font-family: 'Inter-ExtraBold';
        font-size: 20px;
        margin: 1rem 0 1.2rem 1.2rem;
        display: flex;
        align-items: flex-start;
        color: var(--dark-blue);
        cursor: pointer;
        transition: all 0.54s ease-in-out;
    }
    .service a:hover {
        color: var(--soft-red);
    }
    .service p:last-of-type {
        font-size: 19px;
        font-family: 'Inter-Regular';
        margin: 1rem 0 1.2rem 1.2rem;
        line-height: 1.9rem;
        color: var(--dark-grayish-blue);
    }
</style>