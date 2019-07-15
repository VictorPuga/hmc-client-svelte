<script>
  import { Input } from "../../components";
  export let main = "Main";
  export let sub = "Sub";
  export let buttonTitle = "Subscribe";
  export let placeholder = "Enter your email";
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
          action="https://icloud.us3.list-manage.com/subscribe/post?u=be39dc8883a8e4ab32a0dcb36&amp;id=e47756e83b"
          method="post"
          id="mc-embedded-subscribe-form"
          name="mc-embedded-subscribe-form">
          <div class="form__inputs">
            <div class="form__input">
              <input
                class="text-input js-email-input"
                type="email"
                name="EMAIL"
                {placeholder} />
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
                        alt="close" />
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
                              message__bubble_text--out js-reaction-text">
                              <!--updated via JS, no need to enter any text here-->
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
                        alt="close" />
                    </button>
                    <div class="message__body">
                      <div class="message__in">
                        <div class="message__bubble">
                          <div class="message__bubble_text">
                            <b>¡Éxito!</b>
                            Bienvenido a bordo
                            <img
                              class="emoji "
                              src="img/emoji/laughing.png"
                              alt="Emoji" />
                            Ahora tu subscripción está confirmada, hacker.
                          </div>
                        </div>
                        <div class="message__bubble">
                          <div class="message__bubble_text">
                            Por cierto, no olvides vernos en nuestras redes:
                          </div>
                        </div>
                        <div class="message__bubble">
                          <div class="message__bubble_text">
                            <a
                              class="message__bubble_link"
                              href="https://join.slack.com/t/hacker-mafia/shared_invite/enQtNjgzMzQwMzA3MDcyLTQ3ZmM0ZTVhNzEwYjFlM2QyYzA5NTc3M2M0NjIwY2Y0Y2ZkZmFlNmM3ODZmMDE4YWQ1NmM1YWRjZmZmOTY0MGY">
                              Slack
                            </a>
                          </div>
                        </div>
                        <div class="message__bubble">
                          <div class="message__bubble_text">
                            <a
                              class="message__bubble_link"
                              href="https://www.facebook.com/Hacker-Mafia-386592791984319/">
                              Facebook
                            </a>
                          </div>
                        </div>
                        <div class="message__bubble">
                          <div class="message__bubble_text">
                            <a
                              class="message__bubble_link"
                              href="https://twitter.com/hackermafiaclub">
                              Twitter
                            </a>
                          </div>
                        </div>
                        <div class="message__bubble">
                          <div class="message__bubble_text">
                            <a
                              class="message__bubble_link"
                              href="https://medium.com/hacker-mafia-club">
                              Medium
                            </a>
                          </div>
                        </div>
                        <div class="message__bubble">
                          <div class="message__bubble_text">
                            <a
                              class="message__bubble_link"
                              href="javascript:alert('coming soon')">
                              Instagram
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
                            class="button js-react-on-message button--emerald-bg"
                            type="submit">
                            <span class="button__text">¡Genail!</span>
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
                        alt="close" />
                    </button>
                    <div class="message__body">
                      <div class="message__in">
                        <div class="message__bubble">
                          <div class="message__bubble_text">
                            <b>Error.</b>
                            No se ha podido resolver tu petición
                            <img
                              class="emoji "
                              src="img/emoji/cold_sweat.png"
                              alt="Emoji" />
                          </div>
                        </div>
                        <div class="message__bubble">
                          <div class="message__bubble_text">
                            Esto nos ha dicho el servidor:
                            <div
                              class="message__bubble_error js-error-message-text">
                              CONTENT TO BE REPLACED
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
                            style="display: none"
                            class="button js-react-on-message button--ruby-bg
                            change-preferences-button"
                            type="submit">
                            <span class="button__text">
                              Cambia tus preferencias
                            </span>
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
