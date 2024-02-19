<template>
    <div
        class="px-3 bg-gray-50 rounded shadow-sm py-3 overflow-hidden flex flex-col"
    >
        <div class="flex-1 block md:hidden">
            <Disclosure v-slot="{ open }">
                <DisclosureButton class="text-left">
                    <h2 class="text-2xl font-bold py-2">My Groups</h2>
                </DisclosureButton>
                <DisclosurePanel>
                    <TextInput
                        :model-value="searchKeyword"
                        placeholder="Type to search"
                        class="w-full border-none"
                    />
                    <div class="mt-4 h-[300px] overflow-auto">
                        <div v-if="false" class="text-center text-gray-300 p-3">
                            You haven't joined any groups
                        </div>
                        <div v-else class="flex flex-col gap-4 overflow-scroll">
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
                </DisclosurePanel>
                <div class="flex justify-end"></div>
            </Disclosure>
        </div>
        <div class="hidden md:block">
            <h2 class="text-2xl font-bold py-2">My Groups</h2>
            <TextInput
                :model-value="searchKeyword"
                placeholder="Type to search"
                class="w-full"
            />
            <div class="mt-4 h-[300px] overflow-auto">
                <div v-if="false" class="text-center text-gray-300 p-3">
                    You haven't joined any groups
                </div>
                <div v-else class="flex flex-col gap-4 overflow-scroll">
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
        </div>
    </div>
</template>

<script setup>
import GroupItem from "@/Components/app/GroupItem.vue";
import TextInput from "@/Components/TextInput.vue";
import { Disclosure, DisclosureButton, DisclosurePanel } from "@headlessui/vue";
</script>

<style lang="scss" scoped></style>
