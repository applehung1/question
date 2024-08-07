<template>
    <div></div>
</template>

<script>
import axios from 'axios'
export default {
  created () {
    console.log(this.$route.params)
    const seed = 'b55ceec3d9d429c2'
    axios.get(`https://randomuser.me/api/?seed=${seed}`)
      .then((res) => {
        console.log(res)
      })
  }
}
</script>
