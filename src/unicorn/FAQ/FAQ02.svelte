<script>
  const _faq = { q: "Q?", a: "<p>a</p>" };
  export let main = "Main";
  export let sub = "Sub";
  export let faqs = [_faq, _faq, _faq, _faq];
  export let help = "Help";
  export let button = { title: "Send mail", link: "" };
  const c1 = faqs.slice(0, Math.floor(faqs.length / 2));
  const c2 = faqs.slice(Math.ceil(faqs.length / 2));
</script>

<div class="faq-02">

  <div class="container container--small">
    <div class="title-box title-box--center">
      <h2 class="heading">
         {main}
        <img class="emoji " src="img/emoji/chatbot.png" alt="Emoji" />
      </h2>
      <p class="title-box__text">{sub}</p>
    </div>
  </div>
  <div class="container faq-02__container">
    <ul class="faq-02__list">
      {#each c1 as { q, a }}
        <li class="faq-02__item">
          <img class="faq-02__icon" src="img/icons/help.svg" alt="" />
          <h2 class="faq-02__question_heading">{q}</h2>
          <div class="faq-02__answer">
            {@html a}
          </div>
        </li>
      {/each}
    </ul>
    <ul class="faq-02__list">
      {#each c2 as { q, a }}
        <li class="faq-02__item">
          <img class="faq-02__icon" src="img/icons/help.svg" alt="" />
          <h2 class="faq-02__question_heading">{q}</h2>
          <div class="faq-02__answer">
            {@html a}
          </div>
        </li>
      {/each}
    </ul>
  </div>
  <div class="container">
    <ul class="faq-02__button_box">
      <li class="faq-02__button">{help}</li>
      <br />
      <li class="faq-02__button">
        <a class="button button--midnight-outline " href={button.link}>
          <span>{button.title}</span>
        </a>
      </li>
    </ul>
  </div>
</div>
