<script setup>

import { defineProps } from 'vue';

const props = defineProps({
   num: {
    type: String,
    default: '00',
  },
  type: {
    type: String,
    default: 'right',
    validator: (value) => ['right', 'left'].includes(value),
  },
  title: {
    type: String,
    default: '',
  },
  text: {
    type: String,
    default: '',
  }
});

</script>

<template>
<div :class="'step step-' + props.type">
    <div class="step-wrap">
        <div class="step-num"> {{ num }} </div>
        <div class="step-content">
            <div class="step-icon" v-if="$slots.icon"><slot name="icon"></slot></div>
            <div class="step-title"> {{ title }} </div>
            <div class="step-text"> {{ text }} </div>
        </div>
    </div>
</div>
</template>

<style scoped>
.step {
    display: flex;
    margin-bottom: 42px;
}
.step-right {
    justify-content: flex-end;
}
.step-right .step-num {
    margin: 45px 40px 0 5px;
}
.step-left .step-num {
    order: 2;
    margin: 45px 5px 0 40px;
}
.step-left .step-content {
    order: 1;
}
.step-left .step-wrap {
    justify-content: flex-end;
}
.step-left .step-icon {
    display: flex;
    justify-content: flex-end;
}
.step-left .step-title,
.step-left .step-text {
    text-align: right;
}
.step-wrap {
    width: calc(45% + 99px); /* 99px = step-num's (width + margin) */
    display: flex;
}
.step-num {
    position: relative;
    display: flex;
    justify-content: space-around;
    align-items: center;
    min-width: 60px;
    height: 40px;
    background-color: var(--blue-500);
    border-radius: 50px;
    color: var(--white);
    font-weight: 900;
}
.step:nth-of-type(1) .step-num::before {
    content: '';
    position: absolute;
    width: 4px;
    height: 534px;
    top: 20px;
    left: 50%;
    margin-left: -2px;
    background-image: url('/src/assets/img/step-line.png');
    z-index: -1;
}
.step-content {
    max-width: 330px;
}
.step-icon {
}
.step-title {
    position: relative;
    background-color: var(--white);
    color: var(--blue-600);
    font-size: 20px;
    font-weight: 600;
}
.step-text {
    position: relative;
    background-color: var(--white);
    margin-top: 10px;
    line-height: 1.8;
    color: var(--blue-300);
    font-size: 14px;
    font-weight: 400;
}
</style>