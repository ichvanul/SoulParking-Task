<template>
  <div class="home">
    <div class="wrap-menu">
      <h3>Dashboard</h3>
      <Card/>
    </div>
  </div>
</template>

<script>
import Card from '@/components/part/Card.vue'
import dom from '@/mixins/dom.vue'

export default {
  name: 'Home',
  mixins: [dom],
  components: {
    Card
  },
  computed: {
    allMenu () {
      return this.$store.state.foodMenu
    },
    allCategory () {
      return this.$store.state.foodCategory
    }
  },
  methods: {
    select (id, index) {
      this.$store.commit('SELECT_MENU', id)
      this.showCart()
      if (this.$store.state.selected.length > 0) return
      if (this.$store.state.selected.length === 0) this.hideCart()
    }
  }
}
</script>

<style lang="scss" scoped>
.home {
  margin: 55px 0 0 30px;
  padding: 15px;
  box-sizing: border-box;
  height: 90vh;
  overflow-y: scroll;
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
  .wrap-menu {
    display: flex;
    flex-wrap: wrap;
    h3 {
      margin-bottom: 20px;
      margin-left: 10px;
      font-weight: bolder;
      font-size: 25px;
    }
  }
}
.card {
  margin: 10px;
}
</style>
