<template>
  <h1 class="font-bold text-2xl">About {{ name }}</h1>
  <button @click="goToHome" class="underline">Home</button>
</template>

<script setup>
import { computed } from '@vue/reactivity';
import { useStore } from 'vuex';
import { useRouter } from 'vue-router';

const router = useRouter();

const goToHome = () => {
  router.push('/');
};

const store = useStore();
const name = computed(() => {
  return store.state.user.name;
});
</script>
