<template>
    <div class="history">
      <CardOnPark/>
      <div class="wrap-history">
        <CardOnData/>
      </div>
    </div>
</template>

<script>
import CardOnPark from '../components/part/CardOnPark'
import CardOnData from '../components/part/CardOnData'
import dom from '@/mixins/dom.vue'

export default {
  name: 'Gaskir',
  mixins: [dom],
  components: {
    CardOnPark,
    CardOnData
  }
}
</script>

<style lang="scss" scoped>
.history {
  margin: 54px 0 0 60px;
  padding: 15px;
  box-sizing: border-box;
  height: 90vh;
  overflow-y: scroll;
  display: flex;
  &::-webkit-scrollbar {
    width: 5px;
  }
  &::-webkit-scrollbar-thumb {
    background-color: #dbdbdb;
    border-radius: 10px;
  }
  &::-webkit-scrollbar-track {
    background-color: transparent;
    border-radius: 10px;
  }
  .wrap-history {
    display: flex;
    flex-wrap: wrap;
  }
}
</style>
