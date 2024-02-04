<template>
    <div
        @click="postCreating = true"
        class="border border-gray-100 bg-white py-4 px-4 rounded-lg mb-4 shadow-sm"
    >
        <p>Click here to create a new post</p>
    </div>
    <div v-if="postCreating" class="flex justify-between mb-4">
        <button
            type="submit"
            class="rounded-md bg-indigo-600 px-3 py-2 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600 relative"
        >
            Attach a file
            <input
                type="file"
                class="absolute left-0 top-0 right-0 bottom-0 opacity-0"
            />
        </button>
        <button
            type="submit"
            class="rounded-md bg-indigo-600 px-3 py-2 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600 relative"
        >
            Submit
        </button>
    </div>
</template>

<script setup>
import { ref } from "vue";

const postCreating = ref(false);
</script>

<style lang="scss" scoped></style>
