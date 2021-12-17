<template>
  <div>
    <h2>
      这是一个介绍页面
    </h2>
    <h3>{{$route.params.id}}</h3>
    <ul>
      <li v-for="(item,idx) in list" :key="item.id">
        <h5>序号({{idx}})</h5>
        <div>
          <span>姓名:</span> <span>{{item.name}}</span>
        </div>
        <div>
          <span>年龄:</span> <span>{{item.age}}</span>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data(){
    return {
      list: []
    }
  }
  // async asyncData(){
  //   const {data} = await 
  // }
}
</script>

<style>
h2 {
  color: palevioletred;
}
</style>