<template>
  <button
    v-if="type === 'button'"
    :class="[
      'btn',
      {
        'btn--primary': color === 'primary',
        'btn--secondary': color === 'secondary',
        'btn--lightgray': color === 'lightgray',
      }
    ]"
  >
    <slot />
  </button>
  <router-link
    v-else
    :to="to"
    :class="[
      'btn',
      {
        'btn--primary': color === 'primary',
        'btn--secondary': color === 'secondary',
        'btn--lightgray': color === 'lightgray',
      }
    ]"
><slot/></router-link>
</template>

<script setup>
const props = defineProps({

  type: {
    type: String,
    default: "button",
  },
  to: {
    type: String,
    required: false,
  },
  color: {
    type: String,
    required:false,
  }
});
</script>

<style lang="scss" scoped>
.btn {
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
  &--primary{
    background: var(--purple);
    color: #fff;
  }
  &--secondary {
    background: rgba(118, 118, 118, 0.15);
    color: #fff;
  }
  &--lightgray{
    background: #c6b2a7;
    color: #fff;
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
