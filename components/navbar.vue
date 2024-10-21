<script setup lang="ts">
const links = [
  [
    {
      label: "Profile",
      avatar: {
        src: "https://avatars.githubusercontent.com/u/739984?v=4",
      },
      to: "/",
    },
    {
      label: "Habbits",
      icon: "i-heroicons-home",
      to: "/habbits",
    },
    {
      label: "Vertical Navigation",
      icon: "i-heroicons-chart-bar",
      to: "/components/vertical-navigation",
    },
    {
      label: "Command Palette",
      icon: "i-heroicons-command-line",
      to: "/components/command-palette",
    },
  ],
  [
    {
      label: "Examples",
      icon: "i-heroicons-light-bulb",
    },
    {
      label: "Help",
      icon: "i-heroicons-question-mark-circle",
    },
  ],
];
</script>

<template>
  <UVerticalNavigation :links="links">
    <template #default="{ link }">
      <span class="group-hover:text-primary relative">{{ link.label }}</span>
    </template>
  </UVerticalNavigation>
</template>
