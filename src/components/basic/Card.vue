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
<div :class="'card card-' + props.type">
    <div class="card-icon" v-if="$slots.icon"><slot name="icon"></slot></div>
    <div class="card-title"><slot name="title"></slot></div>
    <div class="card-text"><slot name="text"></slot></div>
</div>
</template>

<style scoped>
.card {
    position: relative;
    width: 47.5%;
    margin-bottom: 44px;
    padding: 36px 30px 50px 30px;
    border-radius:  10px;
    border: 2px solid var(--gray-30);
}
.card-blue {
    background-color: var(--blue-500);
}

.card-blue::before {
    content: '';
    position: absolute;
    bottom: 0;
    right: 0;
    width: 136px;
    height: 203px;
    background-image: url('/src/assets/img/lines.png');
}
.card-icon {
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 60px;
    height: 60px;
    background-color: var(--blue-500);
    border-radius: 50%;
    color: var(--white);
}
.card-title {
    margin-top: 22px;
    font-size: 20px;
    color: var(--blue-600);
}
.card-blue .card-title {
    margin-top: 2px;
    font-size: 28px;
    line-height: 1.5;
    font-weight: 600;
    color: var(--white);
}
.card-text {
    margin-top: 12px;
    font-size: 14px;
    line-height: 2;
    font-weight: 400;
    color: var(--blue-300);
}
.card-blue .card-text {
    width: 370px;
    margin-top: 50px;
    font-size: 17px;
    line-height: 1.8;
    color: var(--gray-50);
}
</style>