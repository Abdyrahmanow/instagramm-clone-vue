<template>
  <div class="posts">
    <!-- Header -->
    <header class="header section">
      <div class="header-author">
        <Avatar size="40px" />
        <div class="header-author-info">
          <div>
            <CustomText tag="b">begli.a</CustomText>
          </div>
          <div>
            <CustomText size="xsmall">Montreal Quebec</CustomText>
          </div>
        </div>
      </div>
      <div class="header-more">
        <button type="button">
          <IconMore />
        </button>
      </div>
    </header>
    <!-- Media -->
    <div class="post-media">
      <img
        src="https://images.unsplash.com/photo-1494253109108-2e30c049369b?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&w=1000&q=80"
        alt=""
      />
    </div>
    <!-- Actions -->
    <div class="action-buttons section">
      <button type="button">
        <IconLike />
      </button>
      <button type="button">
        <IconComment />
      </button>
      <button type="button">
        <IconDirect />
      </button>
      <button class="action-save" type="button">
        <IconSave />
      </button>
    </div>
    <!-- View count -->
    <div class="view-count section">
      <CustomText tag="b">
        1.345 likes
      </CustomText>
    </div>
    <!-- Comment list -->
    <!-- Date Time -->
    <!-- Comment form -->
  </div>
</template>

<script>
import Avatar from '@/components/Avatar'
import CustomText from '@/components/CustomText'
import IconMore from '@/icons/more.svg'
import IconLike from '@/icons/like.svg'
import IconComment from '@/icons/comment.svg'
import IconDirect from '@/icons/direct.svg'
import IconSave from '@/icons/save.svg'
export default {
  components: {
    Avatar,
    CustomText,
    IconMore,
    IconLike,
    IconComment,
    IconDirect,
    IconSave
  }
}
</script>

<style lang="postcss" scoped>
.posts {
  border-radius: 3px;
  border: 1px solid rgb(var(--b6a));
}
.section {
  padding-left: 16px;
  padding-right: 16px;
}
.header {
  display: flex;
  align-items: center;
  height: 60px;

  &-author {
    display: flex;
    align-items: center;
    &-info {
      margin-left: 8px;
    }
  }
  &-more {
    margin-left: auto;
  }
}

.action-buttons {
  display: flex;
  align-items: center;
  height: 45px;

  button {
    margin-right: 16px;
  }
  .action-save {
    margin-left: auto;
    margin-right: 0;
  }
}
</style>
