<script>
  import { Nav01 } from "../";

  export let main = "Main";
  export let sub = "Sub";
  export let img = "";
  export let buttons = [
    { title: "Sign up", link: "/" },
    { title: "Learn more" }
  ];
  export let navProps = {};
  const [{ title: title1, link: link1 }, { title: title2 }] = buttons;
</script>

<header class="header-04 js-scroll-this-box">
  <div class="header-04__box" style="background-image: url({img})">
    <div class="header-04__overlay">
      <Nav01 {...navProps} />
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
                    href={link1}
                    target="_blank">
                    <span>{title1}</span>
                  </a>
                </li>
                <li class="buttons-set__item">
                  <button
                    class="button js-scroll-down button--white-bg "
                    type="button">
                    <span class="button__text"> {title2}</span>
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
                <li class="logos__item">
                  <img
                    class="logos__img"
                    src="img/logos/press/white/tech-crunch.svg"
                    alt="Tech Crunch logo"
                    height="25" />
                </li>
                <li class="logos__item">
                  <img
                    class="logos__img"
                    src="img/logos/press/white/forbes.svg"
                    alt="Forbes logo"
                    height="30" />
                </li>
                <li class="logos__item">
                  <img
                    class="logos__img"
                    src="img/logos/press/white/ycombinator.svg"
                    alt="YC logo"
                    height="30" />
                </li>
                <li class="logos__item">
                  <img
                    class="logos__img"
                    src="img/logos/press/white/lifehacker.svg"
                    alt="Lifehacker logo"
                    height="30" />
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</header>
