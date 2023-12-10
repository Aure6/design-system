<script setup>
defineProps({
    to: {
        type: String,
        required: true,
    },
});
</script>

<template>
    <div>
        <slot />
    </div>
</template>
