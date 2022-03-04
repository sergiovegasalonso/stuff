<template>
  <div id="app">
    <NuxtLayout>
      <NuxtPage />
    </NuxtLayout>
  </div>
</template>

<style>
:root {
  --theme-primary-lighter: #ff8b6d;
  --theme-primary-light: #ed6440;
  --theme-primary: #da3e15;
  --theme-primary-dark: #af2a07;
  --theme-primary-darker: #871c00;
  --theme-secondary: #9b4dca;
  --theme-surface: #fff;
  --theme-background: #fafafa;
  --theme-on-primary: #fff;
  --theme-on-secondary: #fff;
  --theme-on-surface: #000;
}

:root.dark {
  --theme-primary-lighter: #ff8b6d;
  --theme-primary-light: #ed6440;
  --theme-primary: #da3e15;
  --theme-primary-dark: #af2a07;
  --theme-primary-darker: #871c00;
  --theme-secondary: #9b4dca;
  --theme-surface: #fff;
  --theme-background: #333333;
  --theme-on-primary: #fff;
  --theme-on-secondary: #fff;
  --theme-on-surface: #000;
}

* {
  box-sizing: border-box;
}

html,
body {
  margin: 0;
}

#app {
  background-color: var(--theme-background);
  min-height: 100vh;
}
</style>
