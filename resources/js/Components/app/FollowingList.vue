<template>
    <div
        class="rounded-lg shadow-sm py-3 h-full overflow-hidden flex flex-col bg-gray-50 px-4"
    >
        <div class="flex-1 block md:hidden">
            <Disclosure v-slot="{ open }">
                <DisclosureButton>
                    <h2 class="text-2xl font-bold py-2">Following</h2>
                </DisclosureButton>
                <DisclosurePanel>
                    <TextInput
                        :model-value="searchKeyword"
                        placeholder="Type to search"
                        class="w-full border-none"
                    />
                    <div class="mt-4 h-[300px] overflow-auto">
                        <div v-if="false" class="text-center text-gray-400 p-3">
                            You don't follow anyone yet
                        </div>
                        <div
                            v-else
                            class="flex flex-col gap-4 lg:h-full h-[300px] overflow-scroll"
                        >
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
                </DisclosurePanel>
            </Disclosure>
        </div>
        <div class="hidden md:block">
            <h2 class="text-2xl font-bold py-2">Following</h2>
            <TextInput
                :model-value="searchKeyword"
                placeholder="Type to search"
                class="border-none w-full"
            />
            <div class="mt-4 h-[300px] overflow-auto">
                <div v-if="false" class="text-center text-gray-400 p-3">
                    You don't follow anyone yet
                </div>
                <div
                    v-else
                    class="flex flex-col gap-4 lg:h-full h-[300px] overflow-scroll"
                >
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
        </div>
    </div>
</template>

<script setup>
import FollowingItem from "@/Components/app/FollowingItem.vue";
import TextInput from "@/Components/TextInput.vue";
import { Disclosure, DisclosureButton, DisclosurePanel } from "@headlessui/vue";
</script>

<style lang="scss" scoped></style>
