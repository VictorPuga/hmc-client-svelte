<script>
  import { link } from "svelte-routing";
  import { Button } from "../../components";
  export let icon = "img/other/logo.svg";
  export let buttons = [
    { title: "One", href: "/" },
    { title: "Two", href: "/" },
    { title: "Three", href: "/" }
  ];
</script>

<nav class="nav-01">
  <div class="container">
    <div class="nav-01__box">
      <div class="nav-01__logo">
        <a class="nav-01__link" href="/" use:link>
          <img class="nav-01__logo_img" src={icon} alt="Logo" />
        </a>
      </div>
      <div class="nav-01__links js-menu">
        <ul class="nav-01__list">
          {#each buttons as button}
            <li class="nav-01__item">
              <Button variant="nav" {...button} />
            </li>
          {/each}
        </ul>
        <div class="nav-01__burger">
          <button class="burger js-open-menu" type="button">
            <div class="burger__box">
              <div class="burger__inner" />
            </div>
          </button>
        </div>
      </div>
    </div>
  </div>
</nav>
