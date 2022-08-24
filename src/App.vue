<script setup>
const count = $ref(0);

const addCount = () => {
  count++;
};
const removeCount = () => {
  count--;
};
const resetCount = () => {
  count = 0;
};
</script>

<template>
  <h1>カウントアプリ</h1>
  <p>{{ count }}</p>
  <button type="button" @click="addCount">+</button>
  <button type="button" @click="removeCount">-</button>
  <button type="button" @click="resetCount">リセット</button>
</template>
