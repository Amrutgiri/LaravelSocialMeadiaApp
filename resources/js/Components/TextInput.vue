<script setup>
import { onMounted, ref } from 'vue';

const model = defineModel({
    type: String,
    required: true,
});

const input = ref(null);

onMounted(() => {
    if (input.value.hasAttribute('autofocus')) {
        input.value.focus();
    }
});

defineExpose({ 
    focus: () => input.value.focus()
     });

defineProps({
    placeholder:String
})
</script>

<template>
    <input
        class="rounded-md shadow-sm"
        v-model="model"
        ref="input"
        :placeholder="placeholder"
    />
</template>
