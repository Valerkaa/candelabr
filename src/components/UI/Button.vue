<template>
  <button
    v-if="type === 'button'"
    :style="{ backgroundColor: background }"
    class="btn"
  >
    <slot />
  </button>
  <router-link
    v-else
    :to="to"
    class="btn"
    :style="{ backgroundColor: background }"
    ><slot
  /></router-link>
</template>

<script setup>
const props = defineProps({
  background: {
    type: String,
    required: false,
  },
  type: {
    type: String,
    default: "button",
  },
  to: {
    type: String,
    required: false,
  },
  colorBtn: {
    type: String,
    default: "#000",
  },
});
</script>

<style lang="scss" scoped>
.btn {
  background: var(--puprle);
  color: #fff;
  padding: 0 32px;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  font-size: 16px;
  cursor: pointer;
  width: 170px;
  height: 56px;
  text-decoration: none;
  &:hover {
    opacity: 0.8;
  }
  //   text-decoration: none;
  //   width: 170px;
  //   height: 56px;
  //   display: flex;
  //   align-items: center;
  //   justify-content: center;
  //   background: rgba(118, 118, 118, 0.15);
  //   cursor: pointer;

  //   &:hover {
  //     background: rgba(118, 118, 118, 0.2);
  //   }
}
</style>
