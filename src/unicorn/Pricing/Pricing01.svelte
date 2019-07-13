<script>
  import { Button } from "../../components";
  const _card = {
    main: "Main",
    sub: "Sub",
    img: "",
    prices: [0, 0],
    items: ["a", "b", "c"],
    button: { title: "Start Now", href: "/" }
  };
  export let main = "Main";
  export let sub = "Sub";
  export let tabs = ["Monthly", "Yearly"];
  export let unit = "month";
  export let badgeText = "+2 free months";
  export let cards = [_card, _card, _card];
</script>

<div class="pricing-01" style="width: 100%" id="subscription-plans">
  <div class="container container--small">
    <div class="title-box title-box--center">
      <h2 class="heading">{main}</h2>
      <p class="title-box__text">{sub}</p>
    </div>
  </div>
  <div class="container">
    <div class="pricing-01__buttons">
      <ul class="pricing-01__buttons_list">
        <li class="tab">
          <button
            class="tab__button state-active-tab js-open-tab"
            type="button"
            data-index="monthly-price-1"
            data-group="my-pricing-group-1">
             {tabs[0]}
          </button>
        </li>
        <li class="tab">
          <button
            class="tab__button js-open-tab"
            type="button"
            data-index="yearly-price-1"
            data-group="my-pricing-group-1">
             {tabs[1]}
          </button>
        </li>
      </ul>
      <div
        class="pricing-01__badge js-tab-content"
        data-index="yearly-price-1"
        data-group="my-pricing-group-1">
        <span class="pointed-badge pointed-badge--left">
          <span class="pointed-badge__text">{badgeText}</span>
          <img class="emoji " src="img/emoji/gift.png" alt="Emoji Gift PNG" />
        </span>
      </div>
    </div>
  </div>
  <div
    class="container"
    style="width: 100%; max-width: 100%; background:
    url(img/other/honeycomb.svg)">
    <div class="pricing-01__cards_container">
      <ul class="pricing-01__cards_list">
        {#each cards as { main, sub, img, prices, items, button }}
          <li class="pricing-01__card_box">
            <div class="pricing-01__card">
              <div class="pricing-01__card_top">
                <img
                  class="pricing-01__card_img"
                  src={img}
                  alt={main}
                  draggable="false" />
              </div>
              <div class="pricing-01__card_bottom">
                <div class="pricing-01__card_title_box">
                  <h3 class="pricing-01__card_title">{main}</h3>
                  <div
                    class="pricing-01__card_price js-tab-content
                    state-active-tab"
                    data-index="monthly-price-1"
                    data-group="my-pricing-group-1">
                    ${prices[0]}
                    <div class="pricing-01__card_period">/{unit}</div>
                  </div>
                  <div
                    class="pricing-01__card_price js-tab-content"
                    data-index="yearly-price-1"
                    data-group="my-pricing-group-1">
                    ${prices[1]}
                    <div class="pricing-01__card_period">/{unit}</div>
                  </div>
                </div>
                <div class="pricing-01__card_info text">
                   {sub}
                  <br />
                  <br />
                  <ul
                    class="pricing-03__benefits_list"
                    style="min-height: 340px">
                    {#each items as item}
                      <li class="pricing-03__benefit">
                        <img
                          src="img/icons/checked--acid.svg"
                          class="pricing-03__benefit_icon"
                          alt=">" />
                        <div class="pricing-03__benefit_text">{item}</div>
                      </li>
                    {/each}
                  </ul>
                </div>
                <div class="pricing-01__card_button">
                  <Button variant="outline" {...button} />
                </div>
              </div>
            </div>
          </li>
        {/each}
      </ul>
    </div>
  </div>
</div>
