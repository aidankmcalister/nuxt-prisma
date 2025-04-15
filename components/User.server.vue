<script setup>
import prisma from "~/lib/prisma";
const user = await prisma.user.findFirst();
</script>

<template>
  <p>{{ user?.name ?? "No user has been added yet." }}</p>
</template>
