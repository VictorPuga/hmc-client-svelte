<script>
  export let cards = ["Card1", "Card2"];
</script>

<div class="text--01">
  <ul class="pricing-01__cards_list ">
    {#each cards as card}
      <li style="max-width: 380px; padding-bottom: 15px">
        <div class="container container--small">
          <div class="text--01__box">
            <div class="text--01__emoji">
              <img
                class="emoji emoji--large"
                src="img/emoji/raising_hands.png"
                alt="Emoji" />
            </div>
            <p class="text--01__content white-text">{card}</p>
          </div>
        </div>
      </li>
    {/each}
  </ul>
</div>
