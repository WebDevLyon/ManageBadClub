<template>
  <NuxtLink :to="route" class="nav-link">
    <font-awesome-icon
      :icon="fontawesomeIcon"
      :style="style"
      class="nav-link__icon"
    />{{ linkText }}
  </NuxtLink>
</template>

<script>
export default {
  data() {
    return {
      style: {
        color: this.colorIcon,
      },
    }
  },
  props: {
    linkText: { type: String, default: 'Link' },
    route: { type: String, default: '#' },
    fontawesomeIcon: {
      type: String,
      default: '',
    },
    colorIcon: {
      type: String,
      default: 'black',
    },
  },
}
</script>

<style lang="scss">
.nav-link {
  padding: 0.65rem 1.5rem;
  font-size: 1rem;
  line-height: 2.5rem;
  text-decoration: none;
  color: $dark;
  &__icon {
    font-size: 1.3rem;
    min-width: 2.25rem;
  }
  &:hover{
    color: red
  }
}
</style>
