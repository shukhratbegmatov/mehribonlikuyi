<template>
  <div>
    <Navbar></Navbar>
      <div class="container">
        <div class="homes_title">
          Mehribonlik uylari
        </div>
        <div class="row">
          <div class="col-xl-4" v-for="item in 24">
            <NuxtLink to="/home_single/12" class="home_card_link">
              <div class="home_cards">
                <div class="card_icons">
                  <svg width="55" height="54" viewBox="0 0 55 54" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <ellipse cx="27.7472" cy="27" rx="26.8419" ry="27" fill="#3734A9"/>
                    <path d="M36.1229 19.1512L35.7153 22.1442C34.6555 22.0622 33.8811 22.2809 33.392 22.8002C32.9028 23.3196 32.6039 24.0166 32.4952 24.8912C32.3865 25.7659 32.3594 26.7089 32.4137 27.7202H36.1229V36.3712H29.1529V26.0802C29.1529 23.5656 29.7779 21.6796 31.0279 20.4222C32.305 19.1649 34.0034 18.7412 36.1229 19.1512ZM25.7699 19.1512L25.3623 22.1442C24.3025 22.0622 23.5281 22.2809 23.039 22.8002C22.5498 23.3196 22.2509 24.0166 22.1422 24.8912C22.0335 25.7659 22.0064 26.7089 22.0607 27.7202H25.7699V36.3712H18.7999V26.0802C18.7999 23.5656 19.4249 21.6796 20.6749 20.4222C21.952 19.1649 23.6504 18.7412 25.7699 19.1512Z" fill="white"/>
                  </svg>
                </div>
                <div class="card_title">
                  Yuridik nomi: MEHRIBONLIK UYI № 21
                  Brend nomi: MEHRIBONLIK UYI № 21
                </div>
                <div class="home_address">
                  Manzil: O'zbekiston, 100017, Toshkent, YUNUS-OBOD TUMANI, daha KIYOT, 21
                </div>
              </div>
            </NuxtLink>
          </div>
        </div>
        <div class="button_home">
          <button>More</button>
        </div>
      </div>
    <Footer></Footer>
  </div>
</template>
