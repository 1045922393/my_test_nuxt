<template>
  <div>
    <h3>{{$route.params.id}}</h3>
  </div>
</template>

<script>
/* eslint-disable no-console */
export default {
  layout: 'paperLayout',
  validate(all) {
    // if (all.params.id === '111154') {
    //   return true
    // } else {
    //   // return new Error('页面丢失')
    //   throw new Error('错误自定义')
    // }
    return /^[0-9]+$/.test(all.params.id)
  },
  transition: 'paper',
  // validate(all) {
  //   console.log(all, 'outside')
  //   return new Promise((resolve, reject) => {
  //     console.log(all, 'insert')
  //     setTimeout(() => {
  //       if(all.params.id === '111154') {
  //         resolve(true)
  //       } else {
  //         resolve(false)
  //         // reject(new Error('页面丢失~'))
  //       }
  //     }, 1500)
  //   })
  // },
  watch: {
    $route(newVal, oldVal) {
      console.log(newVal, oldVal)
    },
  },
  mounted() {
    console.log(this.$route)
  },
}
</script>