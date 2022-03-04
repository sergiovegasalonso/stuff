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
    <div id="theme-switcher" class="wrapper" @click="toggleTheme()">
    <div class="rail">
        <div class="switch"></div>
    </div>
    </div>
</template>

<style scoped>
.wrapper {
    width: 2.25rem;
    height: 1rem;
}
.rail {
    width: 2.25rem;
    height: 1rem;
    background-color: red;
    border-radius: 1rem;
}

.switch {
    position: absolute;
    height: 1.50rem;
    width: 1.50rem;    
    background: black;
    border-radius: 100%;
    top: -25%;
}
</style>