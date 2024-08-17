<template>
    <div class="grid grid-cols-12 gap-6">
        <!-- Books -->
        <TheBook />
        <!-- Pagination -->
    </div>
    <ThePagination />
</template>

<script setup>
import TheBook from "@/components/TheBook.vue";
import ThePagination from "@/components/ThePagination.vue";
</script>

<style scoped></style>
