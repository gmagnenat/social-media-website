<template>
    <h2 class="text-2xl font-bold py-2">Following</h2>
    <TextInput
        :model-value="searchKeyword"
        placeholder="Type to search"
        class="border-none w-full"
    />
    <div class="py-6">
        <div v-if="false" class="">You don't follow anyone yet</div>
        <div v-else class="flex flex-col gap-4">
            <FollowingItem
                image="https://randomuser.me/api/portraits/men/28.jpg"
                title="John Doe"
                description="Lorem ipsum dolor sit, amet consectetur
                                adipisicing elit. Facilis quasi nobis aperiam ab
                                ratione maiores, dolorum repellat cumque, culpa
                                dolorem consequuntur!"
            />
            <FollowingItem
                image="https://randomuser.me/api/portraits/women/18.jpg"
                title="Jane Doe"
                description="Lorem ipsum dolor sit, amet consectetur
                                adipisicing elit. Facilis quasi nobis aperiam ab
                                ratione maiores, dolorum repellat cumque, culpa
                                dolorem consequuntur!"
            />
        </div>
    </div>
</template>

<script setup>
import FollowingItem from "@/Components/app/FollowingItem.vue";
import TextInput from "@/Components/TextInput.vue";
</script>

<style lang="scss" scoped></style>
