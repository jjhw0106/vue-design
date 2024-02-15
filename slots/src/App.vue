<template>
  <div>
    <item-view>
      <template #item-one>{{ items }}</template>
      <template #item-two>{{ items2 }}</template>
    </item-view>
  </div>
</template>

<script>
import ItemView from './components/Item.vue';
export default {
  components: {
    ItemView,
  },
  data() {
    return {
      items: ['아이템 1','아이템 2','아이템 3','아이템 4','아이템 5'],
      items2: ['뉘리리1', '뉘리리 2'],
    }
  }
}
</script>

<style>

</style>