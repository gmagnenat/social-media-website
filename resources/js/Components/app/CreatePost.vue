<template>
    <div class="bg-gray-50 p-4 rounded-lg shadow-sm flex flex-col gap-4">
        <div @click="postCreating = true" class="py-4 px-4 rounded-lg border">
            <p>Click here to create a new post</p>
        </div>
        <div v-if="postCreating" class="flex justify-between">
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
    </div>
</template>

<script setup>
import { ref } from "vue";

const postCreating = ref(false);
</script>

<style lang="scss" scoped></style>
