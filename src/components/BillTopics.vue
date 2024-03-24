<template>
    <div class="topics" v-for="topic in topics" :key="topic.id">
        <a href="#">{{ topic.title }}</a>
        <p>{{ topic.text }}</p>
    </div>
</template>

<script setup>
    const props = defineProps({
        topics:{
            type: Array,
            required: true,
        }
    })
</script>

<style scoped>
    .topics {
      padding: 2rem 0 2.15rem 0;
      border-bottom: 1px solid var(--dark-grayish-blue);
    }
    .topics a {
      color: var(--off-white);
      font-family: 'Inter-Bold';
      letter-spacing: .1rem;
      font-size: 1.5rem;
      margin-bottom: 2rem;
      transition: all 0.54s ease-in-out;
    }
    .topics a:hover {
        color: var(--soft-orange)
    }
    .topics > p {
      color: var(--dark-grayish-blue);
      font-family: 'Inter-Regular';
      padding-top: 1rem;
      line-height: 2rem;
      font-size: large;
    }
</style>