<script setup>
import { ref } from 'vue';
import FollowingItems from '@/Components/app/FollowingItems.vue';
import TextInput from '@/Components/TextInput.vue';

const searchKeyword = ref('');


</script>
<template>
    <div class="px-3 rounded border bg-white py-3 h-[400px]  lg:h-full overflow-hidden flex flex-col">

        <h4 class="text-xl font-bold mb-4">My Friends</h4>
        <TextInput :model-value="searchKeyword" placeholder="Friends Search" class="w-full"/>
        <div class="mt-3 flex-1  overflow-auto">
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
    </div>
</template>
<style>

</style>