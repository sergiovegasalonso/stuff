<script setup lang="ts">
let darkThemeActivated: boolean = false
const toggleTheme = (): void => {
    const htmlElement : HTMLCollectionOf<HTMLHtmlElement> = document.getElementsByTagName('html')    
    if(darkThemeActivated)
        htmlElement[0].classList.remove('dark')
    else
        htmlElement[0].classList.add('dark')

    darkThemeActivated = !darkThemeActivated
}
</script>

<template>
    <button @click="toggleTheme()"></button>
</template>