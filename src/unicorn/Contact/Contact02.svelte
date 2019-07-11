<script>
  const _icon = { img: "", link: "/", platform: "" };
  export let main = "Main";
  export let contacts = [{ title: "hey", email: "hey@hey.hey" }];
  export let icons = [_icon, _icon, _icon];
</script>

<div class="footer-01" style="padding: 40px 40px 120px 40px">
  <div class="container container--mid">
    <ul class="contact-02__list">
      <li class="contact-02__list_item">
        <h3 class="contact-02__item_title">{main}</h3>
        <div class="contact-02__social social-buttons social-buttons--left">
          <ul class="social-buttons__list">
            {#each icons as { img, link, platform }}
              <li class="social-buttons__item">
                <a class="social-buttons__link" href={link} target="_blank">
                  <img class="social-buttons__icon" src={img} alt={platform} />
                </a>
              </li>
            {/each}
          </ul>
        </div>
      </li>
      {#each contacts as { title, email }}
        <li class="contact-02__list_item">
          <h3 class="contact-02__item_title">{title}</h3>
          <a
            class="contact-02__link link"
            href="mailto:{email}"
            target="_blank">
             {email}
          </a>
        </li>
      {/each}
    </ul>
  </div>
</div>
