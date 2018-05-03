<template>
<ul>
<li><button @click="gotoRandom"> Random </button></li>
<li v-for="n in 8" :key="n"><nuxt-link :to="'/sample0' + n"> Sample0{{n}}</nuxt-link></li>
</ul>
</template>
<script>
export default {
  methods: {
      gotoRandom(){
          //this.$router.push('/sample01')
          //this.$router.replace('/sample01')
          this.$router.go(-1)
      }
  }
}
</script>

