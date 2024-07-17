<script setup>
import { IconSearch, IconX } from '@tabler/icons-vue';
import { defineModel } from 'vue';

const model = defineModel({
    type: String,
    required: true
});

const emit = defineEmits(['onSubmit']);

function clearHandler() {
    model.value = '';
}

function submitHandler() {
    emit('onSubmit');
}
</script>

<template>
    <div class="flex w-full justify-center">
        <div class="parent-container">
            <IconSearch class="ml-4 mr-[13px] text-zinc-400" :size="18" />

            <input v-model="model" class="flex-grow" type="text" @keypress.enter="submitHandler" />

            <button v-if="model" title="Clear" @click="clearHandler">
                <IconX class="mx-3 text-zinc-400" :size="22" />
            </button>
        </div>
    </div>
</template>

<style scoped>
input {
    @apply bg-transparent h-full text-gray-200 focus:outline-none;
    font-size: 16px;
}

.parent-container {
    @apply border-[1px] flex flex-grow h-[48px] items-center max-w-[584px] mt-[6px] rounded-full;
    /* Close to border-gray-600 but not quite. */
    border-color: #5f6368;
}

.parent-container:hover {
    @apply shadow-lg;
    /* Close to zinc-800 but not quite. */
    background-color: #303134;
    border-color: #303134;
}
</style>
