<script>
  const _feature = {
    title: "Title",
    description: "Description...",
    img: ""
  };
  export let pre = "";
  export let main = "Main";
  export let sub = "Sub";
  export let features = [_feature, _feature];
</script>

<div class="features-01" id="features">
  <div class="container container--small">
    <div class="features-01__title_box">
      <div class="subheading">{pre}</div>
      <h2 class="heading heading--accent">{main}</h2>
      <p>{sub}</p>
    </div>
  </div>
  <div class="container" style="padding: 0 5%">
    <ul class="features-01__items">
      {#each features as { title, description, img }}
        <li class="features-01__item">
          <div class="feature">
            <h3 class="feature__title">
              <img class="feature__icon" src={img} alt={title} />
              <span class="feature__title_text"> {title} </span>
            </h3>
            <p class="feature__content">
              <span>{description}</span>
            </p>
          </div>
        </li>
      {/each}
    </ul>
  </div>
</div>
