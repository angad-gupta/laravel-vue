<template>
    <div>
        {{ listing.street }}
    </div>
</template>
<script setup>

    defineProps({
        listing: Array,
    })
</script>

