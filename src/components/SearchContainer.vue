<script setup>
import UIButton from './ui/UIButton.vue';

const randomSearchPhrases = [
    "I'm Feeling Curious",
    "I'm Feeling Hungry",
    "I'm Feeling Adventurous",
    "I'm Feeling Playful",
    "I'm Feeling Stellar",
    "I'm Feeling Doodley",
    "I'm Feeling Trendy",
    "I'm Feeling Artistic",
    "I'm Feeling Funny",
];
</script>

<template>
    <div class="flex flex-col items-center p-5">
        <div class="h-[54px]" />

        <div class="flex pt-[18px] gap-1">
            <UIButton text="Google Search" />
            <UIButton text="I'm Feeling Lucky" animate :secondaryText=randomSearchPhrases />
        </div>
    </div>
</template>

<style scoped></style>