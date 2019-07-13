<script>
  const _logo = {
    img: "img/logos/press/white/lifehacker.svg",
    name: "Lifehacker",
    height: 50
  };
  export let main = "Main";
  export let sub = "Sub";
  export let img = "";
  export let buttons = [
    { title: "Sign up", href: "/" },
    { title: "Learn more" }
  ];
  // const [{ title: title1, href: href1 }, { title: title2 }] = buttons;
  export let logos = [_logo, _logo, _logo];
</script>

<style>
  header {
    background-color: var(--header_bg);
  }
</style>

<header class="header-04 js-scroll-this-box">
  <div class="header-04__box" style="background-image: url({img})">
    <div class="header-04__overlay">
      <div class="container container--mid header-04__container">
        <div class="header-04__card header-04__card--top">
          <div class="header-04__card_content">
            <h1 class="heading heading--accent header-04__heading white-text">
               {main}
            </h1>
            <p class="header-04__text white-text">
              {@html sub}
            </p>
            <div class="header-04__buttons buttons-set">
              <ul class="buttons-set__list">
                <li class="buttons-set__item">
                  <a
                    class="button button--alt-accent-bg "
                    href={buttons[0].href}
                    target="_blank">
                    <span>{buttons[0].title}</span>
                  </a>
                </li>
                <li class="buttons-set__item">
                  <button
                    class="button js-scroll-down button--white-bg "
                    type="button">
                    <span class="button__text">{buttons[1].title}</span>
                    <!-- TODO: Implement scroll down -->
                  </button>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div class="container">
          <div class="header-04__logos">
            <div class="logos">
              <ul class="logos__list">
                {#each logos as { img, name, height }}
                  <li class="logos__item">
                    <img
                      class="logos__img"
                      src={img}
                      alt={name}
                      {height}
                      draggable="false"
                      style="padding: 5px;" />
                  </li>
                {/each}
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</header>
