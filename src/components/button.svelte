<script>
  export let title = "Button";
  export let variant = "light";
  const { title: _t, variant: _v, ...props } = $$props;
</script>

<style>
  button {
    overflow: hidden;
    display: inline-block;
    position: relative;
    padding: 12px 20px;
    min-width: 120px;
    border: 2px solid transparent;
    min-height: 44px;
    border-radius: 4px;
    box-shadow: 0 2px 4px 0 rgba(136, 144, 195, 0.2),
      0 5px 15px 0 rgba(37, 44, 97, 0.15);
    font-size: 14px;
    font-weight: 700;
    -webkit-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    user-select: none;
    text-align: center;
    text-decoration: none;
    cursor: pointer;
    transition: color 0.2s ease, background-color 0.2s ease,
      border-color 0.2s ease, box-shadow 0.2s ease, transform 0.2s ease;
  }
  button[disabled] {
    cursor: default;
  }
  button:hover,
  button:focus {
    transform: translateY(-2px);
    box-shadow: 0 2px 8px 0 rgba(136, 144, 195, 0.22),
      0 8px 15px 0 rgba(37, 44, 97, 0.17);
  }
  button:active {
    transform: translateY(-1px);
    box-shadow: 0 2px 4px 0 rgba(136, 144, 195, 0.2),
      0 5px 15px 0 rgba(37, 44, 97, 0.15);
    outline: none;
  }

  .light {
    background-color: var(--button-secondary_bg);
    color: var(--button-secondary_color);
  }
  .primary {
    background-color: var(--button-primary_bg);
    color: var(--button-primary_color);
  }
  .primary:hover,
  .primary:focus {
    background-color: var(--button-primary_hover);
  }
  .ghost {
    background-color: transparent;
    border-color: var(--white);
    color: var(--white);
  }
  .dark {
    background-color: var(--button-secondary_color);
    color: var(--button-secondary_bg);
  }
</style>

<!-- TODO: forward more events -->
<button class={variant} on:click {...props}>{title}</button>
