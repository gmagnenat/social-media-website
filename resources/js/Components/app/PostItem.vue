<template>
    <div class="bg-gray-50 p-4 rounded-lg shadow-sm flex flex-col gap-4">
        <div class="flex gap-2 items-center">
            <a href="javascript:void(0)" class="">
                <img
                    :src="post.user.avatar"
                    alt=""
                    class="rounded-full w-[40px] hover:ring-offset-2 hover:ring-2 transition-all"
                />
            </a>
            <div class="flex flex-col">
                <h4 class="font-bold">
                    <a href="javascript:void(0)" class="hover:underline">{{
                        post.user.name
                    }}</a>
                    <template v-if="post.group">
                        >
                        <a href="javascript:void(0)" class="hover:underline">{{
                            post.group.name
                        }}</a>
                    </template>
                </h4>
                <small class="text-gray-400">{{ post.created_at }}</small>
            </div>
        </div>

        <div>
            <Disclosure v-slot="{ open }">
                <div v-if="!open" v-html="post.body.substring(0, 200)" />

                <DisclosurePanel class="">
                    <div v-html="post.body" />
                </DisclosurePanel>
                <div class="flex justify-end mb-3">
                    <DisclosureButton class="text-indigo-500">
                        <span class="hover:underline">{{
                            open ? "Read less" : "Read more"
                        }}</span>
                    </DisclosureButton>
                </div>
            </Disclosure>
        </div>

        <div class="grid grid-cols-2 lg:grid-cols-3 gap-4 md:gap-2">
            <div v-for="attachment of post.attachments" class="relative">
                <div
                    class="aspect-square bg-gray-100 flex flex-col justify-center items-center rounded-lg shadow text-gray-500 text-xs lg:text-sm"
                >
                    <button
                        class="bg-gray-800/40 w-8 h-8 absolute top-2 right-2 items-center justify-center flex flex-col rounded-full text-white hover:ring-offset-1 hover:ring-2 hover:ring-indigo-500 hover:bg-gray-100 hover:text-black transition-all"
                    >
                        <ArrowDownTrayIcon class="w-4 h-4 cursor-pointer" />
                    </button>

                    <img
                        v-if="isImage(attachment)"
                        class="rounded-md aspect-square w-full object-cover"
                        :src="attachment.url"
                        alt=""
                    />
                    <template v-else>
                        <DocumentIcon class="w-16 h-16" />
                        {{ attachment.name }}
                    </template>
                </div>
            </div>
        </div>

        <div class="flex gap-2 mt-4">
            <button
                class="text-gray-800 flex gap-1 items-center justify-center bg-gray-100 rounded-lg hover:bg-gray-200 py-2 px-4 flex-1"
            >
                <HandThumbUpIcon class="h-6" />
                Like
            </button>
            <button
                class="text-gray-800 flex gap-1 items-center justify-center bg-gray-100 rounded-lg hover:bg-gray-200 py-2 px-4 flex-1"
            >
                <ChatBubbleLeftRightIcon class="h-6" />
                Comment
            </button>
        </div>
    </div>
</template>

<script setup>
import { Disclosure, DisclosureButton, DisclosurePanel } from "@headlessui/vue";
import { DocumentIcon } from "@heroicons/vue/24/solid";
import { ArrowDownTrayIcon } from "@heroicons/vue/24/solid";
import { HandThumbUpIcon } from "@heroicons/vue/24/solid";
import { ChatBubbleLeftRightIcon } from "@heroicons/vue/24/solid";

defineProps({
    post: Object,
});

function isImage(attachment) {
    const mime = attachment.mime.split("/");
    return mime[0].toLowerCase() === "image";
}
</script>

<style lang="scss" scoped></style>
