<template>
    <div>
        <UButton @click="addRow"> Add Row</UButton>
        <UTable :data="data" />
        <div>{{ data }}</div>
    </div>
</template>

<script setup>
const data = ref([]);

const addRow = () => {
    data.value.push({ id: 1, random: Math.random() });
};
</script>

<style>
@import "tailwindcss";
@import "@nuxt/ui";
</style>
