<script setup>
import { ref } from "vue";

const postCreating = ref(false);

</script>

<template>
    <div class="p-4  border bg-white mb-3 rounded-lg">
        <div @click="postCreating=true" class="py-3 px-2 text-gray-400 border border-2 border-gray-200 rounded mb-3">
            Click here to add new post
        </div>
        <div v-if="postCreating" class="flex justify-between ">
            <button type="submit" class="rounded-md bg-indigo-600 px-3 py-2 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600 relative">Attech File
                <input class="absolute right-0 left-0 top-0 bottom-0 opacity-0" type="file" >
            </button>
            <button type="submit" class="rounded-md bg-indigo-600 px-3 py-2 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">Save</button>
        </div>
    </div>
</template>

<style scoped>

</style>