<script setup>
const props = defineProps({
  total: {
    type: Number,
    required: true,
  },
});
</script>

<template>
  <h4>Your Balance</h4>
  <h1 id="balance" class="money" :class="{ plus: total > 0, minus: total < 0 }">${{ total }}</h1>
</template>
