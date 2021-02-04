<template>
  <div>成语接龙</div>
</template>

<script lang="ts">
import Vue from 'vue'
import { MetaInfo } from 'vue-meta/types'

export default Vue.extend({
  async asyncData(params) {
    console.log(params)
    console.log(process, process.server)
    // ;(params.app.head as MetaInfo).title = '123'
    return { title: process.title }
  },
})
</script>
