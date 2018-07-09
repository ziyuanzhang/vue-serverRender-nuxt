<template>
  <h1 class="c-999">Hello {{ name }}!</h1>
</template>

<script>
export default {
  asyncData (context) {
    // called every time before loading the component
    return { name: 'World' }
  },
  layout: 'blog'
}
</script>