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
    <h1 class="text-5xl uppercase italic [text-shadow:2px_2px_2px_var(--tw-shadow-color)] shadow-red-500">{{ title }}</h1>
</template>
