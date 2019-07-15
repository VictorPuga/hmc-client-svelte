<script>
  const { type: _t, onEnter: _o, value: _v, ...props } = $$props;
  export let onEnter = function(val) {};
  export let value = "";

  function keypress(e) {
    if (e.keyCode == 13) {
      onEnter(value);
    }
  }
</script>

<style lang="scss">
  input {
    width: 100%;
    border-radius: 4px;
    padding: 0 20px;
    height: 44px;
    background-color: var(--input_bg);
    border: 2px solid var(--input-border);
    color: var(--input_color);
    font-size: 14px;
    transition: border-color 0.2s ease, background-color 0.2s ease;
    &::-webkit-input-placeholder {
      opacity: 0.5;
      font-size: inherit;
      color: inherit;
      transition: opacity 0.2s ease, transform 0.2s ease;
    }
    &:-moz-placeholder {
      opacity: 0.5;
      font-size: inherit;
      color: inherit;
      transition: opacity 0.2s ease, transform 0.2s ease;
    }
    &::-moz-placeholder {
      opacity: 0.5;
      font-size: inherit;
      color: inherit;
      transition: opacity 0.2s ease, transform 0.2s ease;
    }
    &:-ms-input-placeholder {
      opacity: 0.5;
      font-size: inherit;
      color: inherit;
      transition: opacity 0.2s ease, transform 0.2s ease;
    }
    &:hover {
      border-color: var(--input-border_hover);
    }
    &:focus {
      border-color: var(--black-hard);
      background-color: var(--input_focus);
      &::-webkit-input-placeholder {
        opacity: 0;
        transform: translateX(10px);
      }
      &:-moz-placeholder {
        opacity: 0;
        transform: translateX(10px);
      }
      &::-moz-placeholder {
        opacity: 0;
        transform: translateX(10px);
      }
      &:-ms-input-placeholder {
        opacity: 0;
        transform: translateX(10px);
      }
    }
  }
</style>

<input {...props} bind:value on:keypress={keypress} type="text" />
