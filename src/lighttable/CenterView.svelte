<script lang="ts">
    import {
        textField
    } from "material-components-web/index.d.ts";

    const PrintText = () => {
        const queryText = new textField.MDCTextField(document.querySelector('.queryBar')).value;
        console.log(queryText);
    }
</script>

<label class="mdc-text-field queryBar">
    <span class="mdc-text-field__ripple"></span>
    <span class="mdc-floating-label" id="my-label-id">Enter query...</span>
    <input class="mdc-text-field__input" type="text" aria-labelledby="my-label-id">
    <span class="mdc-line-ripple"></span>
</label>

<style lang="scss">
  @use '@material/textfield';
    .queryBar{
        @include textfield.core-styles(   );
    }
</style>
