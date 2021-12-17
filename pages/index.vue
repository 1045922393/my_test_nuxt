<template>
  <div>
    <!-- <Tutorial/> -->
    <NuxtLogo></NuxtLogo>
    <ul>
      <li><nuxt-link to="/">首页</nuxt-link></li>
      <li>
        <nuxt-link :to="{name: 'about',query:{layout: '3344'}, params: {id: '1104'}}">去介绍页面</nuxt-link>
      </li>
      <li>
        <nuxt-link :to="{name: 'myauth'}">去登录页面</nuxt-link>
      </li>
      <li>
        <nuxt-link :to="{name: 'paper'}">去论文页面</nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {}
</script>
