<template>
  <nav>
    <NuxtLink to="#wires">Провода</NuxtLink>
    <NuxtLink to="#button">Кнопка</NuxtLink>
    <NuxtLink to="#keyboard">Клавиатура</NuxtLink>
  </nav>
  <article>
    <slot />
  </article>
</template>

<style>
body {
  margin: 0;
  font-family: "RoobertPRO", "RoobertPRO override", sans-serif;
}

nav {
  background: #00dc82;
  position: sticky;
  top: 0;
  padding: 20px 0;
  z-index: 10;

  & a {
    margin-right: 12px;
    padding: 20px;
    color: #fff;

    &:hover {
      background: #36e4da;
    }
  }
}

article {
  padding: 0 20px;
}

section {
  scroll-margin-top: 4rem;
}

table {
  border: 1px solid #000;
  border-collapse: collapse;
  margin-top: 12px;
  margin-bottom: 12px;
  max-width: 100%;
  width: 100%;

  & td {
    border: 1px solid #000;
    padding: 6px 12px;

    & img {
      width: 100%;
    }
  }
}

ul {
  padding-inline-start: 14px;
}

ol {
  padding-inline-start: 16px;
}

ol li {
  margin-bottom: 8px;
}
</style>