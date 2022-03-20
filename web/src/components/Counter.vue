<script setup lang="ts">
import { reactive } from 'vue';

const state = reactive({count: 0});

function increment() {
    state.count += 1;
}

</script>

<template>
    <main class="w-screen h-screen bg-gray-600 flex flex-col justify-center items-center">
        <h1 class="text-xl text-white font-semibold">{{ state.count }}</h1>
        <button @click="increment" class="bg-green-500 font-semibold text-xl px-3 py-1 rounded-lg">click</button>
    </main>
</template>