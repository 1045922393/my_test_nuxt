<template>
  <div>
    这是一个登录页面
    <div>选择登录账号</div>
    <ul>
      <li v-for="(item,index) in list" :key="index">
        姓名:{{item.name}} 年龄:{{item.age}}
      </li>
    </ul>
  </div>
</template>

<script>
/* eslint-disable no-console */
export default {
  async asyncData(app) {
    const { data } = await app.$axios.get(
      'http://myjson.dit.upm.es/api/bins/alsr'
    )
    return {
      list: data,
    }
  },
  data() {
    return {}
  },
}
</script>
