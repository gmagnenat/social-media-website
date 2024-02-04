<template>
    <div class="w-full border-b pb-2">
        <div class="">
            <img
                :src="image"
                class="w-full object-cover h-40 rounded-md"
                alt=""
            />
            <div>
                <h3 class="font-bold py-2">{{ title }}</h3>
                <div class="">{{ description }}</div>
            </div>
        </div>
    </div>
</template>

<script setup>
defineProps({
    image: String,
    title: String,
    description: String,
});
</script>

<style lang="scss" scoped></style>
