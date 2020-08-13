<template>
  <div class="home">
    <div class="timeline">
      <h1>Home</h1>
      <CustomText>Salam</CustomText>
      <CustomText tag="p">Salam</CustomText>
      <CustomText tag="p" size="xsmall">Salam</CustomText>
      <CustomText tag="p" size="xxsmall">Salam</CustomText>
      <IconHome width="20" height="20" />

      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. At magni, nulla
        dignissimos aut suscipit minima ea deleniti praesentium qui optio vel
        dolorum perspiciatis, fugit dolorem sint ex veniam expedita quos.
        Aspernatur quam aperiam voluptatibus quidem. Temporibus impedit ducimus
        tempore molestias, numquam fugit, nobis qui quis magnam, ipsam quos
        quidem placeat accusamus corrupti laudantium laborum facilis praesentium
        autem repudiandae fugiat perspiciatis? Quasi dolorem suscipit assumenda
        quisquam, atque nihil alias vero esse, illum aut doloribus repellendus
        totam nam sit maiores facere magni perspiciatis ea recusandae sunt
        impedit eligendi cumque explicabo omnis. Voluptatibus.
      </p>

      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. At magni, nulla
        dignissimos aut suscipit minima ea deleniti praesentium qui optio vel
        dolorum perspiciatis, fugit dolorem sint ex veniam expedita quos.
        Aspernatur quam aperiam voluptatibus quidem. Temporibus impedit ducimus
        tempore molestias, numquam fugit, nobis qui quis magnam, ipsam quos
        quidem placeat accusamus corrupti laudantium laborum facilis praesentium
        autem repudiandae fugiat perspiciatis? Quasi dolorem suscipit assumenda
        quisquam, atque nihil alias vero esse, illum aut doloribus repellendus
        totam nam sit maiores facere magni perspiciatis ea recusandae sunt
        impedit eligendi cumque explicabo omnis. Voluptatibus.
      </p>

      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. At magni, nulla
        dignissimos aut suscipit minima ea deleniti praesentium qui optio vel
        dolorum perspiciatis, fugit dolorem sint ex veniam expedita quos.
        Aspernatur quam aperiam voluptatibus quidem. Temporibus impedit ducimus
        tempore molestias, numquam fugit, nobis qui quis magnam, ipsam quos
        quidem placeat accusamus corrupti laudantium laborum facilis praesentium
        autem repudiandae fugiat perspiciatis? Quasi dolorem suscipit assumenda
        quisquam, atque nihil alias vero esse, illum aut doloribus repellendus
        totam nam sit maiores facere magni perspiciatis ea recusandae sunt
        impedit eligendi cumque explicabo omnis. Voluptatibus.
      </p>

      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. At magni, nulla
        dignissimos aut suscipit minima ea deleniti praesentium qui optio vel
        dolorum perspiciatis, fugit dolorem sint ex veniam expedita quos.
        Aspernatur quam aperiam voluptatibus quidem. Temporibus impedit ducimus
        tempore molestias, numquam fugit, nobis qui quis magnam, ipsam quos
        quidem placeat accusamus corrupti laudantium laborum facilis praesentium
        autem repudiandae fugiat perspiciatis? Quasi dolorem suscipit assumenda
        quisquam, atque nihil alias vero esse, illum aut doloribus repellendus
        totam nam sit maiores facere magni perspiciatis ea recusandae sunt
        impedit eligendi cumque explicabo omnis. Voluptatibus.
      </p>
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
import CustomText from '@/components/CustomText'

export default {
  name: 'Home',
  components: {
    CustomText
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
