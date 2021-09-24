<template>
<div>
  <header>
    <nav class="navbar navbar-expand-lg">
      <div class="container-fluid">
        <a class="navbar-brand" href="#"
          ><img src="~/assets/images/logo.png" alt=""
        /></a>
        <div class="d-flex align-items-center">
          <form class="pe-2 d-block d-sm-none">
            <button class="custom-btn" type="submit">Register</button>
          </form>
          <button
            class="navbar-toggler"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#navbarSupportedContent"
            aria-controls="navbarSupportedContent"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <img src="~/assets/images/menu.svg" alt="" style="width: 35px" />
          </button>
        </div>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto">
            <li class="nav-item dropdown">
              <a
                class="nav-link dropdown-toggle d-flex align-items-center"
                href="#"
                data-bs-toggle="dropdown"
              >
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
              <a
                class="nav-link dropdown-toggle"
                href="#"
                data-bs-toggle="dropdown"
              >
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
              <a
                class="nav-link dropdown-toggle"
                href="#"
                data-bs-toggle="dropdown"
              >
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
              <a class="nav-link d-flex align-items-center" href="#">Market </a>
            </li>
            <li class="nav-item dropdown">
              <a
                class="nav-link dropdown-toggle"
                href="#"
                data-bs-toggle="dropdown"
              >
                Games
              </a>
              <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">HATCH AN EGG</a></li>
              </ul>
            </li>
            <li class="nav-item">
              <a class="nav-link d-flex align-items-center" href="#">FAQs </a>
            </li>
          </ul>
          <ul class="navbar-nav align-items-center">
            <li class="nav-item">
              <a class="nav-link" href="#">Connect to Wallet</a>
            </li>
            <li class="nav-item d-none d-sm-block">
              <form class="px-2"></form>
            </li>

            <li class="nav-item"></li>
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
      <div class="container-fluid">
        <div class="row align-items-center">
          <div class="col-md-6">
            <div class="text-center">
              <h3 class="common-heading">WELCOME TO</h3>
              <h1 class="main-heading">HATCH AN EGG</h1>
              <h5>PARTICIPATE IN OUR HATCH AN EGG GAME</h5>
            </div>

            <p class="p-md-3">
              HATCHED AN EGG IS THE ONE OF THE MOST EXCITING ADVENTURES THAT YOU
              CAN EXPERIENCE. YOU WILL NEED TO BUY A BLANKET TO COVER YOUR EGG
              FROM PREDATORS AND KEEP IT WARM, THE AIM IS TO HATCH YOUR OWN EGG
              AND BE THE LUCKY WINNER OF THE SHARE POT AT THE END OF EACH ROUND.
            </p>
          </div>
          <div class="col-md-6 text-center">
            <img src="~/assets/images/egglogo.png" class="w-100" alt="" />
          </div>
        </div>
      </div>
    </div>

    <!-- _____[GAMING CARDS]_______ -->
    <div class="container-fluid mb-5">
      <div class="row">
        <div class="col-md-4 mb-3">
          <div class="gaming-card">
            <div class="yellow-circle"></div>
            <div class="card-data">
              <h4 class="card-heading">BREETHER REWARD</h4>
            </div>
          </div>
        </div>
        <div class="col-md-4 mb-3">
          <div class="gaming-card">
            <div class="yellow-circle"></div>
            <div class="card-data">
              <h4 class="card-heading">CURRENT BIDDER</h4>
            </div>
          </div>
        </div>
        <div class="col-md-4 mb-3">
          <div class="gaming-card">
            <div class="yellow-circle"></div>
            <div class="card-data">
              <h4 class="card-heading">RESET GAME</h4>
              <button class="card-btn">RESET GAME</button>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- _____[BUY BLANKET]_______ -->
    <div class="white-heading mb-3">BUY A BLANKET</div>
    <div class="container-fluid p-md-5 mb-5 text-center">
      <div class="row">
        <div class="col-md-6 mb-3">
          <div class="d-flex justify-content-center mb-4">
            <div class="balance-card">BALANCE</div>
            <div class="balance-card">1 BLANKET</div>
          </div>
          <button class="common-btn">BUY BLANKET</button>
        </div>
        <div class="col-md-6 mb-3">
          <h3 class="common-heading">START BROODING</h3>
          <h5 style="font-size: 50px; margin-top: 20px">00:00:03:14</h5>
        </div>
      </div>
    </div>

    <!-- _____[DUMMY CONTENT]_______ -->
    <div class="container mt-5">
      <div class="row justify-content-center">
        <div class="col-md-10">
          <h5 class="last-heading">GAME RULES</h5>
          <p>
            THE AIM OF HATCHED AN EGG IS TO BE ONE OF THE LAST THREE PEOPLE WHO
            PURCHASED THE CORRECT BLANKET TO KEEP THE EGG WARM WHEN THE TIMER
            RUNS OUT. EACH ROUND CAN ONLY START WHEN THERE IS A MINIMUM OF 10
            ICR IN THE PRIZE POT. EACH BLANKET COSTS 1 ICR. YOU MAY PURCHASE AS
            MANY BLANKETS AS YOU’D LIKE OVER THE COURSE OF THE ROUND
          </p>
          <!-- <p>EACH BLANKET PURCHASE EXTENDS THE TIMER BY A MINIMUM OF 1 TO A MAXIMUM OF 20 MINUTES. THE EXTENSION IS RANDOMLY GENERATED BY THE SMART CONTRACT EVERY TIME A BLANKET IS PURCHASED BY ANYONE
			NOTE THAT YOU MAY NOT BUY CONCURRENT BLANKETS. YOU MAY ONLY BUY IF YOU WERE NOT THE LAST PERSON WHO BOUGHT.
			IMPORTANT NOTE: ALL BLANKET PURCHASES ARE FINAL! THERE IS ABSOLUTELY NO WAY IN WHICH WE CAN REFUND YOU FOR ANY BLANKETS PURCHASED
		<h1 class="last-heading">WHEN THE COUNTDOWN TIMER ENDS, PRICE POT BALANCE WILL BE DISTRIBUTED AS FOLLOWS:</h1>
    </p>	 -->

          <p>
            40% OF THE PRIZE POT GOES TO THE LAST PERSON WHO BOUGHT THE BLANKET.
          </p>
          <p>
            15% OF THE PRIZE POT GOES TO THE 2ND LAST PERSON WHO BOUGHT THE
            BLANKET.
          </p>
          <p>
            5% OF THE PRIZE POT GOES TO THE 3RD LAST PERSON WHO BOUGHT THE
            BLANKET.
          </p>
          <p>30% OF THE PRIZE POT GOES TO THE NEXT PRIZE POT.</p>
          <p>5% OF THE PRIZE POT IS SENT TO BURN.</p>
          <p>5% OF THE PRIZE POT IS SENT TO THE DEVELOPER.</p>
        </div>
      </div>
    </div>

    <!-- _____[TABLE CONTENT]_______ -->
    <div class="container pb-5">
      <div class="table-menu">
        <ul class="menu-inner">
          <li><a class="active" href="#">ALL</a></li>
          <li><a href="#">BIDS</a></li>
          <li><a href="#">WINS</a></li>
        </ul>
      </div>
      <div class="table-responsive">
        <table class="table mb-0">
          <thead>
            <tr>
              <th>TXN</th>
              <th>TIME</th>
              <th>WALLET</th>
              <th>TYPE</th>
              <th>AMOUNT</th>
            </tr>
          </thead>
          <tbody>
            <tr></tr>
          </tbody>
        </table>
      </div>
    </div>
</div>
</template>

<script>
export default {};
</script>

<style scoped>
/* nav menu starts */
.custom-btn {
  color: rgb(33, 40, 51);
  border-radius: 4px;
  padding: 6px 12px;
  min-height: 24px;
  border: none;
  background-image: linear-gradient(rgb(248, 209, 47) 0%,
      rgb(240, 185, 11) 100%);
  min-width: 52px;
  font-weight: 400;
  font-size: 14px;
  line-height: 20px;
}

.navbar {
  background-color: #181a20;
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
  background-color: #f0b90b;
  color: #1e2329;
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
  border-right-color: #f0b90b;
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
  color: #707a8a;
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
  background-color: #181a20;
}

.dropdown-item {
  color: #ffffff;
}

.show-hidden {
  cursor: pointer;
  color: #c99400;
  transition: all 0.3s ease-in-out;
}

.show-hidden:hover {
  color: #f0b90b;
}

.hidden-menu {
  margin-top: 10px;
  display: none;
}

/* nav menu end */




/*--------------------------------------------------------------
------------------------ Common Styling ------------------------
--------------------------------------------------------------*/
body {
  background-image: url(~/assets/images/bg-back.png);
  background-size: cover;
  padding-bottom: 5em;
  font-family:
    "sans-serif";

  color: rgb(30, 35, 41);

}

.main {
  max-width: 1440px;
  width: 100%;
  margin-left: auto;
  margin-right: auto;
}

.common-heading {
  color: #FF0101;
  font-size: 50px;
  line-height: 50px;
  margin: 0;
}

.main-heading {
  margin: 0;
  line-height: 75px;
  color: #FFD043;
  font-size: 75px;
  text-shadow: -1px 1px black;
}

p {
  font-size: 25px;
}

.banner {
  padding: 30px 0;
  margin-bottom: 40px;
}

.gaming-card {
  padding: 30px 35px;
  background: #FFFFFF 0% 0% no-repeat padding-box;
  box-shadow: 7px 0.61px 27px #04040459;
  border-radius: 10px;
  display: flex;
}

.yellow-circle {
  width: 100px;
  height: 100px;
  border-radius: 100%;
  box-shadow: 4px 0.35px 8px #04040463;
  background-color: #FFD043;
}

.card-data {
  width: 100%;
  flex: 2;
  text-align: center;
}

.card-heading {
  font-size: 20px;
}

.common-btn {
  border: none;
  padding: 15px 40px;
  border-radius: 50px;
  background: #FFBF00 0% 0% no-repeat padding-box;
  box-shadow: 7px 0.61px 27px #04040459;
}

.card-btn {
  border: none;
  padding: 15px 25px;
  margin-top: 10px;
  border-radius: 50px;
  background: #FFD043 0% 0% no-repeat padding-box;
  box-shadow: 7px 0.61px 27px #04040459;
}

.white-heading {
  padding: 35px 65px;
  background-color: #FFFFFF;
  box-shadow: 7px 0.61px 27px #04040459;
}

.balance-card {
  height: 130px;
  width: 190px;
  margin-right: 5px;
  padding: 20px 15px;
  text-align: center;
  background: #FFFFFF;
  box-shadow: 7px 0.61px 27px #04040459;
}

.table-menu {
  text-align: center;
  margin: 30px auto;
  max-width: max-content;
  padding: 30px 20px;
  border-radius: 50px;
  background: #FFFFFF;
  box-shadow: 7px 0.61px 27px #04040459;
}

.menu-inner {
  margin: 0;
  padding: 0;
  display: flex;
  align-items: center;
  justify-content: center;
}

.menu-inner li {
  list-style-type: none;
}

.menu-inner li a {
  text-decoration: none;
  margin-right: 12px;
  color: #000000;
  padding: 15px 45px;
  border-radius: 50px;
  background: #FFBF00;
  box-shadow: 3px 0.26px 18px #000000D1;
}

.menu-inner li:last-child a {
  margin-right: 0;
}

.menu-inner li a.active {
  background-color: #FF0101;
  color: #FFFFFF;
}

.table {
  background: #FFFFFF;
  box-shadow: 3px 0.26px 18px #00000099;
}

.table thead th {
  padding: 20px 10px;
  border-bottom: 1px solid #FFBF00;
  border-bottom-color: #FFBF00 !important;
}

.last-heading {
  font-size: 50px;
  margin-bottom: 10px;
  text-align: center
}

@media only screen and (max-width: 768px) {
  .table-menu {
    padding: 20px;
  }

  .menu-inner li a {
    padding: 5px 15px;
  }

  .common-heading {
    font-size: 30px;
    line-height: 40px;
  }

  .main-heading {
    font-size: 40px;
    line-height: 40px;
  }

  p {
    font-size: 18px;
  }

  .last-heading {
    font-size: 40px;
    margin-bottom: 10px;
    text-align: center
  }

  .card-btn {
    padding: 10px;
  }
}

</style>