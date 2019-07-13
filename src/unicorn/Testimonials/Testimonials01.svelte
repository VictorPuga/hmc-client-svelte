<script>
  const _testimonial = {
    text: "Hey".repeat(10),
    author: "John",
    sub: "Sub",
    img: ""
  };
  export let main = "Main";
  export let sub = "Sub";
  export let testimonials = [_testimonial, _testimonial, _testimonial];
  function handle(e) {
    // console.log("d");
  }
</script>

<!-- 
<div class="testimonials-01">
  <div class="container container--small">
    <div class="title-box title-box--center">
      <h2 class="heading">{main}</h2>
      <p class="title-box__text">{sub}</p>
    </div>
  </div>
  <div class="testimonials-01__container container">
    <div class="slider">
      <div class="slider__arrow slider__arrow--prev">
        <button
          class="circle-button js-prev-arrow circle-button--icon
          circle-button--light-blue-bg slick-arrow"
          type="button"
          style="">
          <span class="icon">
            <svg
              width="24"
              height="17"
              viewBox="0 0 24 17"
              xmlns="http://www.w3.org/2000/svg">
              <g id="styleguide" fill="none" fill-rule="evenodd">
                <g
                  id="Unicorn-Styleguide"
                  transform="translate(-121 -2006)"
                  fill-rule="nonzero"
                  fill="#00396B">
                  <g id="Icons" transform="translate(55 1963)">
                    <g
                      id="arrow-pointing-to-right"
                      transform="translate(66 43)">
                      <path
                        d="M23.673 7.688L16.531.336a1.094 1.094 0 0 0-1.578 0
                        1.173 1.173 0 0 0 0 1.625l5.237 5.39H1.116C.5 7.351 0
                        7.866 0 8.5s.5 1.149 1.116 1.149H20.19l-5.237 5.39a1.173
                        1.173 0 0 0 0 1.625 1.097 1.097 0 0 0 1.578
                        0l7.142-7.352a1.173 1.173 0 0 0 0-1.624z"
                        id="Shape"
                        transform="matrix(-1 0 0 1 24 0)" />
                    </g>
                  </g>
                </g>
              </g>
            </svg>
          </span>
        </button>
      </div>
      <div class="slider__arrow slider__arrow--next">
        <button
          class="circle-button js-next-arrow circle-button--icon
          circle-button--light-blue-bg slick-arrow"
          type="button"
          style="">
          <span class="icon">
            <svg viewBox="0 0 13 10" xmlns="http://www.w3.org/2000/svg">
              <path
                d="M12.823 4.164L8.954.182a.592.592 0 0 0-.854 0 .635.635 0 0 0
                0 .88l2.836 2.92H.604A.614.614 0 0 0 0 4.604c0
                .344.27.622.604.622h10.332L8.1 8.146a.635.635 0 0 0 0
                .88.594.594 0 0 0 .854 0l3.869-3.982a.635.635 0 0 0 0-.88z"
                fill-rule="nonzero"
                fill="#00396B" />
            </svg>
          </span>
        </button>
      </div>
      <ul
        class="slider__box js-slider slick-initialized slick-slider slick-dotted"
        data-slider-config={{ dots: true, infinite: true, speed: 300, fade: false, cssEase: 'ease', adaptiveHeight: false, lazyLoad: 'ondemand' }}>
        <div
          id="slick-list"
          class="slick-list draggable"
          draggable=true
          on:drag|preventDefault={handle}
>
          <div
            class="slick-track"
            style="opacity: 1; width: 7112px; transform: translate3d(-1016px,
            0px, 0px);">
            {#each testimonials as { text, author, sub, img }}
              <li
                class="slider__item slick-slide slick-cloned"
                data-slick-index="-1"
                aria-hidden="true"
                tabindex="-1"
                style="width: 1016px;">
                <div class="testimonials-01__item">
                  <img
                    class="testimonials-01__logo testimonials-01__logo--round"
                    src="https://unicornplatform.com/app/img/photos/team-2/via-talen-de-st-croix.jpg"
                    alt="" />
                  <p class="testimonials-01__text">{text}</p>
                  <div class="testimonials-01__author">
                     {author}
                    <br />
                    Frontend developer-freelancer
                  </div>
                </div>
              </li>
            {/each}
          </div>
        </div>

        <ul class="slick-dots" role="tablist" style="">
          <li class="slick-active" role="presentation">
            <button
              type="button"
              role="tab"
              id="slick-slide-control00"
              aria-controls="slick-slide00"
              aria-label="1 of 3"
              tabindex="0"
              aria-selected="true">
              1
            </button>
          </li>
          <li role="presentation">
            <button
              type="button"
              role="tab"
              id="slick-slide-control01"
              aria-controls="slick-slide01"
              aria-label="2 of 3"
              tabindex="-1">
              2
            </button>
          </li>
          <li role="presentation">
            <button
              type="button"
              role="tab"
              id="slick-slide-control02"
              aria-controls="slick-slide02"
              aria-label="3 of 3"
              tabindex="-1">
              3
            </button>
          </li>
        </ul>
      </ul>
    </div>
  </div>
</div> -->

<div class="testimonials-01">
  <div class="container container--small">
    <div class="title-box title-box--center">
      <h2 class="heading">Nuestros Patrocinadores</h2>
      <p class="title-box__text">
        Sin ellos Hacker Mafia sería solo una idea en la mente de todos
        nosotros.
      </p>
    </div>
  </div>
  <div class="testimonials-01__container container">
    <div class="slider">
      <div class="slider__arrow slider__arrow--prev">
        <button
          class="circle-button js-prev-arrow circle-button--icon
          circle-button--light-blue-bg"
          type="button">
          <span class="icon">
            <svg
              width="24"
              height="17"
              viewBox="0 0 24 17"
              xmlns="http://www.w3.org/2000/svg">
              <g id="styleguide" fill="none" fill-rule="evenodd">
                <g
                  id="Unicorn-Styleguide"
                  transform="translate(-121 -2006)"
                  fill-rule="nonzero"
                  fill="#00396B">
                  <g id="Icons" transform="translate(55 1963)">
                    <g
                      id="arrow-pointing-to-right"
                      transform="translate(66 43)">
                      <path
                        d="M23.673 7.688L16.531.336a1.094 1.094 0 0 0-1.578 0
                        1.173 1.173 0 0 0 0 1.625l5.237 5.39H1.116C.5 7.351 0
                        7.866 0 8.5s.5 1.149 1.116 1.149H20.19l-5.237 5.39a1.173
                        1.173 0 0 0 0 1.625 1.097 1.097 0 0 0 1.578
                        0l7.142-7.352a1.173 1.173 0 0 0 0-1.624z"
                        id="Shape"
                        transform="matrix(-1 0 0 1 24 0)" />
                    </g>
                  </g>
                </g>
              </g>
            </svg>
          </span>
        </button>
      </div>
      <div class="slider__arrow slider__arrow--next">
        <button
          class="circle-button js-next-arrow circle-button--icon
          circle-button--light-blue-bg"
          type="button">
          <span class="icon">
            <svg viewBox="0 0 13 10" xmlns="http://www.w3.org/2000/svg">
              <path
                d="M12.823 4.164L8.954.182a.592.592 0 0 0-.854 0 .635.635 0 0 0
                0 .88l2.836 2.92H.604A.614.614 0 0 0 0 4.604c0
                .344.27.622.604.622h10.332L8.1 8.146a.635.635 0 0 0 0
                .88.594.594 0 0 0 .854 0l3.869-3.982a.635.635 0 0 0 0-.88z"
                fill-rule="nonzero"
                fill="#00396B" />
            </svg>
          </span>
        </button>
      </div>
      <ul
        class="slider__box js-slider"
        data-slider-config={JSON.stringify({
          dots: true,
          infinite: true,
          speed: 300,
          fade: false,
          cssEase: 'ease',
          adaptiveHeight: false,
          lazyLoad: 'ondemand'
        })}>
        <li class="slider__item">
          <div class="testimonials-01__item">
            <img
              class="testimonials-01__logo"
              src="img/logos/companies/intercom.svg" />
            <p class="testimonials-01__text">
              "Lotus nixs ducunt ad domina. A falsis, orgia festus castor. Sunt
              brodiumes convertam superbus, fortis galataees. Pol, historia!
              Nobilis sagas ducunt ad sectam. Eheu. Nunquam quaestio medicina.
              Acipensers ire! Cur era messis? Cum accentor velum, omnes
              demolitionees experientia talis, neuter finises. Lotus brabeuta
              callide anhelares messor est."
            </p>
            <div class="testimonials-01__author">
              John Allen
              <br />
              Co-founder & CMO
            </div>
          </div>
        </li>
        <li class="slider__item">
          <div class="testimonials-01__item">
            <img
              class="testimonials-01__logo"
              src="img/logos/companies/instacart.svg" />
            <p class="testimonials-01__text">
              "Hippotoxotas crescere! Burgus de flavum omnia, quaestio mons!
              Audax accentor unus experientias xiphias est. A falsis, rumor
              lotus finis. Ignigena de secundus exsul, locus idoleum! Nunquam
              locus torquis. Sunt absolutioes amor neuter, castus plasmatores. A
              falsis, lura lotus luna. Ferox, placidus caesiums acceleratrix
              captis de fatalis, grandis nuclear vexatum iacere."
            </p>
            <div class="testimonials-01__author">
              Bob Musk
              <br />
              Chief Designer
            </div>
          </div>
        </li>
        <li class="slider__item">
          <div class="testimonials-01__item">
            <img
              class="testimonials-01__logo testimonials-01__logo--round"
              src="https://unicornplatform.com/app/img/photos/team-2/via-talen-de-st-croix.jpg" />
            <p class="testimonials-01__text">
              "Sunt habenaes carpseris camerarius, varius abaculuses. Nunquam
              locus cacula. Cur amor ortum? Vortex raptus candidatus est.
              Hercle, fraticinida varius!, fiscina! Hercle, nuptia audax!,
              mirabilis torquis! Lumens studere in albus aetheres! Impositios
              ridetis, tanquam azureus eleates. Azureus, nobilis indexs hic
              attrahendam de talis, mirabilis solitudo. Est festus lura,
              cesaris."
            </p>
            <div class="testimonials-01__author">
              Mark Jobs
              <br />
              Frontend developer-freelancer
            </div>
          </div>
        </li>
      </ul>
    </div>
  </div>
</div>
