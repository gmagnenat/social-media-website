<template>
    <h2 class="text-2xl font-bold py-2">My Groups</h2>
    <TextInput
        :model-value="searchKeyword"
        placeholder="Type to search"
        class="w-full border-none"
    />
    <div class="py-6">
        <div v-if="false" class="">You haven't joined any groups</div>
        <div v-else class="flex flex-col gap-4">
            <GroupItem
                image="https://picsum.photos/200"
                title="Laravel Developer"
                description="Lorem ipsum dolor sit, amet consectetur
                                adipisicing elit. Facilis quasi nobis aperiam ab
                                ratione maiores, dolorum repellat cumque, culpa
                                dolorem consequuntur!"
            />
            <GroupItem
                image="https://picsum.photos/200"
                title="Vue.js Developer"
                description="Lorem ipsum dolor sit, amet consectetur
                                adipisicing elit. Facilis quasi nobis aperiam ab
                                ratione maiores, dolorum repellat cumque, culpa
                                dolorem consequuntur!"
            />
        </div>
    </div>
</template>

<script setup>
import GroupItem from "@/Components/app/GroupItem.vue";
import TextInput from "@/Components/TextInput.vue";
</script>

<style lang="scss" scoped></style>
