<script lang="ts">
    import { Input } from '@smui/textfield';
    import Paper from '@smui/paper';
    import Fab from '@smui/fab';
    import { Icon } from '@smui/common';


    let queryText = "";

     function printText(txt) {
         console.log(txt)
     }
</script>
<div>
    <Paper class="solo-paper" elevation={6}>
        <Icon class="material-icons">search</Icon>
        <Input
                bind:queryText
                placeholder="Search"
                class="solo-input"
        />
    </Paper>
    <Fab
            on:click={printText(queryText)}
            disabled={queryText === ''}
            color="primary"
            mini
            class="solo-fab"
    >
        <Icon class="material-icons">arrow_forward</Icon>
    </Fab>
</div>

