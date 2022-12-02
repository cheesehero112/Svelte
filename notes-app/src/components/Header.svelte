<script lang="ts">
  import logo from '@/assets/svelte.svg'

</script>

<header class="global-header">
  <div class="app-name">
    <img src={logo} alt="Svelte Logo" class="logo"/>
    <div class="title">Notes App</div>
  </div>
</header>

<style lang="scss">
:global(body) {
  /* this will apply to <body> */
  margin: 0;
  height: 100%;
  background-color: #fbfbfb;
}
  .global-header {
    background-color: #313131;
    height: 56px;
    color: white;
    padding: 15px;
    box-sizing: border-box;
    .app-name {
      display: flex;
      align-items: center;
      height: 100%;
      .logo {
        height: 100%;
        margin-right: 5px;
      }
      .title {
        font-weight: bold;
      }
    }
  }
</style>
