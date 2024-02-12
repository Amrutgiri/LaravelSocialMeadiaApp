<script setup>

import { Disclosure, DisclosureButton, DisclosurePanel } from '@headlessui/vue';
import GroupListItems from '@/Components/app/GroupListItems.vue';


</script>
<template>
    <div class="px-3 bg-white rounded border py-3   lg:h-full overflow-hidden">
        <div class=" block lg:hidden">
            <Disclosure v-slot="{ open }">
            <DisclosureButton class="w-full">
                <div class="flex justify-between items-center">
                    <h4 class="text-xl font-bold ">My Groups</h4>
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="w-6 h-6 transition-all" :class="open ? 'rotate-90 transform':''">
                        <path fill-rule="evenodd" d="M13.28 11.47a.75.75 0 0 1 0 1.06l-7.5 7.5a.75.75 0 0 1-1.06-1.06L11.69 12 4.72 5.03a.75.75 0 0 1 1.06-1.06l7.5 7.5Z" clip-rule="evenodd" />
                        <path fill-rule="evenodd" d="M19.28 11.47a.75.75 0 0 1 0 1.06l-7.5 7.5a.75.75 0 1 1-1.06-1.06L17.69 12l-6.97-6.97a.75.75 0 0 1 1.06-1.06l7.5 7.5Z" clip-rule="evenodd" />
                    </svg>
                </div>
                </DisclosureButton>
            <DisclosurePanel >
                <GroupListItems/>
            </DisclosurePanel>
        </Disclosure>
        </div>
       <div class="h-full flex-col overflow-hidden hidden lg:flex">
            <h4 class="text-xl font-bold">My Groups</h4>
           <GroupListItems/>
       </div>
    </div>
</template>
<style>

</style>