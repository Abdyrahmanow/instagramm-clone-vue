<template>
  <div class="home">
    <h1>Home</h1>
    <CustomText>Salam</CustomText>
    <CustomText tag="p">Salam</CustomText>
    <CustomText tag="p" size="xsmall">Salam</CustomText>
    <CustomText tag="p" size="xxsmall">Salam</CustomText>
    <IconHome width="20" height="20" />
  </div>
</template>

<script>
import CustomText from '@/components/CustomText'

export default {
  name: 'Home',
  components: {
    CustomText
  }
}
</script>

<style scoped>
h1 {
  color: red;

  @media (--t) {
    color: blue;
  }
}
</style>
