<template>
  <div class="wrapper">
      <ListItem v-for="list in listsItem" :key="list" :list="list"/>
  </div>
</template>

<script>
import listsItem from '../testData.json'
import ListItem from '@/components/ListItem'
export default {
  name: 'App',
  components: {
    ListItem
  },
  data() {
    return {
      listsItem
    }
  },
}
</script>

<style>
  .wrapper {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }
</style>
