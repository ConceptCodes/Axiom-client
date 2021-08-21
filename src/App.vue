<template>
  <main id="app">
    <router-view/>
    <footer class="company-tag">Perspectives</footer>
  </main>
</template>

<style lang="scss">
  @import url('https://fonts.googleapis.com/css2?family=Inconsolata:wght@300;500;700&display=swap');
  body {
    height: 100vh !important;
    width: 100vw !important;
    overflow-y: hidden;
    font-family: 'Inconsolata', monospace;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    margin: 0px 0px 0px 0px;
  }
  #app {
      .company-tag {
        position: fixed;
        width: 100%;
        text-align: center;
        bottom: 20px;
        padding-top: 20px;
        font-style: normal;
        font-weight: 500;
        color: #A7A3A3;
      }
  }

</style>
