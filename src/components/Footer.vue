<template>
  <div class="footer">
    <div class="container">
      <a class="repo" href="https://github.com/TsungLinYeh/a-golay-hadamard-unitary" target="_blank">
          check on github
      </a>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'Footer'
  }
</script>

<style>
  .footer {
    position: absolute;
    display: flex;
    bottom: 0;
    height: 5vh;
    width: 100vw;
    background: black;
    justify-content: center;
  }
  .container {
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .repo {
    font-size: 0.5em;
    color: white;
    text-decoration: none;
  }
</style>