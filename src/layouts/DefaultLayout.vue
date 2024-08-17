<script setup>
import TheHeader from "@/components/TheHeader.vue";
import TheCategory from "@/components/TheCategory.vue";
import TheFooter from "@/components/TheFooter.vue";
</script>

<template>
    <!-- Header navbar -->
    <TheHeader />
    <!-- Main Content -->
    <div class="grid grid-cols-12 gap-6">
        <!-- Sidebar -->
        <TheCategory />
        <!-- Book row -->
        <div class="col-span-10 mt-6">
            <router-view />
        </div>
    </div>
    <TheFooter />
</template>

<style scoped></style>
