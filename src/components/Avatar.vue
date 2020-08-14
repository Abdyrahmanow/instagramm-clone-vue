<template>
  <figure class="avatar">
    <img :src="src" :alt="alt" :width="size" :height="size" />
  </figure>
</template>

<script>
export default {
  name: 'Avatar',
  props: {
    src: {
      type: String,
      default:
        'http://drupalace.ru/sites/default/files/styles/medium/public/vk.png?itok=tHWgTfxf'
    },
    alt: {
      type: String
    },
    size: Number
  }
}
</script>

<style lang="postcss" scoped>
.avatar {
  padding: 2px;
  display: inline-flex;
  border-radius: 50%;
  background-color: red;
  img {
    border-radius: inherit;
    border: 2px solid white;
  }
}
</style>
