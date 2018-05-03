<template>
<ul>
<li v-for="n in 8" :key="n"><nuxt-link :to="'/sample0' + n"> Sample0{{n}}</nuxt-link></li>
</ul>
</template>

