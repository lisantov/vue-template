<template>
  <div class="flex w-full items-center gap-12">
    <h1 class="text-[180px] font-medium">
      404
    </h1>
    <div class="flex flex-col gap-4">
      <span class="text-2xl">Кажется, вы заблудились</span>
      <app-button @click.stop="router.push('/')">
        На главную
      </app-button>
    </div>
  </div>
</template>

<script lang="ts" setup>
import { AppButton } from '@/shared/ui';
import { useRouter } from 'vue-router';

const router = useRouter()
</script>
