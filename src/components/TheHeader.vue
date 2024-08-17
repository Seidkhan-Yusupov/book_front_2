<script setup></script>
<template>
    <header class="bg-gray-800">
        <ul class="flex indent-10 text-white font-bold">
            <router-link to="/" class="cursor-pointer hover:text-gray-500 p-3"
                >Bosh sahifa</router-link
            >
            <li class="cursor-pointer hover:text-gray-500 p-3">Kitoblar</li>
            <li class="cursor-pointer hover:text-gray-500 p-3">
                Bestsellerlar
            </li>
            <li class="cursor-pointer hover:text-gray-500 p-3">
                Shaxsiy Kabinet
            </li>
            <router-link
                to="/login"
                class="cursor-pointer hover:text-gray-500 p-3"
                >Kirish</router-link
            >
            <li class="cursor-pointer hover:text-gray-500 p-3">Chiqish</li>
        </ul>
    </header>
</template>
<style scoped></style>
