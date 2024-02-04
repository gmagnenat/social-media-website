<template>
    <div class="">
        <div class="flex gap-2 items-center">
            <img :src="image" class="rounded-full w-[40px]" alt="" />
            <div>
                <h3 class="">{{ title }}</h3>
            </div>
        </div>
    </div>
</template>

<script setup>
defineProps({
    image: String,
    title: String,
});
</script>

<style lang="scss" scoped></style>
