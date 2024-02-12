<template>
     <TextInput :model-value="searchKeyword" placeholder="Group Search" class="w-full mt-4"/>
            <div class="mt-3 flex-1 overflow-auto">
                <div v-if="false" class="text-gray-400 text-center p-4">
                    You are not joined to any groups
                </div>
                <div v-else>

                        <GroupItems image="https://picsum.photos/200"
                                    title="Laravel Developer"
                                    description="Lorem ipsum dolor sit amet consectetur adipisicing elit."/>

                        <GroupItems image="https://picsum.photos/200"
                        title="PHP Developer"
                        description="Lorem ipsum dolor sit amet consectetur adipisicing elit."/>

                        <GroupItems image="https://picsum.photos/200"
                                    title="Laravel Developer"
                                    description="Lorem ipsum dolor sit amet consectetur adipisicing elit."/>

                        <GroupItems image="https://picsum.photos/200"
                        title="PHP Developer"
                        description="Lorem ipsum dolor sit amet consectetur adipisicing elit."/>

                        <GroupItems image="https://picsum.photos/200"
                                    title="Laravel Developer"
                                    description="Lorem ipsum dolor sit amet consectetur adipisicing elit."/>

                        <GroupItems image="https://picsum.photos/200"
                        title="PHP Developer"
                        description="Lorem ipsum dolor sit amet consectetur adipisicing elit."/>

                    

                
                </div>
            </div>
</template>

<script setup>
import { ref } from 'vue';
import GroupItems from '@/Components/app/GroupItems.vue'
import TextInput from '@/Components/TextInput.vue';

const searchKeyword = ref('');

</script>

<style lang="scss" scoped>

</style>