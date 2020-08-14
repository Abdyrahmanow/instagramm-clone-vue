<template>
  <div class="home">
    <div class="timeline">
      <h1>Home</h1>
      <br />
      <br />
      <br />
      <Posts />
      <br />
      <br />
      <br />
      <br />
      <br />
    </div>

    <div class="sidebar">
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Excepturi
        possimus, porro aperiam illo mollitia, similique doloremque nesciunt
        laborum hic ratione fugit. Laboriosam dolores dicta in consectetur ad
        nemo magnam earum?Sapiente quas natus perspiciatis recusandae ullam
        obcaecati autem suscipit laudantium? Voluptate, consequuntur harum
        distinctio earum porro modi possimus recusandae in reiciendis, nulla
        illo non officiis eius! Vitae nobis odit tempore!
      </p>
    </div>
  </div>
</template>

<script>
import Posts from '@/components/Posts'
export default {
  name: 'Home',
  components: {
    Posts
  }
}
</script>

<style scoped>
.home {
  max-width: 605px;
  margin-left: auto;
  margin-right: auto;

  @media (--t) {
    max-width: none;
    display: grid;
    grid-template-columns: 1fr 295px;
    grid-gap: 30px;
  }
}
.sidebar {
  display: none;

  @media (--t) {
    display: block;
  }
}
</style>
