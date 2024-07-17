<template>
    <div class="logo-container">
        <img srcset="/logo_1x.png 1x, /logo_2x.png 2x" alt="Google" height="92">
    </div>
</template>

<style scoped>
.logo-container {
    @apply flex flex-col items-center justify-end min-h-[92px] w-full max-h-[290px];
    height: calc(100% - 560px);
}
</style>
