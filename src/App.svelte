<script type="module" lang="ts">
  import AppBar from './utils/AppBar.svelte'
  import CenterView from "./lighttable/CenterView.svelte";
</script>

<main>
  <div class="appbar"><AppBar/></div>
  <div class="grid-container">
    <div class="centerv"><CenterView/></div>
  </div>
</main>

<style lang="scss">
  .flex-container{
    display: flex;
    flex-direction: row;
    justify-content: center;
    gap: 50px;
  }

  .grid-container{
    display: grid;
    grid-template-areas:
    'appbar appbar appbar appbar appbar'
    'menul centerv centerv centerv menur'
  }
  .appbar {grid-area: appbar}
  .menul {grid-area: menul}
  .centerv {grid-area: centerv}
  .menur{grid-area: menur}
</style>
