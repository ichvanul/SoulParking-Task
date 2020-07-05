<template>
  <div class="history">
    <CardOnPark/>
    <CardOnData/>
    <div class="wrap-history">
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
  },
  computed: {
    allMenu () {
      return this.$store.state.foodMenu
    }
  },
  methods: {
    select (id, index) {
      this.$store.commit('SELECT_MENU', id, index)
      this.showCart()
    },
    getItem () {
      const proto = {
        mutation: 'GET_ITEM',
        urlPath: 'menu'
      }
      this.$store.dispatch('getApi', proto)
    }
  },
  created () {
    this.getItem()
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
  .wrap-history {
    display: flex;
    flex-wrap: wrap;
  }
}
</style>
