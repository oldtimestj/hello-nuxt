<template>
  <div>
    <h2>商品列表</h2>
    <ul>
      <li v-for="item of list" :key="item.name">
        <nuxt-link :to="'/detail/' + item.id">{{item.name}}</nuxt-link>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  data() {
    return {
      list: [
        { id: '009', name:'iphone', price: 100 },
        { id: '008', name: 'huawei', price: 1000 },
        { id: '007', name: 'xiaomi', price: 800 },
      ],
    }
  },
}
</script>
