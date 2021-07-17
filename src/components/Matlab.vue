<template>
  <div class="container">
    <!-- <a href="/Matlab/order1000_.mat" download>test</a> -->
    <select v-model="selected">
      <option v-for="item in List" :value="item" :key="'matlab' + item">
        {{item}}
      </option>
    </select>
    <span>{{selected}}</span>
    <a :href="'/Matlab/order' + selected + '_.mat'" @click="download">Download</a>
  </div>
</template>

<script>
  import List from '../assets/List'

  export default {
    name: 'Matlab',
    data () {
      return {
        List: List,
        selected: ''
      }
    }
  }
</script>