<script lang="ts">
    import { Input } from '@smui/textfield';
    import { Icon } from '@smui/common';
    import Paper from '@smui/paper';
    import Fab from '@smui/fab';


    let queryText = "";

     function printText(txt: string) {
         console.log(txt)
     }
</script>

<div class="solo-container">
    <Paper class="solo-paper" elevation={6}>
        <Icon class="material-icons">search</Icon>
        <Input
                bind:queryText
                placeholder="Search"
                class="solo-input"
        />
    </Paper>
    <Fab
            on:click={() => printText(queryText)}
            disabled={queryText === ''}
            color="primary"
            mini
            class="solo-fab"
    >
        <Icon class="material-icons">arrow_forward</Icon>
    </Fab>
</div>

<style>
  .solo-container {
    display: flex;
    justify-content: center;
    align-items: center;
  }
  * :global(.solo-paper) {
    display: flex;
    align-items: center;
    flex-grow: 1;
    max-width: 600px;
    margin: 0 12px;
    padding: 0 12px;
    height: 48px;
  }
  * :global(.solo-paper > *) {
    display: inline-block;
    margin: 0 12px;
  }
  * :global(.solo-input) {
    flex-grow: 1;
    color: var(--mdc-theme-on-surface, #000);
  }
  * :global(.solo-input::placeholder) {
    color: var(--mdc-theme-on-surface, #000);
    opacity: 0.6;
  }
  * :global(.solo-fab) {
    flex-shrink: 0;
  }
</style>