<template>
<div>
    <header>
    <nav class="navbar navbar-expand-lg">
      <div class="container-fluid">
        <a class="navbar-brand" href="#"><img src="~/assets/images/logo.png" alt=""></a>
        <div class="d-flex align-items-center">
          <form class="pe-2 d-block d-sm-none">
            <button class="custom-btn" type="submit">Register</button>
          </form>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <img src="~/assets/images/menu.svg" alt="" style="width: 35px">
          </button>
        </div>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto">
            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle d-flex align-items-center" href="#" data-bs-toggle="dropdown">
                <span>Dashboard</span>
              </a>
              <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">Assets</a></li>
                <li>
                  <a class="dropdown-item" href="#">Ref</a>
                </li>
              </ul>
            </li>

            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle" href="#" data-bs-toggle="dropdown">
                Trading
              </a>
              <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">Exchange</a></li>
                <li>
                  <a class="dropdown-item" href="#">Liquidity</a>
                </li>
                <li>
                  <a class="dropdown-item" href="#"> Cash balance</a>
                </li>
              </ul>
            </li>
            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle" href="#" data-bs-toggle="dropdown">
                Earn
              </a>
              <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">Staking</a></li>
                <li>
                  <a class="dropdown-item" href="#">Solopool</a>
                </li>
              </ul>
            </li>

            <li class="nav-item">
              <a class="nav-link d-flex align-items-center" href="#">Market
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link d-flex align-items-center" href="#">Games
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link d-flex align-items-center" href="#">FAQs
              </a>
            </li>
          </ul>
          <ul class="navbar-nav align-items-center">
            <li class="nav-item">
              <a class="nav-link" href="#">Connect to Wallet</a>
            </li>
            <li class="nav-item d-none d-sm-block">
              <form class="px-2">

              </form>
            </li>

            <li class="nav-item">

            </li>
            <li class="nav-item d-flex align-items-center">

              <span style="color: #5e6673">|</span>

            </li>
            <li class="nav-item"></li>
          </ul>
        </div>
      </div>
    </nav>
  </header>
  <!-- header end -->
      <div class="banner">
    <div class="container">
      <div class="banner-heading">
        <h2>Farms</h2>
        <p>
          Stake LP tokens to earn. <br>
          <a href="#">Apply for a LP-Staking<i class="fa fa-arrow-right"></i></a>
        </p>
      </div>
    </div>
  </div>
  <!-- _____[TABLE]_______ -->
  <div class="container">
    <div class="table-common">
      <div class="table-common-header">
        <div class="row">
          
          <div class="col-md-2 col-6">
            <label class="switchSmall2 m5">
              <input type="checkbox" checked="">
              <small></small>
              <p>Staked only</p>
            </label>
          </div>
          <div class="col-md-3 col-12">
            <div class="tab-slider-nav">
              <ul class="tab-slider-tabs" :class="{'slide': tab_slider == 'tab2'}">
                <li class="tab-slider-trigger" @click="tabSlider('tab1')" :class="{'active': tab_slider == 'tab1'}" rel="tab1">Live</li>
                <li class="tab-slider-trigger" @click="tabSlider('tab2')" :class="{'active': tab_slider == 'tab2'}" rel="tab2">Finished</li>
              </ul>
            </div>
          </div>
          <div class="col-md-6 col-12">
            <div class="input-group-custom">
              <div class="select-filter">
                <label for="" class="filter-label">SORT BY</label>
                <select name="" id="" class="custom-select">
                  <option value="" selected="">Hot</option>
                  <option value="">ARR</option>
                  <option value="">Earned</option>
                  <option value="">Total stacked</option>
                </select>
              </div>
              <div class="search-filter">
                <label for="" class="filter-label">Search</label>
                <input type="text" placeholder="Search Pools">
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="tab-slider-container">
        <div id="tab1" class="tab-slider-body" v-if="tab_slider == 'tab1'">
          <div class="table-grid">
            <div class="accordion" id="accordionExample">
              <div class="accordion-item">
                <h2 class="accordion-header" id="headingOne">
                  <button @click="showToggle('first')" :class="{'collapsed': tab != 'first'}" class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="false" aria-controls="collapseOne">
                    <div class="grid-row">
                      <div class="grid-col">
                        <div class="main-data">
                          <div class="coin-img">
                            <img src="~/assets/images/soloicr.png" alt="">
                            <img src="~/assets/images/btc.png" class="img-icon" alt="">
                          </div>
                          <div class="coin-name">
                            <h3>TokenA-TokenB</h3>
                          </div>
                        </div>
                      </div>
                      <div class="grid-col">
                        <div class="col-heading">Earned</div>
                        <div class="dull-data">0</div>
                      </div>
                      <div class="grid-col">
                        <div class="col-heading">APR</div>
                        <div class="strong-data">83.67%</div>
                      </div>
                      <div class="grid-col d-none d-md-block">
                        <div class="col-heading">Liquidity</div>
                        <div class="strong-data">$770,509,475</div>
                      </div>
                      <div class="grid-col d-none d-md-block">
                        <div class="col-heading">End at</div>
                        <div class="strong-data">20.11.2021 14:00</div>
                      </div>
                      <div class="grid-col d-none d-md-block">
                        <div class="detail-btn">Details</div>
                      </div>
                    </div>
                  </button>
                </h2>
                <div :class="{'collapse': tab != 'first'}" id="collapseOne" class="accordion-collapse" aria-labelledby="headingOne" data-bs-parent="#accordionExample" style="">
                  <div class="accordion-body">
                    <div class="row">
                      <div class="col-md-6 col-12" style="
    margin-top: 18px;
">
                        <div class="row">
                          <div class="col-md-6 col-12">
                            <div class="token-details">
                              <div class="detail-link">
                                <a href="#">See Token Info
                                  <i class="fa fa-external-link"></i></a>
                              </div>
                              <div class="detail-link">
                                <a href="#">View Project Site
                                  <i class="fa fa-external-link"></i></a>
                              </div>
                              <div class="detail-link">
                                <a href="#">View Contract
                                  <i class="fa fa-external-link"></i></a>
                              </div>
                              
                            </div>
                          </div>
                          <div class="col-md-6 col-12">
                            <div class="
                                  d-flex
                                  align-items-center
                                  justify-content-between
                                " style="
    padding-top: 5px;
    padding-bottom: 5px;
">
                              <div class="normal-text">Staking fee:</div>
                              <div class="normal-text"><b>3%</b></div>
                            </div>
                            <div class="
                                  d-flex
                                  align-items-center
                                  justify-content-between
                                " style="
    padding-top: 5px;
    padding-bottom: 5px;
">
                              <div class="normal-text">
                                Referral payments:
                              </div>
                              <div class="normal-text"><b>15%</b></div>
                            </div>
                            <div class="
                                  d-flex
                                  align-items-center
                                  justify-content-between
                                " style="padding-top: 2px;padding-bottom: 2px;">
                              <div class="normal-text">Started at</div>
                              <div class="normal-text">
                                <b>29.7.2021, 12:41:39</b>
                              </div>
                            </div>
                            
                          </div>
                        </div>
                      </div>
                      <div class="col-md-3 col-12">
                        <div class="profit-box" style="
    margin-top: 8px;
">
                          <div class="profit-heading">Reward Info</div>
                          <div class="profit-data">
                            <div>
                              <div class="profit-number">64.4756876 ICR</div>
                              <div class="dull-data-small">0 USD</div>
                            </div>
                            <button class="profit-btn harvest block">Harvest</button>
                          </div>
                        </div>
                      </div>
                      <div class="col-md-3 col-12">
                        <div class="profit-box" style="
    margin-top: 8px;
">
                          <div class="profit-heading">Start Staking</div>
                          <div class="profit-data">
                            <button class="profit-btn w-100">
                              Connect Wallet
                            </button>
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
              <div class="accordion-item">
                <h2 class="accordion-header" id="headingTwo">
                  <button @click="showToggle('second')" :class="{'collapsed': tab != 'second'}" class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
                    <div class="grid-row">
                      <div class="grid-col">
                        <div class="main-data">
                          <div class="coin-img">
                            <img src="~/assets/images/soloicr.png" alt="">
                            <img src="~/assets/images/logob.png" class="img-icon" alt="">
                          </div>
                          <div class="coin-name">
                            <h3>TokenA-TokenB</h3>
                          </div>
                        </div>
                      </div>
                      <div class="grid-col">
                        <div class="col-heading">Earned</div>
                        <div class="dull-data">0</div>
                      </div>
                      <div class="grid-col">
                        <div class="col-heading">APR</div>
                        <div class="strong-data">83.67%</div>
                      </div>
                      <div class="grid-col d-none d-md-block">
                        <div class="col-heading">Liquidity</div>
                        <div class="strong-data">$770,509,475</div>
                      </div>
                      <div class="grid-col d-none d-md-block">
                        <div class="col-heading">End at</div>
                        <div class="strong-data">20.09.2021 14:00</div>
                      </div>
                      <div class="grid-col d-none d-md-block">
                        <div class="detail-btn">Details</div>
                      </div>
                    </div>
                  </button>
                </h2>
                <div :class="{'collapse': tab != 'second'}" id="collapseTwo" class="accordion-collapse" aria-labelledby="headingTwo" data-bs-parent="#accordionExample" style="">
                  <div class="accordion-body">
                    <div class="row">
                      <div class="col-md-4 col-12">
                        <div class="token-details">
                          <div class="detail-link">
                            <a href="#">Get CAKE-BNB LP
                              <i class="fa fa-external-link"></i></a>
                          </div>
                          <div class="detail-link">
                            <a href="#">View Contract
                              <i class="fa fa-external-link"></i></a>
                          </div>
                          <div class="detail-link">
                            <a href="#">See Pair Info
                              <i class="fa fa-external-link"></i></a>
                          </div>
                          <div class="auto-btn">
                            <a href="#">
                              <i class="fa fa-sync"></i> &nbsp;&nbsp; Core
                            </a>
                          </div>
                        </div>
                      </div>
                      <div class="col-md-4 col-12">
                        <div class="profit-box">
                          <div class="profit-heading">Cake Earned</div>
                          <div class="profit-data">
                            <div class="profit-number">0</div>
                            <button class="profit-btn" disabled="">
                              Harvest
                            </button>
                          </div>
                        </div>
                      </div>
                      <div class="col-md-4 col-12">
                        <div class="profit-box">
                          <div class="profit-heading">Start Stalking</div>
                          <div class="profit-data">
                            <button class="profit-btn w-100">
                              Connect Wallet
                            </button>
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div id="tab2" class="tab-slider-body" v-if="tab_slider == 'tab2'">
          <h2 class="info-msg">These pools are no longer distributing rewards. Please unstake your tokens.</h2>
          <div class="table-grid">
            <div class="accordion" id="accordionExample">
              <div class="accordion-item">
                <h2 class="accordion-header" id="headingOne">
                  <button @click="showToggle('third')" :class="{'collapsed': tab != 'third'}" class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="false" aria-controls="collapseOne">
                    <div class="grid-row">
                      <div class="grid-col">
                        <div class="main-data">
                          <div class="coin-img">
                            <img src="~/assets/images/soloicr.png" alt="">
                            <img src="~/assets/images/btc.png" class="img-icon-top" alt="">
                          </div>
                          <div class="coin-name">
                            <h3>CAKE-BNB</h3>
                          </div>
                        </div>
                      </div>
                      <div class="grid-col">
                        <div class="col-heading">Earned</div>
                        <div class="dull-data">0</div>
                      </div>
                      <div class="grid-col">
                        <div class="col-heading">APR</div>
                        <div class="strong-data">83.67%</div>
                      </div>
                      <div class="grid-col d-none d-md-block">
                        <div class="col-heading">Liquidity</div>
                        <div class="strong-data">$770,509,475</div>
                      </div>
                      <div class="grid-col d-none d-md-block">
                        <div class="col-heading">End at</div>
                        <div class="strong-data">20.10.2021 14:00</div>
                      </div>
                      <div class="grid-col d-none d-md-block">
                        <div class="detail-btn">Details</div>
                      </div>
                    </div>
                  </button>
                </h2>
                <div :class="{'collapse': tab != 'third'}" id="collapseOne" class="accordion-collapse" aria-labelledby="headingOne" data-bs-parent="#accordionExample" style="">
                  <div class="accordion-body">
                    <div class="row">
                      <div class="col-md-6 col-12" style="
    margin-top: 18px;
">
                        <div class="row">
                          <div class="col-md-6 col-12">
                            <div class="token-details">
                              <div class="detail-link">
                                <a href="#">See Token Info
                                  <i class="fa fa-external-link"></i></a>
                              </div>
                              <div class="detail-link">
                                <a href="#">View Project Site
                                  <i class="fa fa-external-link"></i></a>
                              </div>
                              <div class="detail-link">
                                <a href="#">View Contract
                                  <i class="fa fa-external-link"></i></a>
                              </div>
                              
                            </div>
                          </div>
                          <div class="col-md-6 col-12">
                            <div class="
                                  d-flex
                                  align-items-center
                                  justify-content-between
                                " style="
    padding-top: 5px;
    padding-bottom: 5px;
">
                              <div class="normal-text">Staking fee:</div>
                              <div class="normal-text"><b>3%</b></div>
                            </div>
                            <div class="
                                  d-flex
                                  align-items-center
                                  justify-content-between
                                " style="
    padding-top: 5px;
    padding-bottom: 5px;
">
                              <div class="normal-text">
                                Referral payments:
                              </div>
                              <div class="normal-text"><b>15%</b></div>
                            </div>
                            <div class="
                                  d-flex
                                  align-items-center
                                  justify-content-between
                                " style="padding-top: 2px;padding-bottom: 2px;">
                              <div class="normal-text">Started at</div>
                              <div class="normal-text">
                                <b>29.7.2021, 12:41:39</b>
                              </div>
                            </div>
                            
                          </div>
                        </div>
                      </div>
                      <div class="col-md-3 col-12">
                        <div class="profit-box" style="
    margin-top: 8px;
">
                          <div class="profit-heading">Reward Info</div>
                          <div class="profit-data">
                            <div>
                              <div class="profit-number">64.4756876 ICR</div>
                              <div class="dull-data-small">0 USD</div>
                            </div>
                            <button class="profit-btn harvest block">Harvest</button>
                          </div>
                        </div>
                      </div>
                      <div class="col-md-3 col-12">
                        <div class="profit-box" style="
    margin-top: 8px;
">
                          <div class="profit-heading">Start Staking</div>
                          <div class="profit-data">
                            <button class="profit-btn w-100">
                              Connect Wallet
                            </button>
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
              <div class="accordion-item">
                <h2 class="accordion-header" id="headingTwo">
                  <button @click="showToggle('forth')" :class="{'collapsed': tab != 'forth'}" class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
                    <div class="grid-row">
                      <div class="grid-col">
                        <div class="main-data">
                          <div class="coin-img">
                            <img src="~/assets/images/soloicr.png" alt="">
                            <img src="~/assets/images/logob.png" class="img-icon-top" alt="">
                          </div>
                          <div class="coin-name">
                            <h3>CAKE-BNB</h3>
                          </div>
                        </div>
                      </div>
                      <div class="grid-col">
                        <div class="col-heading">Earned</div>
                        <div class="dull-data">0</div>
                      </div>
                      <div class="grid-col">
                        <div class="col-heading">APR</div>
                        <div class="strong-data">83.67%</div>
                      </div>
                      <div class="grid-col d-none d-md-block">
                        <div class="col-heading">Liquidity</div>
                        <div class="strong-data">$770,509,475</div>
                      </div>
                      <div class="grid-col d-none d-md-block">
                        <div class="col-heading">End at</div>
                        <div class="strong-data">20.10.2021 14:00</div>
                      </div>
                      <div class="grid-col d-none d-md-block">
                        <div class="detail-btn">Details</div>
                      </div>
                    </div>
                  </button>
                </h2>
                <div :class="{'collapse': tab != 'forth'}" id="collapseTwo" class="accordion-collapse" aria-labelledby="headingTwo" data-bs-parent="#accordionExample" style="">
                  <div class="accordion-body">
                    <div class="row">
                      <div class="col-md-4 col-12">
                        <div class="token-details">
                          <div class="detail-link">
                            <a href="#">Get CAKE-BNB LP
                              <i class="fa fa-external-link"></i></a>
                          </div>
                          <div class="detail-link">
                            <a href="#">View Contract
                              <i class="fa fa-external-link"></i></a>
                          </div>
                          <div class="detail-link">
                            <a href="#">See Pair Info
                              <i class="fa fa-external-link"></i></a>
                          </div>
                          <div class="auto-btn">
                            <a href="#">
                              <i class="fa fa-sync"></i> &nbsp;&nbsp; Core
                            </a>
                          </div>
                        </div>
                      </div>
                      <div class="col-md-4 col-12">
                        <div class="profit-box">
                          <div class="profit-heading">Cake Earned</div>
                          <div class="profit-data">
                            <div class="profit-number">0</div>
                            <button class="profit-btn" disabled="">
                              Harvest
                            </button>
                          </div>
                        </div>
                      </div>
                      <div class="col-md-4 col-12">
                        <div class="profit-box">
                          <div class="profit-heading">Start Stalking</div>
                          <div class="profit-data">
                            <button class="profit-btn w-100">
                              Connect Wallet
                            </button>
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
</template>
<script>
export default {
  data() {
    return {
      tab: '',
      currentTab: '',
      tab_slider: 'tab1'
    }
  },
  methods: {
    showToggle(tab) {
      if(this.currentTab) {
        if(tab == this.currentTab) {
          this.tab = ''
          this.currentTab = ''
          return
        } else {
          this.tab = tab
          this.currentTab = tab
        }
      }
      this.tab = tab
      this.currentTab = tab
    }, 
    tabSlider(tab) {
      this.tab_slider = tab
      this.tab = ''
      this.currentTab = ''
    }
  }
}
</script>
<style scoped>
/*--------------------------------------------------------------
------------------------ Common Styling ------------------------
--------------------------------------------------------------*/

@import url('https://fonts.googleapis.com/css2?family=Heebo:wght@100;200;300;400;500;600;700;800;900&display=swap');

body {
    font-family: Heebo, 'sans-serif';
    background-color: #FAFAFA;
    color: rgb(30, 35, 41);
}

.custom-btn {
    color: rgb(33, 40, 51);
    border-radius: 4px;
    padding: 6px 12px;
    min-height: 24px;
    border: none;
    background-image: linear-gradient(rgb(248, 209, 47) 0%, rgb(240, 185, 11) 100%);
    min-width: 52px;
    font-weight: 400;
    font-size: 14px;
    line-height: 20px;
}

.navbar {
    background-color: #181A20;
}

.navbar .nav-item .dropdown-menu {
    display: none;
}

.navbar .nav-item:hover .dropdown-menu {
    display: block;
}

.navbar .nav-item .dropdown-menu {
    margin-top: 0;
}

.nav-item .nav-link {
    color: #ffffff;
}

.arrow-link {
    box-sizing: border-box;
    margin: 0;
    min-width: 0;
    display: -webkit-box;
    display: -webkit-flex;
    display: -ms-flexbox;
    display: flex;
    position: relative;
    border-radius: 4px;
    margin-left: 8px;
    padding-left: 4px;
    padding-right: 4px;
    font-size: 12px;
    line-height: 16px;
    background-color: #F0B90B;
    color: #1E2329;
}

.arrow-link:before {
    content: "";
    position: absolute;
    width: 0;
    height: 0;
    left: -3px;
    top: 2px;
    border-left: 0;
    border-top: 6px solid transparent;
    border-bottom: 6px solid transparent;
    border-right: 6px solid;
    border-right-color: #F0B90B;
}

.chart-card {
    margin-bottom: 16px;
    padding: 16px;
    display: block;
    background-color: #fff;
    color: #1E2329;
    position: relative;
    border-radius: 3px;
    box-shadow: rgb(0 0 0 / 4%) 0px 0px 20px 0px;
}

.chart-card .chart-heading {
    box-sizing: border-box;
    margin: 0;
    min-width: 0;
    font-size: 14px;
}

.chart-prices {
    white-space: nowrap;
    font-size: 20px;
    color: rgb(209, 160, 51);
    font-weight: 500;
}

.chart-prices span {
    font-weight: 400;
    color: #707A8A;
    margin-left: 4px;
    font-size: 12px;
}

.chart-volume {
    font-size: 12px;
    margin: 0;
    min-width: 0;
    color: #707A8A;
    margin-right: 2px;
}

.chart-card img {
    top: 10%;
    right: 20px;
    position: absolute;
}

.chart-volume span {
    margin-right: 8px;
    font-weight: 400;
    color: rgb(14, 203, 129);
}

.table-header {
    margin: 24px 0;
}

.nav-tabs .nav-item {
    padding: 0 1rem;
}

.nav-tabs .nav-item:first-child {
    padding-left: 0;
}

.nav-tabs .nav-item .nav-link {
    box-sizing: border-box;
    margin: 0;
    min-width: 0;
    padding-top: 16px;
    padding-bottom: 16px;
    font-size: 14px;
    color: #707A8A;
    position: relative;
    white-space: nowrap;
    font-weight: 500;
    cursor: pointer;
    border: 0;
    padding-left: 0;
    padding-right: 0;
}

.nav-tabs .nav-item .nav-link.active::after {
    content: "";
    width: 100%;
    left: 0px;
    height: 3px;
    position: absolute;
    bottom: 0px;
    background-color: rgb(240, 185, 11);
}

.nav-pills .nav-item .nav-link {
    margin: 0px 12px 0px 0px;
    cursor: pointer;
    white-space: nowrap;
    outline: none;
    border-radius: 4px;
    padding: 5px 16px;
    min-height: 24px;
    border: 1px solid rgb(230, 230, 230);
    box-shadow: none;
    min-width: 52px;
    font-size: 12px;
    font-weight: 400;
    line-height: 16px;
    background-color: transparent;
    color: rgb(30, 35, 41);
}

.nav-pills .nav-item .nav-link.active {
    color: rgb(201, 148, 0);
    border: 1px solid rgb(252, 234, 156);
    background-color: rgb(255, 253, 240);
}

.dropdown-menu {
    background-color: #181A20;
}

.dropdown-item {
    color: #ffffff;
}

.table-header .form-control {
    color: #1E2329;
    font-size: 14px;
    padding-left: 8px;
    padding-right: 8px;
    padding: 0;
    outline: none;
    border: none;
    height: 48px;
    background-color: #ffffff;
}

.table-header .input-group {
    border: 1px solid transparent;
    border-color: #EAECEF;
    border-radius: 4px;
    transition: all 0.3s ease;
}

.table-header .form-control:focus {
    outline: none;
    box-shadow: none;
}

.table-header .input-group:focus-within {
    border: 1px solid #ffde00;
}

.table-header .input-group:hover {
    border: 1px solid #ffde00;
}

.table-header .input-group-text {
    background-color: #ffffff;
    border: none;
    outline: none;
}

.table-header .input-group-text .fa {
    color: #848E9C
}

.table-main {
    background-color: #ffffff;
    width: 100%;
    padding: 24px;
}

.table-custom {
    background-color: #ffffff;
    width: 100%;
}

.table-custom thead {
    border-bottom: 1px solid rgb(234, 236, 239);
    border-top-color: rgb(234, 236, 239);
    border-right-color: rgb(234, 236, 239);
    border-left-color: rgb(234, 236, 239);
    background-color: #fafafa;
}

.table-custom thead th {
    padding: 16px 8px;
    line-height: 16px;
    font-size: 12px;
    color: #707a8a;
}

.table-custom tbody tr {
    border-bottom: 1px solid rgb(234, 236, 239);
    border-top-color: rgb(234, 236, 239);
    border-right-color: rgb(234, 236, 239);
    border-left-color: rgb(234, 236, 239);
}

.table-custom>tbody>tr:hover {
    background-color: rgb(245, 245, 245);
}

.table-custom tbody td {
    font-size: 14px;
    line-height: 16px;
    font-weight: 400;
    height: 50px;
    padding: 0 8px;
    color: rgb(30, 35, 41);
}

.table-custom .name-data {
    display: flex;
    align-items: center;
}

.table-custom .img-data {
    display: inline-block;
    height: 21px;
    width: 21px;
    border: 2px solid #fff;
    background: #fff;
    border-radius: 21px;
    box-shadow: 0 0 0 1px #e3e3e3;
    overflow: hidden;
}

.table-custom .img-data img {
    width: 100%;
    height: 100%;
}

.name-data .name {
    margin-left: 16px;
    font-size: 16px;
    color: rgb(30, 35, 41);
}

.name-data .name p {
    font-size: 12px;
    color: rgb(112, 122, 138);
    margin: 0;
}




/*--------------------------------------------------------------
------------------------ Pools Page Styling --------------------
--------------------------------------------------------------*/

.banner {
    background: linear-gradient(90deg, #ffb807, #ffea00);
}

.banner-heading {
    padding: 32px 0;
}

.banner-heading h2 {
    font-size: 50px;
    font-weight: 600;
    line-height: 1.1;
    margin-top: 0;
    margin-bottom: 24px;
    color: #ffffff;
}

.banner-heading p {
    font-size: 20px;
    font-weight: 600;
    line-height: 1.1;
    color: #ffffff;
}

.banner-heading p a {
    text-decoration: none;
    color: #c99400;
    display: block;
    margin-top: 10px;
}

.banner-heading p a i {
    font-size: 14px;
    padding-left: 5px;
}

.change-grid {
    display: flex;
    align-items: center;
    justify-content: space-evenly;
}

.change-grid a {
    text-decoration: none;
}

.change-grid a svg {
    fill: #bdc2c4;
}

.change-grid a svg.active {
    fill: #ffea00;
}

.switchSmall2 {
    display: flex;
    align-items: center;
}

.switchSmall2 input {
    display: none;
}

.switchSmall2 small {
    display: inline-block;
    width: 38px;
    height: 15px;
    background: #eeeaf4;
    border-radius: 30px;
    position: relative;
    cursor: pointer;
}

.switchSmall2 small:before {
    content: "";
    position: absolute;
    width: 19px;
    height: 19px;
    background: #fcea9c;
    border-radius: 50%;
    border: 1px solid transparent;
    top: -2px;
    left: -1px;
    transition: .3s;
    box-shadow: -3px 0 3px rgba(0, 0, 0, 0.25);
}

.switchSmall2 input:checked~small {
    background: #ffea00;
    transition: .3s;
    border-color: #7e7c77;
}

.switchSmall2 input:checked~small:before {
    transform: translate(20px, 0px);
    transition: .3s;
    box-shadow: 3px 0 3px rgba(0, 0, 0, 0.25);
}

.table-common {
    padding: 32px 0;
}

.table-common-header {
    padding: 16px 24px;
}

.switchSmall2 p {
    color: #280d5f;
    margin-left: 8px;
    font-size: 16px;
    font-weight: 400;
    line-height: 1.5;
    margin-bottom: 0;
}

.tab-slider-nav {
    width: 100%;
    float: left;
    margin-bottom: 20px;
}

.tab-slider-tabs {
    display: block;
    float: left;
    margin: 0;
    padding: 0;
    list-style: none;
    position: relative;
    border-radius: 35px;
    border: 1px solid #ffea00;
    overflow: hidden;
    background: #fffdf0;
    height: 35px;
    -webkit-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    user-select: none;
}

.tab-slider-tabs:after {
    content: "";
    width: 50%;
    background: #ffea00;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
    transition: all 250ms ease-in-out;
    border-radius: 35px;
}

.tab-slider-tabs.slide:after {
    left: 50%;
}

.tab-slider-trigger {
    font-size: 12px;
    line-height: 1;
    font-weight: bold;
    color: #c99400;
    text-transform: uppercase;
    text-align: center;
    padding: 11px 20px;
    position: relative;
    z-index: 2;
    cursor: pointer;
    display: inline-block;
    transition: color 250ms ease-in-out;
    -webkit-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    user-select: none;
}

.tab-slider-trigger.active {
    color: #fff;
}

.tab-slider-body {
    margin-bottom: 20px;
}

.input-group-custom {
    display: flex;
    align-items: center;
    justify-content: flex-end;
}

.select-filter {
    margin-right: 15px;
}

.input-group-custom label {
    display: block;
    margin-bottom: 0;
}

.input-group-custom select,
.input-group-custom input {
    color: rgb(40, 13, 95);
    font-weight: 500;
    line-height: 1.1;
    padding: 11px 20px;
    position: relative;
    z-index: 2;
    cursor: pointer;
    transition: all 250ms ease-in-out;
    width: 100%;
    height: 40px;
    display: flex;
    -webkit-box-align: center;
    align-items: center;
    -webkit-box-pack: justify;
    justify-content: space-between;
    padding: 0px 16px;
    box-shadow: rgb(74 74 104 / 10%) 0px 2px 2px -1px inset;
    border: 1px solid #fcea9c;
    border-radius: 16px;
    background: #fffdf0;
    transition: all 0.15s ease 0s;
}

.input-group-custom select {
    margin-right: 10px;
}

.input-group-custom select:focus,
.input-group-custom label input:focus {
    outline: none !important;
    box-shadow: none !important;
}

.filter-label {
    color: rgb(39, 37, 47);
    font-weight: 600;
    line-height: 1.5;
    text-transform: uppercase;
    font-size: 12px;
}

/* .input-group-custom select option{
    background: #fefdf0;
    position: absolute;
    border-bottom-left-radius: 14px;
    border-bottom-right-radius: 14px;
    top: -30px;
} */

.table-grid .accordion-item:first-of-type .accordion-button {
    border-top-left-radius: 24px;
    border-top-right-radius: 24px;
}

.table-grid .accordion-item:first-of-type {
    border-top-left-radius: 24px;
    border-top-right-radius: 24px;
}

.table-grid .accordion-button {
    padding: 0 16px;
    border-bottom: 1px solid #cdcdcd;
}

.table-grid .accordion-button:not(.collapsed) {
    color: inherit;
    background: #ffffff !important;
    box-shadow: none !important;
}

.table-grid .accordion-button:focus {
    border-color: transparent !important;
    box-shadow: none !important;
}

.grid-row {
    width: 100%;
    display: flex;
    justify-content: space-between;
    flex-direction: row;
}

.grid-col {
    flex: 1;
    max-width: fit-content;
    padding: 24px 8px;
}

.main-data {
    display: flex;
    align-items: center;
}

.main-data .coin-img {
    position: relative;
}

.main-data .coin-img img {
    z-index: 2;
    width: 40px;
    position: relative;
}

.main-data .coin-img .img-icon {
    width: 20px;
    position: absolute;
    bottom: -5px;
    right: -5px;
}

.main-data .coin-img .img-icon-top {
    width: 20px;
    position: absolute;
    top: -5px;
    left: -5px;
    z-index: 1;
}

.coin-name {
    margin-left: 16px;
}

.coin-name h4 {
    margin: 0;
    font-size: 16px;
    color: rgb(30, 35, 41);
}

.coin-name h3 {
    color: rgb(40, 13, 95);
    font-size: 16px;
    font-weight: 600;
    line-height: 1.5;
    margin: 0;
}

.coin-name p {
    font-size: 12px;
    color: rgb(112, 122, 138);
    margin: 0;
}

.col-heading {
    color: #c99400;
    font-weight: 400;
    line-height: 1.2;
    font-size: 12px;
}

.dull-data {
    color: rgb(189, 194, 196);
    font-weight: 600;
    line-height: 1.2;
    margin-top: 4px;
    font-size: 16px;
}

.dull-data-small {
    color: rgb(189, 194, 196);
    line-height: 1.2;
    font-size: 12px;
}

.strong-data {
    color: rgb(40, 13, 95);
    font-weight: 400;
    line-height: 1.5;
    font-size: 16px;
}

.detail-btn {
    color: #c99400;
    font-size: 16px;
    font-weight: 600;
    line-height: 3;
}

.table-grid .accordion-body {
    background: rgb(246, 246, 246);
}

.detail-link {
    margin-bottom: 8px;
}

.detail-link a {
    color: #c99400;
    font-size: 16px;
    font-weight: 400;
    line-height: 1.5;
    text-decoration: none;
}

.detail-link a:hover {
    text-decoration: underline;
}

.detail-link a i {
    margin-left: 3px;
}

.auto-btn a {
    align-items: center;
    border-radius: 16px;
    display: inline-flex;
    font-weight: 400;
    white-space: nowrap;
    height: 28px;
    padding: 0px 8px;
    font-size: 14px;
    color: #c99400;
    background: transparent;
    border: 2px solid #c99400;
    text-decoration: none;
}

.manual-btn a {
    align-items: center;
    border-radius: 16px;
    display: inline-flex;
    font-weight: 400;
    white-space: nowrap;
    height: 28px;
    padding: 0px 8px;
    font-size: 14px;
    color: rgb(40, 13, 95);
    border: 1px solid rgb(40, 13, 95);
    overflow: hidden;
    background: #fffdf0;
    text-decoration: none;
}

.profit-box {
    height: auto;
    max-height: 450px;
    margin-top: 1rem;
    padding: 16px;
    border: 2px solid rgb(238, 234, 244);
    border-radius: 16px;
}

.profit-heading {
    color: #c99400;
    font-weight: 600;
    line-height: 1.5;
    text-transform: uppercase;
    font-size: 12px;
}

.profit-data {
    display: flex;
    align-items: center;
    justify-content: space-between;
    /* flex-direction: column; */
}

.profit-number {
    font-size: 13px;
    font-weight: 600;
    line-height: 1.5;
}

.profit-btn:disabled {
    background: rgb(233, 234, 235);
    border-color: rgb(233, 234, 235);
    box-shadow: none;
    color: rgb(189, 194, 196);
    cursor: not-allowed;
}

.profit-btn {
    -webkit-box-align: center;
    align-items: center;
    border: 0px;
    border-radius: 16px;
    box-shadow: rgba(14, 14, 44, 40%) 0px -1px 0px 0px inset;
    cursor: pointer;
    display: inline-flex;
    font-family: inherit;
    font-size: 16px;
    font-weight: 600;
    -webkit-box-pack: center;
    justify-content: center;
    letter-spacing: 0.03em;
    line-height: 1;
    opacity: 1;
    outline: 0px;
    height: 48px;
    padding: 0px 24px;
    background-image: linear-gradient(rgb(248, 209, 47) 0%, rgb(240, 185, 11) 100%);
    color: white;
    margin-top: 5px;
    margin-left: auto;
}

.profit-btn.harvest{
    height: 42px;
    padding: 0 16px;
    font-size: 13px;
    border-radius: 10px;
}


.info-msg {
    color: rgb(237, 75, 158);
    font-weight: 400;
    line-height: 1.5;
    padding-bottom: 32px;
    font-size: 20px;
}

.grid-card {
    position: relative;
    width: 100%;
    overflow: hidden;
    height: fit-content;
    background: rgb(255, 255, 255);
    border-radius: 24px;
}

.grid-card.active {
    background: linear-gradient(#ffb807, #fcea9c) 0% 0% / 400% 400%;
    border-radius: 24px;
    overflow: hidden;
    animation: 3s ease 0s infinite normal none running shadowAnime;
    padding: 1px 1px 3px;
}

.grid-card-header {
    background-color: #fffdf0;
    display: flex;
    align-items: center;
    justify-content: space-between;
    border-radius: 24px 24px 0px 0px;
    padding: 24px;
}

.header-heading h3 {
    font-size: 24px;
    font-weight: 600;
    line-height: 1.1;
    color: #c99400;
    margin: 0;
}

.header-heading p {
    color: rgb(122, 110, 170);
    font-size: 16px;
    font-weight: 400;
    line-height: 1.5;
    margin: 0;
}

.header-img {
    position: relative;
}

.header-img img {
    width: 60px;
}

.header-img .img-small {
    width: 32px !important;
    position: absolute;
    bottom: -5px;
    right: -5px;
}

.grid-card-body {
    padding: 24px;
    background-color: #ffffff;
}

.body-heading {
    display: flex;
    -webkit-box-align: center;
    align-items: center;
    -webkit-box-pack: justify;
    justify-content: space-between;
}

.body-heading p {
    color: rgb(40, 13, 95);
    font-size: 16px;
    font-weight: 400;
    line-height: 1.5;
    text-decoration: underline dotted rgb(122, 110, 170);
    text-underline-offset: 0.1em;
}

.body-heading h5 {
    color: rgb(40, 13, 95);
    font-weight: 600;
    line-height: 1.5;
    font-size: 16px;
}

.body-extra {
    margin-top: 24px;
}

.body-extra h6 {
    color: rgb(40, 13, 95);
    font-weight: 400;
    line-height: 1.5;
    font-size: 14px;
}

.underlined-text {
    color: rgb(40, 13, 95);
    font-weight: 400;
    line-height: 1.5;
    font-size: 14px;
    text-decoration: underline dotted rgb(122, 110, 170);
    text-underline-offset: 0.1em;
}

.body-button {
    margin-top: 24px;
}

.body-button h5 {
    color: #c99400;
    font-weight: 600;
    line-height: 1.5;
    text-transform: uppercase;
    margin-bottom: 10px;
    font-size: 12px;
}

.body-button button {
    -webkit-box-align: center;
    align-items: center;
    border: 0px;
    border-radius: 16px;
    box-shadow: rgb(14 14 44 / 40%) 0px -1px 0px 0px inset;
    cursor: pointer;
    display: inline-flex;
    font-family: inherit;
    font-size: 16px;
    font-weight: 600;
    -webkit-box-pack: center;
    justify-content: center;
    letter-spacing: 0.03em;
    line-height: 1;
    opacity: 1;
    outline: 0px;
    height: 48px;
    padding: 0px 24px;
    background-image: linear-gradient(rgb(248, 209, 47) 0%, rgb(240, 185, 11) 100%);
    color: white;
}

.grid-card-footer {
    border-top: 1px solid rgb(231, 227, 235);
    padding: 24px;
    background-color: #ffffff;
    border-radius: 0 0 24px 24px;
}

.show-hidden {
    cursor: pointer;
    color: #c99400;
    transition: all .3s ease-in-out;
}

.show-hidden:hover {
    color: #F0B90B;
}

.hidden-menu {
    margin-top: 10px;
    display: none;
}

.normal-text {
    color: rgb(40, 13, 95);
    font-size: 14px;
    font-weight: 400;
    line-height: 1.5;
}

.card-finished {
    z-index: 10;
    background-color: rgb(189, 194, 196);
    color: white;
    margin: 0px;
    padding: 5px 0px;
    position: absolute;
    right: 0px;
    top: 0px;
    text-align: center;
    transform: translateX(30%) translateY(0%) rotate(45deg);
    transform-origin: left top;
    width: 85px;
}

.card-finished>div {
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
    width: 85px;
}

.card-finished::before {
    right: 100%;
}

.card-finished::after {
    left: 100%;
}

.card-finished::before,
.card-finished::after {
    background-color: rgb(189, 194, 196);
    content: "";
    height: 100%;
    margin: 0px -1px;
    position: absolute;
    top: 0px;
    width: 100%;
}

.grid-card.disabled-card .grid-card-header {
    background-color: rgb(233, 234, 235);
}

.disabled-card .header-heading h3,
.disabled-card .header-heading p {
    color: rgb(189, 194, 196);
}

.blank-tag {
    border: 1px solid #ffea00;
    overflow: hidden;
    background: #fffdf0;
    color: #c99400;
    border-radius: 16px;
    height: 28px;
    padding: 0px 8px;
    text-align: center;
    font-size: 14px;
    margin-right: 5px;
}

.blank-tag svg {
    margin-right: 4px;
    align-self: center;
    fill: #c99400;
}

.filled-tag {
    border: 1px solid #ffea00;
    overflow: hidden;
    background: #ffea00;
    align-items: center;
    border-radius: 16px;
    color: rgb(255, 255, 255);
    display: inline-flex;
    font-weight: 400;
    white-space: nowrap;
    height: 28px;
    padding: 0px 8px;
    font-size: 14px;
}

.img-reversed img {
    z-index: 2;
    position: relative;
}

.img-reversed .img-small {
    top: -10px !important;
    left: -10px !important;
    z-index: 1;
}

@media (max-width: 992px) {
    .accordion-button span {
        padding-left: 0
    }
}

@keyframes shadowAnime {
    0% {
        background-position: 50% 0%;
    }

    50% {
        background-position: 50% 100%;
    }

    100% {
        background-position: 50% 0%;
    }
}
</style>