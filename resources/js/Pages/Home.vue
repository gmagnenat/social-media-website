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

    <div class="grid grid-cols-12 p-4 gap-4 h-screen">
        <div
            class="col-span-12 md:col-span-3 h-[500px] lg:h-full overflow-hidden"
        >
            <GroupList />
        </div>
        <div
            class="col-span-12 md:col-span-6 order-1 h-[500px] lg:h-full overflow-hidden flex flex-col"
        >
            <CreatePost />
            <PostList class="flex-1" />
        </div>
        <div
            class="col-span-12 md:col-span-3 order-3 h-[300px] lg:h-full overflow-hidden"
        >
            <FollowingList />
        </div>
    </div>
</template>

<style></style>
