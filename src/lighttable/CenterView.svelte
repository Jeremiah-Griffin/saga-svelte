<script type="module" lang="ts">
    import {MDCTextField} from '@material/textfield';

    const textField = new MDCTextField(document.querySelector('.mdc-text-field'));

     function printText(txt) {
         console.log(txt)
     }
</script>

<label class="mdc-text-field mdc-text-field--filled">
    <span class="mdc-text-field__ripple"></span>
    <span class="mdc-floating-label" id="my-label-id">Hint text</span>
    <input class="mdc-text-field__input" type="text" aria-labelledby="my-label-id">
    <span class="mdc-line-ripple"></span>
</label>


<style lang="scss">
  @use "@material/floating-label/mdc-floating-label";
  @use "@material/line-ripple/mdc-line-ripple";
  @use "@material/notched-outline/mdc-notched-outline";
  @use "@material/textfield";

  @include textfield.core-styles;
</style>