<script setup>
import {router} from "@inertiajs/vue3";
import {route} from "ziggy-js";

const logout = () => {
    router.post(route('logout'));
};
</script>

<template>
    <h1 class="text-2xl font-bold">Dashboard</h1>
    <a :href="logout" class="text-white bg-red-500 px-4 py-2 rounded-lg">
        Logout
    </a>
</template>


