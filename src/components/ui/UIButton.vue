<script setup>
import { ref } from 'vue';

const props = defineProps({
    text: {
        type: String,
        required: true,
    },

    animate: {
        type: Boolean,
        default: false,
    },

    secondaryText: {
        type: Array,
        default: () => [],
    },
});

const secondaryIndex = ref(0);

const emit = defineEmits(['onClick']);

function clickHandler() {
    if (!props.animate) {
        emit('onClick');
    } else {
        emit('onClick', secondaryIndex.value);
    }
}

function focusHandler() {
    if (props.animate) {
        // In a production-ready version, this is where logic could be triggered to handle cycling through the props.secondaryText,
        // picking a random one, and leaving it displayed to the user.
        // This functionality can be seen by hovering over the "I'm Feeling Lucky" button, which brings you to various Google-specific pages when clicked.
        // The secondaryIndex ref would get updated to reflect which entry was selected so the parent could handle the interaction differently if needed.
    }
}
</script>

<template>
    <button :aria-label="props.text" @click="clickHandler" @focus="focusHandler">
        {{ props.text }}
    </button>
</template>

<style scoped>
button {
    @apply border-[1px] font-roboto h-9 mx-1 my-[11px] px-4 rounded text-gray-200;
    /* Close to zinc-800 but not quite.*/
    background-color: #303134;
    border-color: #303134;
}

button:hover {
    /* Close to zinc-600 but not quite.*/
    border-color: #5F6367;
}
</style>
