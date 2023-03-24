<template>
    <div class="flex items-center justify-center h-screen w-full">
        <div class="border-red-400 border-2 ronded-lg p-4 flex flex-col">
            <input class="rounded-lg p-2 outline-0 text-white" v-model="text" />
            <div class="my-2 mx-1">{{ text }} {{ count }}</div>
            <div class="bg-green-900 p-2 font-bold rounded-lg text-center" @click="go">Click me!</div>
            <a href="/toto">s</a>
        </div>
    </div>
</template>

<script setup lang="ts">
import { ref } from "vue";

const text = ref("Change me!");
const count = ref(0);

const go = () => {
    count.value++;
};
</script>
