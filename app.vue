<template>
  <div id="app">
    <NuxtLayout>
      <NuxtPage />
    </NuxtLayout>
  </div>
</template>

<style>
:root.light {
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
  --theme-primary: #f34c84;
  --theme-secondary: #c297dc;
  --theme-surface: #2f2b2b;
  --theme-background: #1b1919;
  --theme-on-primary: #443e42;
  --theme-on-secondary: #000;
  --theme-on-surface: #f5f1f1;
}
</style>
