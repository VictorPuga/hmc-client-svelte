<script>
  import { Input } from "../../components";
  export let main = "Main";
  export let sub = "Sub";
  export let buttonTitle = "Subscribe";
  export let placeholder = "Enter your email";

  // function send() {
  //   console.log("sending");
  //   var xhttp = new XMLHttpRequest();
  //   // xhttp.setRequestHeader("Access-Control-Allow-Origin", "*");
  //   xhttp.onreadystatechange = function() {
  //     if (this.readyState == 4 && this.status == 200) {
  //       // document.getElementById("demo").innerHTML = this.responseText;
  //       console.log("cool");
  //       console.log(this.responseText);
  //     }
  //   };
  //   xhttp.open(
  //     "POST",
  //     "https://icloud.us3.list-manage.com/subscribe/post?u=be39dc8883a8e4ab32a0dcb36&id=e47756e83b",
  //     true
  //   );
  //   xhttp.send();
  // }
</script>

<div class="cta_form-03">
  <div class="container container--mid">
    <div class="cta_form-03__wrapper">
      <div class="cta_form-03__heading_box">
        <h2 class="cta_form-03__heading">{main}</h2>
        <span class="cta_form-03__text">
          {@html sub}
        </span>
      </div>
      <div class="cta_form-03__form_box">
        <form
          class="form js-subscribe-mailchimp-form"
          method="post"
          action="https://icloud.us3.list-manage.com/subscribe/post?u=be39dc8883a8e4ab32a0dcb36&id=e47756e83b"
          id="mc-embedded-subscribe-form"
          name="mc-embedded-subscribe-form">
          <div class="form__inputs">
            <div class="form__input">
              <!-- TODO: Implement mail -->
              <Input type="email" name="EMAIL" {placeholder} />
              <div class="form__messages">
                <div
                  class="message message--engaging js-message
                  js-engaging-message"
                  data-index="email-form-15">
                  <div class="message__box">
                    <button
                      class="message__close js-close-message"
                      type="button">
                      <img
                        class="message__close_icon"
                        src="img/icons/corner-top--blue.svg"
                        alt="" />
                    </button>
                    <div class="message__body">
                      <div class="message__in">
                        <div class="message__bubble">
                          <div class="message__bubble_text">
                            Exciting product updates.
                          </div>
                        </div>
                        <div class="message__bubble">
                          <div class="message__bubble_text">
                            The hottest stories from the blog.
                          </div>
                        </div>
                        <div class="message__bubble">
                          <div class="message__bubble_text">
                            Exclusive discounts and gifts
                            <img
                              class="emoji "
                              src="img/emoji/smirking.png"
                              alt="Emoji" />
                          </div>
                        </div>
                      </div>
                      <div class="message__out">
                        <div class="message__out_box">
                          <div class="message__bubble">
                            <div
                              class="message__bubble_text
                              message__bubble_text--out js-reaction-text" />
                          </div>
                        </div>
                      </div>
                    </div>
                    <div class="message__reply_box">
                      <div class="message__reply_word">Reply</div>
                      <div class="message__options">
                        <div class="message__option">
                          <button
                            class="button js-react-on-message button--accent-bg "
                            type="submit">
                            <span class="button__text">I will join</span>
                          </button>
                        </div>
                        <div class="message__option">
                          <button
                            class="button js-react-on-message button--accent-bg "
                            type="submit">
                            <span class="button__text">Sounds sexy!</span>
                          </button>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
                <div
                  class="message message--success js-message js-success-message">
                  <div class="message__box">
                    <button
                      class="message__close js-close-message"
                      type="button">
                      <img
                        class="message__close_icon"
                        src="img/icons/corner-top--blue.svg"
                        alt="" />
                    </button>
                    <div class="message__body">
                      <div class="message__in">
                        <div class="message__bubble">
                          <div class="message__bubble_text">
                            <b>Success!</b>
                            Welcome aboard!
                            <img
                              class="emoji "
                              src="img/emoji/laughing.png"
                              alt="Emoji" />
                            Now go and confirm your subscription pls.
                          </div>
                        </div>
                        <div class="message__bubble">
                          <div class="message__bubble_text">
                            BTW, we post our happy faces on Instagram and
                            Twitter. Welcome:
                          </div>
                        </div>
                        <div class="message__bubble">
                          <div class="message__bubble_text">
                            <a
                              class="message__bubble_link"
                              href="https://instagram.com/unicornplatform">
                              https://instagram.com/unicornplatform
                            </a>
                          </div>
                        </div>
                        <div class="message__bubble">
                          <div class="message__bubble_text">
                            <a
                              class="message__bubble_link"
                              href="https://twitter.com/unicornplatform/">
                              https://twitter.com/unicornplatform
                            </a>
                          </div>
                        </div>
                      </div>
                      <div class="message__out">
                        <div class="message__out_box">
                          <div class="message__bubble">
                            <div
                              class="message__bubble_text
                              message__bubble_text--out js-reaction-text">
                              Coming!
                            </div>
                          </div>
                        </div>
                      </div>
                    </div>
                    <div class="message__reply_box">
                      <div class="message__reply_word">Reply</div>
                      <div class="message__options">
                        <div class="message__option">
                          <button
                            class="button js-react-on-message button--emerald-bg
                            "
                            type="submit">
                            <span class="button__text">Coming!</span>
                          </button>
                        </div>
                        <div class="message__option">
                          <button
                            class="button js-react-on-message button--emerald-bg
                            "
                            type="submit">
                            <span class="button__text">Got you there!</span>
                          </button>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="message message--error js-message js-error-message">
                  <div class="message__box">
                    <button
                      class="message__close js-close-message"
                      type="button">
                      <img
                        class="message__close_icon"
                        src="img/icons/corner-top--blue.svg"
                        alt="" />
                    </button>
                    <div class="message__body">
                      <div class="message__in">
                        <div class="message__bubble">
                          <div class="message__bubble_text">
                            <b>Error.</b>
                            Your form has not been submitted
                            <img
                              class="emoji "
                              src="img/emoji/cold_sweat.png"
                              alt="Emoji" />
                          </div>
                        </div>
                        <div class="message__bubble">
                          <div class="message__bubble_text">
                            This is what the server says:
                            <div
                              class="message__bubble_error js-error-message-text">
                              There must be an @ at the beginning.
                            </div>
                          </div>
                        </div>
                      </div>
                      <div class="message__out">
                        <div class="message__out_box">
                          <div class="message__bubble">
                            <div
                              class="message__bubble_text
                              message__bubble_text--out js-reaction-text">
                              I will retry
                            </div>
                          </div>
                        </div>
                      </div>
                    </div>
                    <div class="message__reply_box">
                      <div class="message__reply_word">Reply</div>
                      <div class="message__options">
                        <div class="message__option">
                          <button
                            class="button js-react-on-message button--ruby-bg "
                            type="submit">
                            <span class="button__text">Uh oh!</span>
                          </button>
                        </div>
                        <div class="message__option">
                          <button
                            class="button js-react-on-message button--ruby-bg "
                            type="submit">
                            <span class="button__text">I will retry</span>
                          </button>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="form__button">
              <button
                class="button js-submit-button button--alt-accent-bg "
                type="submit">
                <!-- on:click|preventDefault={send} -->
                <span class="button__text">{buttonTitle}</span>
                <div class="spinner" />
                <div class="button__submit_success">
                  <div class="button__success_circle" />
                  <div>
                    <svg
                      class="button__success_tick"
                      width="13"
                      height="13"
                      viewBox="0 0 13 13"
                      xmlns="http://www.w3.org/2000/svg">
                      <path
                        class="button__success_tick_path"
                        stroke="#FFF"
                        d="M0 8l5.119 3.873L11.709.381"
                        fill="none"
                        fill-rule="evenodd"
                        stroke-linecap="square" />
                    </svg>
                  </div>
                </div>
                <span class="icon">
                  <svg viewBox="0 0 13 10" xmlns="http://www.w3.org/2000/svg">
                    <path
                      d="M12.823 4.164L8.954.182a.592.592 0 0 0-.854 0 .635.635
                      0 0 0 0 .88l2.836 2.92H.604A.614.614 0 0 0 0 4.604c0
                      .344.27.622.604.622h10.332L8.1 8.146a.635.635 0 0 0 0
                      .88.594.594 0 0 0 .854 0l3.869-3.982a.635.635 0 0 0 0-.88z"
                      fill-rule="nonzero"
                      fill="#00396B" />
                  </svg>
                </span>
              </button>
            </div>
          </div>
        </form>
      </div>
    </div>
  </div>
</div>
