<template>
  <div class="home">
    <CustomText tag="h1">Profile </CustomText>

    <div id="nav">
      <router-link to="/profile/posts">Profile Posts</router-link> |
      <router-link to="/profile/igtv">Profile IGTV</router-link> |
      <router-link to="/profile/save">Profile Save</router-link> |
      <router-link to="/profile/tag">Profile Tag</router-link>
    </div>
    <router-view />
  </div>
</template>

<script>
import CustomText from '@/components/CustomText'

export default {
  name: 'Profile',
  components: {
    CustomText
  }
}
</script>

<style scoped></style>
