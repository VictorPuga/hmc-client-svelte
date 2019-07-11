<script>
  const _card = {
    main: "Main",
    sub: "Sub",
    img: "",
    prices: [0, 0],
    items: ["a", "b", "c"],
    button: { title: "Start Now", link: "/" }
  };
  export let main = "Main";
  export let sub = "Sub";
  export let tabs = ["Monthly", "Yearly"];
  export let badgeText = "+2 free months";
  export let cards = [_card, _card, _card];

  let selectedIndex = 0;

  function changeTab(i) {
    selectedIndex = i;
  }
</script>

<div class="pricing-01" style="width: 100%">
  <div class="container container--small">
    <div class="title-box title-box--center">
      <h2 class="heading">{main}</h2>
      <p class="title-box__text">{sub}</p>
    </div>
  </div>
  <div class="container">
    <div class="pricing-01__buttons">
      <ul class="pricing-01__buttons_list">
        {#each tabs as tab, i}
          <li class="tab">
            <button
              class="tab__button {i == selectedIndex ? 'state-active-tab' : ''}
              js-open-tab"
              type="button"
              data-index="yearly-price-1"
              data-group="my-pricing-group-1"
              on:click={() => changeTab(i)}>
               {tab}
            </button>
          </li>
        {/each}
      </ul>
      {#if selectedIndex == tabs.length - 1}
        <div
          class="pricing-01__badge js-tab-content state-active-tab"
          data-index="yearly-price-1"
          data-group="my-pricing-group-1">
          <span
            class="pointed-badge pointed-badge--acid-bg pointed-badge--left">
            <span class="pointed-badge__text">{badgeText}</span>
            <img class="emoji " src="img/emoji/gift.png" alt="Emoji Gift PNG" />
          </span>
        </div>
      {/if}
    </div>
  </div>
  <div
    class="container"
    style="width: 100%; max-width: 100%; background:
    url(img/other/honeycomb.svg)">
    <div class="pricing-01__cards_container">
      <ul class="pricing-01__cards_list">
        {#each cards as { main, sub, img, prices, items, button: { title, link } }}
          <li class="pricing-01__card_box">
            <div class="pricing-01__card">
              <div class="pricing-01__card_top">
                <img class="pricing-01__card_img" src={img} alt={main} />
              </div>
              <div class="pricing-01__card_bottom">
                <div class="pricing-01__card_title_box">
                  <h3 class="pricing-01__card_title">{main}</h3>
                  <div
                    class="pricing-01__card_price js-tab-content
                    state-active-tab"
                    data-index="monthly-price-1"
                    data-group="my-pricing-group-1">
                    ${prices[selectedIndex]}
                    <div class="pricing-01__card_period">/mes</div>
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
                        <div class="pricing-03__benefit_text"> {item} </div>
                      </li>
                    {/each}
                  </ul>
                </div>
                <div class="pricing-01__card_button">
                  <button class="button button--black-outline" type="submit">
                    <a href={link} style="text-decoration: none;">
                      <span class="button__text">{title}</span>
                    </a>
                  </button>
                </div>
              </div>
            </div>
          </li>
        {/each}
      </ul>
    </div>
  </div>
</div>
