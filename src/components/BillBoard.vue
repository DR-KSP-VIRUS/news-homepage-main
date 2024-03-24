<template>
    <section class="bill-board">
        <div class="left-panel">
            <BillLeftPanel />
        </div>
        <div class="right-panel">
            <BillRightPanel />
        </div>
    </section>
</template>

<script setup>
    import BillLeftPanel from './BillLeftPanel.vue';
    import BillRightPanel from './BillRightPanel.vue';
</script>

<style scoped>
    .left-panel {
        display: flex;
        flex-direction: column;
    }
    .right-panel {
        display: flex;
        padding: 0rem 1.5rem;
        margin-top: 3rem;
        align-items: flex-start;
        flex-direction: column;
        background: var(--very-dark-blue);
    }
</style>