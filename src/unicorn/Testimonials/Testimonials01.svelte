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
</script>

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
        {#each testimonials as { text, author, sub, img }}
          <li class="slider__item">
            <div class="testimonials-01__item">
              <img class="testimonials-01__logo" src={img} alt="" />
              <p class="testimonials-01__text">{text}</p>
              <div class="testimonials-01__author">
                {author}
                <br />
                {sub}
              </div>
            </div>
          </li>
        {/each}
      </ul>
    </div>
  </div>
</div>
