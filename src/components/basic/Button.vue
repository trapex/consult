<script setup>
import { defineProps } from 'vue';

const props = defineProps({
  type: {
    type: String,
    default: 'white',
    validator: (value) => ['white', 'blue'].includes(value),
  },
});

</script>

<template>
  <button :class="'button button-' + props.type">
    <span class="icon" v-if="$slots.icon"><slot name="icon"></slot></span>
    <slot></slot>
  </button>
</template>

<style scoped>
.button {
    display: flex;
    align-items: center;
    padding: 10px 50px;
    border-radius: 5px;
    font-size: 16px;
}
.button-white {
    color: var(--blue-500);
    border: 2px solid var(--gray-30);
}
.button-blue {
    background-color: var(--blue-500);
    color: var(--white);
}
.icon {
    margin-top: 5px;
    margin-right: 5px;
}
</style>