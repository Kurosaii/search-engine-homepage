<template>
    <div class="parent-container">
        <div class="flex min-w-[30%] order-1">
            <a href="#">Advertising</a>
            <a href="#">Business</a>
            <a href="#">How Search works</a>
        </div>
        <div class="middle-container">
            <a href="#" class="flex items-center">
                <img class="h-3.5 mr-1.5" src="/leaf.png" />
                <span>Our third decade of climate action: join us</span>
            </a>
        </div>
        <div class="flex min-w-[30%] justify-end order-3">
            <a href="#">Privacy</a>
            <a href="#">Terms</a>
            <a href="#">Settings</a>
        </div>
    </div>
</template>

<style scoped>
a {
    @apply text-gray-200 whitespace-nowrap p-[15px] hover:underline no-underline;
    line-height: normal;
}

.parent-container {
    @apply bg-neutral-900 px-5 flex flex-wrap justify-between;
}

.middle-container {
    @apply flex order-2;
}

@media only screen and (max-width: 1200px) {
    .parent-container {
        @apply justify-evenly;
    }

    .middle-container {
        @apply order-none w-full justify-center;
    }
}
</style>
