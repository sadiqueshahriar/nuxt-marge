<template>
  <div>
    <div class="header">
      <div class="header__logo">
        <a href="index.html"><img src="~/assets/images/logo.png" /></a>
      </div>
      <ul class="header__nav">
        <li class="nav-item dropdown">
          <a
            data-toggle="dropdown"
            href="#"
            role="button"
            aria-haspopup="true"
            aria-expanded="false"
            class="nav-link dropdown-toggle"
            >Dashboard</a
          >
          <div class="dropdown-menu">
            <a href="assets/index.html" class="dropdown-item">Assets</a>
            <a href="ref/index.html" class="dropdown-item">Ref</a>
          </div>
        </li>
        <li class="nav-item dropdown active">
          <a
            data-toggle="dropdown"
            href="#"
            role="button"
            aria-haspopup="true"
            aria-expanded="false"
            class="nav-link dropdown-toggle"
            >Trading</a
          >
          <div class="dropdown-menu">
            <span class=""
              ><a href="index.html" class="clickslider dropdown-item"
                >Exchange</a
              ></span
            >
            <span class="active"
              ><a href="index.html" class="dropdown-item">Liquidity</a></span
            >
          </div>
        </li>
        <li class="nav-item dropdown">
          <a
            data-toggle="dropdown"
            href="#"
            role="button"
            aria-haspopup="true"
            aria-expanded="false"
            class="nav-link dropdown-toggle"
            >Earn</a
          >
          <div class="dropdown-menu">
            <span class=""
              ><a href="staking/staking.html#/ICR/active" class="dropdown-item"
                >LP Staking</a
              ></span
            >
            <a href="#" class="dropdown-item">Solopool</a>
          </div>
        </li>
        <li class="nav-item">
          <a aria-current="page" href="pairs/index.html" class="nav-link"
            >Market</a
          >
        </li>
        <li class="nav-item">
          <a aria-current="page" href="games/index.html" class="nav-link"
            >Games</a
          >
        </li>
        <li class="nav-item">
          <a
            aria-current="page"
            target="_blank"
            href="https://intercroneworld.gitbook.io/intercrone/"
            class="nav-link"
            >FAQs</a
          >
        </li>
      </ul>
      <div class="header__grow"></div>
      <div class="header__tools">
        <!---->
        <button class="btn primary">Connect to wallet</button>
        <button class="btn header__cog">
          <img src="~/assets/images/cog.svg" />
        </button>
        <button class="btn header__bars">
          <img src="~/assets/images/bars.svg" />
        </button>
      </div>
      <!---->
      <!---->
    </div>
    <div class="page_header">
      <div class="container">
        <div class="row align-items-center">
          <div class="col-md-5">
            <div class="banner_left_content">
              <h2>SWAP Your</h2>
              <h1>TRC20</h1>
              <h3>Tokens</h3>
            </div>
          </div>
          <div class="col-md-7">
            <div class="form__wrap">
              <div class="form__swap">
                <ul class="form__nav">
                  <li class="active"></li>
                </ul>

                <h4 class="liquidity_text">
                  <img
                    class="arrow_img"
                    src="~assets/images/left-arrow.svg"
                    alt=""
                  />
                  Add Liquidity
                </h4>
                <div class="inp-box">
                  <div class="inp-box__head">
                    <div class="inp-box__label">From</div>
                    <div class="inp-box__balance">Balance: <b>0</b></div>
                  </div>
                  <div class="inp-box__wrap">
                    <input placeholder="0" class="inp-box__inp fff" />
                    <!---->

                    <span class="max_color">MAX</span>
                    <b-button
                      v-b-modal.modal-center
                      class="inp-box__token mm button_color_change"
                    >
                      <img
                        src=" https://intercroneswap.finance:2053/tokens/tokenalogo1623860470402.png "
                      />
                      <span class="color-black">TRX</span>
                      <!---->
                    </b-button>

                    <div class="modal_redious">
                      <b-modal
                        id="modal-center1"
                        top
                        title="Select a token"
                        hide-footer
                      >
                        <div class="select-token">
                          <input
                            placeholder="Search by name"
                            class="inp select-token__filter"
                          />
                          <div class="select-token__head">
                            <span class="select-token__head-label"
                              >Token name</span
                            >
                          </div>
                          <ul class="select-token__list">
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenalogo1623860470402.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">TRX</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenalogo1623852578883.jpg "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">WIN</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenalogo1623206974186.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">ICR</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenblogo1623860470402.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">SUN</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenblogo1623860372677.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">MEOX</div>
                            </li>
                            <li style="display: none">
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenblogo1623909860373.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">USDT</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenalogo1624264428747.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">JST</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenalogo1624264492447.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">BTC</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenalogo1624264550164.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">WBTT</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenblogo1624264599948.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">TUSD</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenalogo1624264635685.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">DOGE</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenblogo1624264677682.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">LTC</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenblogo1624264759498.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">LIVE</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenalogo1624264795719.jpg "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">DICE</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenalogo1624264845561.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">ETH</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenalogo1624264885029.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">NFT</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenalogo1624264922329.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">USDJ</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenblogo1624267570104.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">KLV</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenalogo1624382641258.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">HT</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenblogo1624428531816.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">UME</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenalogo1624636761283.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">NUTS</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenalogo1624686658383.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">TRONPAD</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenalogo1625231505798.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">SAFEMONEY</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenblogo1625207429295.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">JM</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenblogo1628703897592.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">WBTZC</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenblogo1629222855525.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">SOURCE</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenalogo1629535558350.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">USDC</div>
                            </li>
                            <li>
                              <img
                                src=" https://intercroneswap.finance:2053/tokens/tokenalogo1630249417746.png "
                                class="select-token__icon"
                              />
                              <div class="select-token__name">YFX</div>
                            </li>
                          </ul>
                        </div>
                      </b-modal>
                    </div>
                  </div>
                </div>
                <div class="form__to"></div>
                <div class="inp-box empty">
                  <div class="inp-box__head">
                    <div class="inp-box__label">To</div>
                    <!---->
                  </div>
                  <div class="inp-box__wrap">
                    <input placeholder="0" class="inp-box__inp bbb" />
                    <!---->

                    <b-button
                      v-b-modal.modal-center
                      class="inp-box__token nn empty button_color_change"
                    >
                      <!---->
                      <!---->
                      <span class="color-black">Select a token</span>
                    </b-button>
                    <b-modal
                      id="modal-center"
                      top
                      title="Select a token"
                      hide-footer
                    >
                      <div class="select-token">
                        <input
                          placeholder="Search by name"
                          class="inp select-token__filter"
                        />
                        <div class="select-token__head">
                          <span class="select-token__head-label"
                            >Token name</span
                          >
                        </div>
                        <ul class="select-token__list">
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenalogo1623860470402.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">TRX</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenalogo1623852578883.jpg "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">WIN</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenalogo1623206974186.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">ICR</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenblogo1623860470402.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">SUN</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenblogo1623860372677.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">MEOX</div>
                          </li>
                          <li style="display: none">
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenblogo1623909860373.png "
                              onerror="this.src = 'modules/site/main/assets/tokens/token.png'"
                              class="select-token__icon"
                            />
                            <div class="select-token__name">USDT</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenalogo1624264428747.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">JST</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenalogo1624264492447.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">BTC</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenalogo1624264550164.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">WBTT</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenblogo1624264599948.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">TUSD</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenalogo1624264635685.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">DOGE</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenblogo1624264677682.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">LTC</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenblogo1624264759498.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">LIVE</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenalogo1624264795719.jpg "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">DICE</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenalogo1624264845561.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">ETH</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenalogo1624264885029.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">NFT</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenalogo1624264922329.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">USDJ</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenblogo1624267570104.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">KLV</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenalogo1624382641258.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">HT</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenblogo1624428531816.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">UME</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenalogo1624636761283.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">NUTS</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenalogo1624686658383.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">TRONPAD</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenalogo1625231505798.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">SAFEMONEY</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenblogo1625207429295.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">JM</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenblogo1628703897592.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">WBTZC</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenblogo1629222855525.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">SOURCE</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenalogo1629535558350.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">USDC</div>
                          </li>
                          <li>
                            <img
                              src=" https://intercroneswap.finance:2053/tokens/tokenalogo1630249417746.png "
                              class="select-token__icon"
                            />
                            <div class="select-token__name">YFX</div>
                          </li>
                        </ul>
                      </div>
                    </b-modal>
                  </div>
                </div>
                <!---->
                <button class="btn primary form__submit">Select a token</button>
              </div>
              <!---->
            </div>
            <!---->
            <!---->
            <!---->
            <!---->
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
/* nav bar starts  */

body,
select,
textarea,
input,
button {
  font: 14px/1.3 "Poppins", sans-serif;
}

.header {
  display: flex;
  align-items: center;
  padding: 10px 30px;
  position: relative;
  background-color: #0a0a1e;
}

a {
  text-decoration: none;
  cursor: pointer;
  color: var(--primary-color);
}

img {
  vertical-align: middle;
  border-style: none;
}

.header__nav {
  list-style: none;
  display: flex;
  padding: 0 20px 0 30px;
  margin: 0;
}

li {
  display: list-item;
  text-align: -webkit-match-parent;
}

.dropdown-toggle::after {
  display: inline-block;
  margin-left: 0.255em;
  vertical-align: 0.255em;
  content: "";
  border-top: 0.3em solid;
  border-right: 0.3em solid transparent;
  border-bottom: 0;
  border-left: 0.3em solid transparent;
}

.header__nav li {
  padding: 0 15px;
}

.header__nav li.active a {
  color: #ffde00;
}

.header__nav a {
  color: #f2f2f2;
  font-size: 16px;
  padding: 5px 10px;
}

.nav-link {
  display: block;
  padding: 0.5rem 1rem;
}

.dropdown-toggle {
  white-space: nowrap;
}

.dropdown-menu {
  position: absolute;
  top: 100%;
  left: 0;
  z-index: 1000;
  display: none;
  float: left;
  min-width: 10rem;
  padding: 0.5rem 0;
  margin: 0.125rem 0 0;
  font-size: 1rem;
  color: #212529;
  text-align: left;
  list-style: none;
  background-color: #fff;
  background-clip: padding-box;
  border: 1px solid rgba(0, 0, 0, 0.15);
  border-radius: 0.25rem;
}

.header__nav li.active .dropdown-menu a {
  color: #f2f2f2;
}

.dropdown,
.dropleft,
.dropright,
.dropup {
  position: relative;
}

.dropdown-toggle::after {
  display: inline-block;
  margin-left: 0.255em;
  vertical-align: 0.255em;
  content: "";
  border-top: 0.3em solid;
  border-right: 0.3em solid transparent;
  border-bottom: 0;
  border-left: 0.3em solid transparent;
}

.dropdown-item {
  display: block;
  width: 100%;
  padding: 0.25rem 1.5rem;
  clear: both;
  font-weight: 400;
  color: #212529;
  text-align: inherit;
  white-space: nowrap;
  background-color: transparent;
  border: 0;
}

.header__grow {
  flex: 1 0;
}

.header__tools {
  display: flex;
  margin: -8px -5px;
}

.btn.primary {
  background-image: linear-gradient(90deg, #ffb807, #ffea00);
  border-radius: 50px;
  padding: 8px 30px;
  color: #0a0a1e;
  font-size: 16px;
  line-height: 24px;
  text-transform: capitalize;
  font-weight: 400;
}

.header__cog {
  padding: 2px 9px 4px 8px;
}

img {
  max-width: 100%;
}

.header__bars {
  padding: 11px 10px 3px;
}

.header__tools > * {
  margin: 0 5px;
}

.btn {
  color: #000;
  background: #f1f5f8;
  border: 1px solid transparent;
  padding: 5px 19px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  cursor: pointer;
  border-radius: 10px 10px;
  transition: 0.2s;
}

ul {
  display: block;
  list-style-type: disc;
  margin-block-start: 1em;
  margin-block-end: 1em;
  margin-inline-start: 0px;
  margin-inline-end: 0px;
  padding-inline-start: 40px;
}

@media screen and (max-width: 599.98px) {
  .header__logo {
    text-align: center;
    padding: 0 0 30px 0;
  }
}

@media screen and (max-width: 599.98px) {
  .header {
    flex-direction: column;
  }
}

@media screen and (max-width: 479.98px) {
  .layout {
    zoom: 0.8;
  }
}

@media screen and (max-width: 1199.98px) {
  .header__nav {
    display: none;
  }
}

@media screen and (max-width: 599.98px) {
  .header__tools {
    justify-content: center;
  }
}

/* navbar end */

/* hero  component style starts */
.page_header {
  min-height: 100vh;
  padding: 50px 0 20px;
  margin: 0;
  border: 0;
  display: flex;
  align-items: center;
  background-image: url(~/assets/images/home_banner.jpg);
  background-size: cover;
  background-repeat: no-repeat;
}

.banner_left_content:before {
  content: "";
  background-image: url(~/assets/images/home_banner_01.png);
  width: 235px;
  height: 464px;
  position: absolute;
  top: -150px;
  left: 0;
  right: 0;
  margin: 0 auto;
  z-index: -1;
}

.banner_left_content {
  position: relative;
  text-align: center;
  z-index: 50;
}

.banner_left_content h1 {
  color: #f3c914;
  font-size: 96px;
  font-weight: 700;
  margin: 0;
  line-height: 75px;
  text-transform: uppercase;
}

.banner_left_content h2 {
  font-size: 48px;
  color: #0a0a1e;
  margin: 0;
  line-height: 50px;
  text-transform: uppercase;
}

.banner_left_content h3 {
  font-size: 37px;
  color: #0a0a1e;
  margin: 0;
  text-transform: uppercase;
}

.form__wrap {
  margin: 0 auto;
  max-width: 440px;
  border-radius: 30px;
  background: rgba(255, 255, 255, 0.4);
  box-shadow: 0 -3px 5px rgb(0 0 0 / 3%);
}

.form__swap {
  background-color: #fff;
  box-shadow: 0 0 10px 5px rgb(0 0 0 / 10%);
  border-radius: 15px;
  color: #0a0a1e;
  padding: 30px 20px;
  z-index: 99;
  position: relative;
}

.form__nav {
  list-style: none;
  margin: 0 0 20px 0;
  padding: 10px 0;
  align-items: center;
  justify-content: space-around;
  display: flex;
}

.form__nav li {
  padding: 0 10px;
  text-align: center;
}

.form__nav li.active a {
  color: #f3c914;
}

.inp-box {
  /* background: rgb(255 233 0 / 10%); */
  border-radius: 20px;
  padding: 15px 20px;
}

.form__to {
  background: url(~/assets/images/arrow-to.svg) no-repeat center;
  padding: 30px 0;
  cursor: pointer;
}

.inp-box__head {
  display: flex;
}

.inp-box__label {
  flex: 1 0;
  font-size: 16px;
}

.inp-box__balance {
  font-size: 16px;
}

b,
strong {
  font-weight: bolder;
}

.inp-box__wrap {
  display: flex;
  padding: 7px 0 0;
  align-items: center;
}

.inp-box__inp {
  flex: 1 0;
  font-size: 30px;
  font-weight: 500;
  background: none;
  border: none;
  min-width: 40px;
  overflow: hidden;
  text-overflow: ellipsis;
  border-bottom: 2px solid #dadada;
}

.inp-box__token {
  display: flex;
  align-items: center;
  cursor: pointer;
  border-radius: 2px 2px;
  padding: 7px 8px;
  white-space: nowrap;
}

.inp-box__token span {
  margin: 0 0 0 8px;
  font-size: 20px;
}

.inp-box__token:after {
  content: "";
  background: url(~/assets/images/arrow-down.svg);
  width: 11px;
  height: 5px;
  margin: 0 0 0 15px;
}

.form__to {
  background: url(~/assets/images/arrow-to.svg) no-repeat center;
  padding: 30px 0;
  cursor: pointer;
}

.inp-box {
  /* background: rgb(255 233 0 / 10%); */
  border-radius: 20px;
  padding: 15px 20px;
}

.inp-box__head {
  display: flex;
}

.inp-box__label {
  flex: 1 0;
  font-size: 16px;
}

.inp-box__wrap {
  display: flex;
  padding: 7px 0 0;
  align-items: center;
}

.inp-box__inp {
  flex: 1 0;
  font-size: 30px;
  font-weight: 500;
  background: none;
  border: none;
  min-width: 40px;
  overflow: hidden;
  text-overflow: ellipsis;
  border-bottom: 2px solid #dadada;
}

.inp-box__token.empty {
  background: #fff;
  box-shadow: 0px 0px 5px rgb(186 10 115 / 10%);
}

.inp-box__token {
  display: flex;
  align-items: center;
  cursor: pointer;
  border-radius: 2px 2px;
  padding: 7px 8px;
  white-space: nowrap;
}

.inp-box__token:after {
  content: "";
  background: url(~/assets/images/arrow-down.svg);
  width: 11px;
  height: 5px;
  margin: 0 0 0 15px;
}

.form__submit {
  margin: 20px 0 0;
  width: 100%;
  padding: 18px 0;
  font-size: 19px;
  box-shadow: 0px 4px 4px rgb(255 187 7 / 30%);
}

.inp-box__token img {
  max-width: 24px;
  max-height: 24px;
}

.button_color_change {
  background: transparent !important;
  border: transparent !important;
}

.button_color_change:hover {
  background: transparent !important;
  border: transparent !important;
}

.select-token__filter {
  width: 100%;
}

.select-token__head {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 15px 0;
  margin: 10px 0 0;
}

.select-token__head-label {
  font-size: 18px;
}

.select-token__list {
  list-style: none;
  padding: 0;
  height: calc(100vh - 320px);
  overflow: auto;
  overflow-x: hidden;
}

.select-token__list li {
  display: flex;
  border-top: 2px dashed #f2f2f2;
  padding: 12px 0;
  align-items: center;
  cursor: pointer;
}

.select-token__icon {
  max-height: 20px;
  width: 20px;
}

.select-token__name {
  padding: 0 10px;
  flex: 1 0;
  font-size: 14px;
}

.color-black {
  color: black;
}

.liquidity_text {
  margin-left: 18px;
  margin-top: -18px;
}

.arrow_img {
  height: 18px;
  width: 18px;
}

.max_color {
  color: #f3c914;
  font-weight: 600;
}

.btn.primary {
  background-image: linear-gradient(90deg, #ffb807, #ffea00);

  border-radius: 50px;
  padding: 8px 30px;
  color: #0a0a1e;
  font-size: 16px;
  line-height: 24px;
  text-transform: capitalize;
  font-weight: 400;
}

.inp {
  background: #fff;
  border: 1px solid #adbcc7;
  padding: 8px 9px 9px;
  display: inline-block;
  border-radius: var(--border-radius);
  transition: 0.2s;
}

@media screen and (max-width: 767px) {
  .page_header {
    padding: 50px 0 80px;
  }
}

@media screen and (max-width: 767px) {
  .banner_left_content:before {
    top: -40px;
    background-size: 40%;
    background-repeat: no-repeat;
    background-position: center top;
  }
}

::-webkit-scrollbar {
  width: 6px;
}

/* Track */

/* Handle */
::-webkit-scrollbar-thumb {
  background: #ffb807;
  border-radius: 6px;
}

.modal_redious {
  border: 1px solid transparent !important;
  border-radius: 10px !important;
}

*,
*:after,
*:before {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body,
select,
textarea,
input,
button {
  font: 14px/1.3 "Poppins", sans-serif;
}

button,
input {
  overflow: visible;
}

input {
  text-rendering: auto;
  color: -internal-light-dark(black, white);
  letter-spacing: normal;
  word-spacing: normal;
  line-height: normal;
  text-transform: none;
  text-indent: 0px;
  text-shadow: none;
  display: inline-block;
  text-align: start;
  appearance: auto;
  -webkit-rtl-ordering: logical;
  cursor: text;
  background-color: -internal-light-dark(rgb(255, 255, 255), rgb(59, 59, 59));
  margin: 0em;
  padding: 1px 2px;
  border-width: 2px;
  border-style: inset;
  border-color: -internal-light-dark(rgb(118, 118, 118), rgb(133, 133, 133));
  border-image: initial;
}

*,
*::before,
*::after {
  box-sizing: border-box;
}

/* hero components style end */
</style>