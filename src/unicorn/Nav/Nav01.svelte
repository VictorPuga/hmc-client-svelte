<script>
  import { link } from "svelte-routing";
  export let icon = "img/other/logo.svg";
  export let buttons = [
    { title: "One", link: "/" },
    { title: "Two", link: "/" },
    { title: "Three", link: "/", outline: true }
  ];
  let open = false;
  function toggle() {
    open = !open;
    document.body.className = open ? "state-fixed-body" : "";
  }
</script>

<nav class="nav-01">
  <div class="container">
    <div class="nav-01__box">
      <div class="nav-01__logo">
        <a class="nav-01__link" href="/" use:link>
          <img class="nav-01__logo_img" src={icon} alt="Logo" />
        </a>
      </div>
      <div class="nav-01__links js-menu {open ? 'state-opened-menu' : ''}">
        <ul class="nav-01__list">
          {#each buttons as { title, link, outline }}
            <li class="nav-01__item">
              <a
                class="button button--white-outline {outline ? '' : 'button--empty'}"
                href={link}>
                <span>{title}</span>
              </a>
            </li>
          {/each}
        </ul>
        <div class="nav-01__burger">
          <button
            class="burger js-open-menu {open ? 'state-active-burger' : ''}"
            type="button"
            on:click={toggle}>
            <div class="burger__box">
              <div class="burger__inner" />
            </div>
          </button>
        </div>
      </div>
    </div>
  </div>
</nav>
