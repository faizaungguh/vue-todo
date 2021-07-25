<template>
  <div>Title</div>
  <slot :data="title"/>
  <div>Content</div>
  <slot :data="content" />
  <div>Footer</div>
  <slot :data="footer"/>
</template>

<script>
export default {
  data() {
    return {
      title: 'ini title',
      content: 'ini content',
      footer: 'ini footer'
    }
  },
};
</script>
