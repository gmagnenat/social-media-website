<template>
    <div class="flex gap-2 items-center">
        <a href="javascript:void(0)">
            <img :src="post.user.avatar" alt="" class="rounded-full w-[40px]" />
        </a>
        <div class="flex flex-col">
            <a href="javascript:void(0)" class="">
                <h4 class="font-bold">{{ post.user.name }}</h4>
            </a>
            <small class="text-gray-400">{{ post.created_at }}</small>
        </div>
    </div>
    <div>
        <Disclosure v-slot="{ open }">
            <div v-if="!open" v-html="post.body.substring(0, 200)" />

            <DisclosurePanel class="">
                <div v-html="post.body" />
            </DisclosurePanel>
            <div class="flex justify-end">
                <DisclosureButton class="text-indigo-500">
                    <span>{{ open ? "Read less" : "Read more" }}</span>
                </DisclosureButton>
            </div>
        </Disclosure>
    </div>
</template>

<script setup>
import { Disclosure, DisclosureButton, DisclosurePanel } from "@headlessui/vue";
defineProps({
    post: Object,
});
</script>

<style lang="scss" scoped></style>
