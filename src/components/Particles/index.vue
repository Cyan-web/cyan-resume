<template>
    <div
        id="particles-js"
        class="w-[500px] h-[500px]"
    />
</template>

<script lang="ts" setup>
import 'particles.js'
import config from './particles.json'

// eslint-disable-next-line no-undef
particlesJS.load('particles-js', config)
</script>

<style scoped></style>
