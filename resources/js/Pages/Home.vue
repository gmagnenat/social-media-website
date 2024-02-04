<script setup>
import { Head, Link } from "@inertiajs/vue3";
import GroupList from "@/Components/app/GroupList.vue";
import CreatePost from "@/Components/app/CreatePost.vue";
import PostList from "@/Components/app/PostList.vue";
import TextInput from "@/Components/TextInput.vue";
import FollowingList from "@/Components/app/FollowingList.vue";

defineProps({});
</script>

<template>
    <Head title="Social Media Website" />

    <div class="grid grid-cols-12 p-4 gap-4">
        <div
            class="col-span-12 md:col-span-3 bg-gray-50 rounded-lg p-4 shadow-sm order-2 md:order-1"
        >
            <GroupList />
        </div>
        <div
            class="col-span-12 md:col-span-6 bg-gray-50 rounded-lg p-4 shadow-sm order-1"
        >
            <CreatePost />
            <PostList />
        </div>
        <div
            class="col-span-12 md:col-span-3 bg-gray-50 rounded-lg p-4 shadow-sm order-3"
        >
            <FollowingList />
        </div>
    </div>
</template>

<style></style>
