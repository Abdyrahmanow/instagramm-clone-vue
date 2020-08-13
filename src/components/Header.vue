<template>
  <header class="header">
    <Container class="header-inner">
      <router-link to="/" class="logo">
        Instagram
      </router-link>

      <form class="search">
        <input type="text" placeholder="Search" />
      </form>

      <nav class="navigation">
        <router-link to="/">
          <IconHomeFill v-if="$route.name === 'Home'" />
          <IconHome v-else />
        </router-link>

        <router-link to="/direct">
          <IconDirectFill v-if="$route.name === 'Direct'" />
          <IconDirect v-else />
        </router-link>

        <router-link to="/explore">
          <ExploreFill v-if="$route.name === 'Explore'" />
          <Explore v-else />
        </router-link>
        <router-link to="/profile">Profile</router-link>
      </nav>
    </Container>
  </header>
</template>

<script>
import Container from '@/components/Container'
import IconHome from '@/icons/home.svg'
import IconHomeFill from '@/icons/home-fill.svg'
import IconDirect from '@/icons/direct.svg'
import IconDirectFill from '@/icons/direct-fill.svg'
import Explore from '@/icons/explore.svg'
import ExploreFill from '@/icons/explore-fill.svg'

export default {
  name: 'MainHeader',
  components: {
    Container,
    IconHome,
    IconHomeFill,
    IconDirect,
    IconDirectFill,
    Explore,
    ExploreFill
  }
}
</script>

<style scoped>
.header {
  border-bottom: 1px solid rgb(var(--b6a));
}
.header-inner {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  align-items: center;
  height: 60px;
}
.logo {
  font-size: 1.6rem;
  font-weight: bold;
}
.search {
  text-align: center;
}
.search input {
  width: 215px;
  height: 28px;
  border: 1px solid rgb(var(--b6a));
  background-color: rgba(var(--b3f));
  border-radius: 4px;
  padding-left: 20px;
  padding-right: 20px;
}
.navigation {
  display: flex;
  justify-content: flex-end;
  align-items: center;
}
.navigation a {
  margin-left: 20px;
}
</style>
