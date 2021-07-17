<template>
  <div class="container">
    <span class="filetype">Matlab files</span>
    <select v-model="selected" class="list">
      <option v-for="item in List" :value="item" :key="'matlab' + item">
        {{item}}
      </option>
    </select>
    <a :href="'/Matlab/order' + selected + '_.mat'" @click="download">
      <button class="download">
        Download
      </button>
    </a>
  </div>
</template>

<script>
  import List from '../assets/List'

  export default {
    name: 'Matlab',
    data () {
      return {
        List: List,
        selected: '1'
      }
    }
  }
</script>

<style>
  .filetype {
    font-size: 1em;
    font-weight: bold;
  }
  .list {
    margin-left: 1em;
    margin-right: 1em;
  }
  .download {
    background: white;
    width: 7em;
    box-shadow: inset 0 0 0 0 black;
    transition: ease 0.5s;
  }
  .download:hover {
    box-shadow: inset 7em 0 0 0 black;
    color: white;
    cursor: pointer;
  }
</style>