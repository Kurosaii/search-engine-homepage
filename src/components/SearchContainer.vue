<script setup>
import { ref } from 'vue';

import UIButton from './ui/UIButton.vue';
import UIInput from './ui/UIInput.vue';

const searchTerm = ref('');

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

function luckyHandler(index) {
    // In a production-ready version, this is where logic would go to navigate to different pages based on the index and the page associated with the phrase.
    console.log('In a production-ready version, this is where logic would go to navigate to different pages based on the index and the page associated with the phrase. index:', index);
}

function searchHandler() {
    if (!searchTerm.value) {
        return;
    }

    // In a production-ready version, this is where logic for go for navigating the user to the search page.
    console.log('In a production-ready version, this is where logic for go for navigating the user to the search page. searchTerm:', searchTerm.value);
}
</script>

<template>
    <div class="flex flex-col items-center p-5">
        <UIInput v-model="searchTerm" @onSubmit="searchHandler" />

        <div class="flex gap-1 pt-[18px]">
            <UIButton text="Google Search" @onClick="searchHandler" />
            <UIButton animate :secondaryText="randomSearchPhrases" text="I'm Feeling Lucky" @onClick="luckyHandler" />
        </div>
    </div>
</template>
