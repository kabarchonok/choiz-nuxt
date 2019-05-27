<template>
  <div class="index">
    <Header></Header>
    <div class="wrapper">
      <div class="content">
        <feed></feed>
      </div>
      <top50></top50>
    </div>
  </div>
</template>

<script>
import Header from '~/components/Header.vue'
import Top50 from '~/components/Top50.vue'
import Feed from '~/components/Feed.vue'

export default {
  components: {
    Header,
    Top50,
    Feed
  }
}
</script>

<style>
.index {
  max-width: 1440px;
  margin: auto;
  padding-top: 65px;
}
.wrapper {
  display: flex;
}
.index,
.wrapper {
  height: 100%;
}
</style>
