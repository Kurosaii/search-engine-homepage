<template>
    <div class="logo-container">
        <img srcset="/logo_1x.png 1x, /logo_2x.png 2x" alt="Google" height="92">
    </div>
</template>

<style scoped>
.logo-container {
    @apply flex flex-col items-center justify-end max-h-[290px] min-h-[92px] w-full;
    height: calc(100% - 560px);
}
</style>
