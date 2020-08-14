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
        <router-link to="/profile">
          <Avatar size="26px" />
        </router-link>
      </nav>
    </Container>
  </header>
</template>

<script>
import Container from '@/components/Container'
import Avatar from '@/components/Avatar'

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
    Avatar,
    IconHome,
    IconHomeFill,
    IconDirect,
    IconDirectFill,
    Explore,
    ExploreFill
  }
}
</script>

<style lang="postcss" scoped>
.header {
  z-index: 90;
  position: fixed;
  left: 0;
  right: 0;
  top: 0;
  background-color: #fff;
  border-bottom: 1px solid rgb(var(--b6a));
}
.header-inner {
  height: var(--header-height);
  display: flex;
  align-items: center;
  justify-content: center;

  @media (--t) {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    align-items: center;
  }
}
.logo {
  font-size: 1.6rem;
  font-weight: bold;
}
.search {
  display: none;
  @media (--t) {
    display: block;
    text-align: center;

    input {
      width: 215px;
      height: 28px;
      border: 1px solid rgb(var(--b6a));
      background-color: rgba(var(--b3f));
      border-radius: 4px;
      padding-left: 20px;
      padding-right: 20px;
      padding-bottom: 2px;
    }
  }
}
.navigation {
  z-index: 90;
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #fff;
  border-top: 1px solid rgb(var(--b6a));
  height: 70px;
  display: flex;
  align-items: center;
  justify-content: space-around;

  @media (--t) {
    height: auto;
    position: static;
    justify-content: flex-end;
    border: 0;

    a {
      margin-left: 20px;
    }
  }
}
</style>
