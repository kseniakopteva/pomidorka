<script setup>
    import { defineProps } from "vue";
    defineProps({
        title: {
            type: String,
            required: true,
        },
    });
</script>

<template>
    <div class="border-b border-red-700 p-2 m-2 text-center">
        <h2 class="text-2xl">{{ title }}</h2>
    </div>
</template>
