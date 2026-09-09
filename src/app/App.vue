<script setup lang="ts">
import { RouterView } from 'vue-router'
import { DefaultLayout } from './layouts'

import { Notivue, NotivueSwipe, Notification } from 'notivue'
</script>

<template>
<Notivue v-slot="item">
  <NotivueSwipe :item="item">
    <Notification :item="item" />
  </NotivueSwipe>
</Notivue>

  <default-layout>
    <router-view />
  </default-layout>
</template>
