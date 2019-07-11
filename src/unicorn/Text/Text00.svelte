<script>
  export let main = "Main";
  export let sub = "Sub";
  export let items = ["1", "2", "3"];
</script>

<div class="testimonials-01" style="padding: 0px 0 20px">
  <img
    src="img/other/triangle.svg"
    height="203"
    width="100%"
    draggable="false"
    alt="" />
  <div class="container container--small">
    <div class="title-box title-box--center">
      <h2 class="heading">{main}</h2>
      <p class="title-box__text"> {sub} </p>
      <ul class="pricing-03__benefits_list">
        {#each items as item}
          <li class="pricing-03__benefit">
            <img
              src="img/icons/arrow-pointing-to-right--blue.svg"
              class="pricing-03__benefit_icon"
              alt=">" />
            <div class="pricing-03__benefit_text">{item}</div>
          </li>
        {/each}
        <!-- <li class="pricing-03__benefit">
          <img
            src="img/icons/arrow-pointing-to-right--blue.svg"
            class="pricing-03__benefit_icon"
            alt=">" />
          <div class="pricing-03__benefit_text">Bootcamps: $300</div>

        </li>
        <li class="pricing-03__benefit">
          <img
            src="img/icons/arrow-pointing-to-right--blue.svg"
            class="pricing-03__benefit_icon"
            alt=">" />
          <div class="pricing-03__benefit_text">Hackathones: $400</div>
        </li> -->
      </ul>
    </div>
  </div>
  <img
    src="img/other/triangle.svg"
    height="203"
    width="100%"
    style="transform: rotate(180deg)"
    draggable="false"
    alt="" />
</div>
