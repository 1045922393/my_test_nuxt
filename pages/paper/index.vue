<template>
  <div>
    <h2>page of paper</h2>
    <ul>
      <li>
        <nuxt-link :to="{path: '/paper/00412412', params:{id: 999444234}}">turn to 444234</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/paper/111154">turn to 111154</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/paper/335466">turn to 335466</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/paper/fdafadfsf">turn to fdasf</nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>
/* eslint-disable no-console */
export default {
  transition: 'paper',
}
</script>
