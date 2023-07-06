<template>
    <div>Show</div>

        {{ listing.street }}

</template>

<script setup>
    import { Link } from '@inertiajs/vue3';
    defineProps({
        listing: Object,
    })
</script>

