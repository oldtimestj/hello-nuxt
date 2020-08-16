<template>
  <div>
    <h2>详情页</h2>
    {{$route.params.id}}
    <p>{{detail.price}}</p>
    <p>{{detail.description}}</p>
  </div>
</template>
<script>
  import axios from 'axios';
  export default {
    async asyncData() {
     const res = await axios.get('/data/test.json');
     console.log('res', res)
      return {
          detail: res.data,
        }
    }
  }
</script>

