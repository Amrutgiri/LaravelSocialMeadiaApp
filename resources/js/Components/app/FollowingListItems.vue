<script setup>
import { ref } from 'vue';
import FollowingItems from '@/Components/app/FollowingItems.vue';
import TextInput from '@/Components/TextInput.vue';

const searchKeyword = ref('');
</script>

<template>
<TextInput :model-value="searchKeyword" placeholder="Friends Search" class="w-full mt-4"/>
        <div class="mt-3 h-[200px] lg:flex-1 overflow-auto">
            <div v-if="false" class="text-gray-400 text-center p-4">
                You don't have a friends yet.
            </div>
            <div v-else>

                    <FollowingItems image="https://picsum.photos/200"
                                title="Elon Musk"
                                />

                    <FollowingItems image="https://picsum.photos/200"
                    title="Gautam Adani"
                    />

                    <FollowingItems image="https://picsum.photos/200"
                                title="Elon Musk"
                                />

                    <FollowingItems image="https://picsum.photos/200"
                    title="Gautam Adani"
                    />

                    <FollowingItems image="https://picsum.photos/200"
                                title="Elon Musk"
                                />

                    <FollowingItems image="https://picsum.photos/200"
                    title="Gautam Adani"
                    />

                    <FollowingItems image="https://picsum.photos/200"
                                title="Elon Musk"
                                />

                    <FollowingItems image="https://picsum.photos/200"
                    title="Gautam Adani"
                    />

               
            </div>
        </div>
</template>


<style lang="scss" scoped>

</style>