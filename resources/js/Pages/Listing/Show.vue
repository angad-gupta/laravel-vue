<template>
    <div>Show</div>

        {{ listing.street }}   {{ listing.baths }}   {{ listing.price }} 

</template>

<script setup>
    import { Link } from '@inertiajs/vue3';
    defineProps({
        listing: Object,
    })
</script>

