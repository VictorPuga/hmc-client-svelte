<script>
  import { link } from "svelte-routing";
  export let title = "Button";
  export let variant = "light";
  export let href = "";
  const { title: _t, variant: _v, href: _h, ...props } = $$props;
</script>

<style lang="scss">
  button,
  a {
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

    &:hover,
    &:focus {
      transform: translateY(-2px);
      box-shadow: 0 2px 8px 0 rgba(136, 144, 195, 0.22),
        0 8px 15px 0 rgba(37, 44, 97, 0.17);
    }

    &:active {
      transform: translateY(-1px);
      box-shadow: 0 2px 4px 0 rgba(136, 144, 195, 0.2),
        0 5px 15px 0 rgba(37, 44, 97, 0.15);
      outline: none;
    }

    &.light {
      background-color: var(--button-secondary_bg);
      color: var(--button-secondary_color);
    }

    &.primary {
      background-color: var(--button-primary_bg);
      color: var(--button-primary_color);
      &:hover,
      &:focus {
        background-color: var(--button-primary_hover);
      }
    }

    &.outline {
      background-color: transparent;
      border-color: var(--general-text-01);
      color: var(--general-text-01);
    }

    &.ghost {
      box-shadow: none;
      color: var(--general-text-01);
      &:hover,
      &:focus {
        box-shadow: none;
        background-color: var(--button-ghost_hover);
      }
    }

    /* .nav buttons are always white */
    &.nav {
      box-shadow: none;
      color: var(--white);
      &:hover,
      &:focus {
        box-shadow: none;
        background-color: rgba(255, 255, 255, 0.1);
      }
    }

    &[disabled] {
      cursor: default;
      opacity: 0.4;
      &:hover {
        transform: none;
      }
    }
  }
</style>

<!-- TODO: forward more events -->
{#if !href}
  <button class={variant} on:click {...props}>{title}</button>
{:else if href.includes('#')}
  <a {href} class={variant} {...props} use:link>{title}</a>
{:else}
  <a {href} class={variant} {...props}>{title}</a>
{/if}
