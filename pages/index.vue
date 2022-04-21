<template>
  <div>
    <Navbar></Navbar>
    <div class="container">
      <div class="row main_page_content">
        <div class="col-xl-6">
          <div class="home_text">
            Har bir bola
            mehr va e'tiborda
          </div>
          <div class="home_description">
            Har bir bola oilada ulg‘ayish huquqiga ega
          </div>
          <div class="button_image">
            <NuxtLink to="/galery">
              Rasmlar

              <svg width="14" height="11" viewBox="0 0 14 11" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M0.5 5H12M12 5L7.5 1M12 5L7.5 9.5" stroke="white" stroke-width="2"/>
              </svg>

            </NuxtLink>
          </div>
          <div class="people_child">
            <img src="../assets/img/People.png" alt="">
          </div>
          <div class="people_title">
            Bolalarga bering dunyoni! Jami mehribonlik uylarida istiqomat qiladigan bolalar
          </div>
        </div>
        <div class="col-xl-6">
          <div class="home_image">
            <img src="../assets/img/image1.png" alt="">
          </div>
        </div>
      </div>
    </div>
    <section class="home_section">
      <div class="container">
        <div class="main_title">
          Ijtimoiy yetimlikni oldini olishda davlat va nodavlat tashkilotlari
        </div>
        <div class="section_icons">

          <div class="row">
            <div class="col-xl-2" v-for="item in 6">
              <a href="https://www.uzedu.uz/uz">
                <div class="cards">
                  <div>
                    <div>
                      <img src="../assets/img/logo-wide.png" alt="">
                    </div>
                    <div class="logo_title">
                      Халқ таълими вазирлиги
                    </div>
                  </div>
                </div>
              </a>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="container news">
      <div class="news_content">
        <div class="news_title">Yangiliklar</div>
        <div class="news_link">
          <NuxtLink to="/">Barcha yangiliklar
            <svg width="25" height="21" viewBox="0 0 25 21" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path
                d="M10.6294 1.40657L11.8681 0.33902C12.3926 -0.113007 13.2407 -0.113007 13.7596 0.33902L24.6066 9.68251C25.1311 10.1345 25.1311 10.8655 24.6066 11.3127L13.7596 20.661C13.2351 21.113 12.387 21.113 11.8681 20.661L10.6294 19.5934C10.0993 19.1366 10.1105 18.3912 10.6517 17.944L17.3753 12.4235H1.33914C0.597032 12.4235 0 11.909 0 11.2694V9.73059C0 9.09102 0.597032 8.57648 1.33914 8.57648H17.3753L10.6517 3.05599C10.1049 2.60877 10.0937 1.86341 10.6294 1.40657Z"
                fill="black"/>
            </svg>
          </NuxtLink>
        </div>
      </div>
      <div class="row">
        <div class="col-xl-4" v-for="item in 3">
          <NuxtLink class="news_f" to="/">
            <div class="news_card">
              <img src="../assets/img/news.jpg" alt="">
              <div class="news_titlee">
                "MEHR DAFTARI" TIZIMI YUZASIDAN O‘QUV-MASHG‘ULOT
              </div>
              <div class="news_date">
                5.4.2022
              </div>
            </div>
          </NuxtLink>
        </div>
      </div>
    </section>
    <section class="media_contens">
      <div class="container">
        <div class="row">
          <div class="col-xl-6">
            <div class="main_content">
              <div>
                <div class="media_title">
                  Eng qiziqarli va ta'sirchan roliklar
                </div>
                <div class="media_description">
                  Bollalarga bering dunyoni!
                </div>
                <div class="button_image">
                  <button>
                    Ko'rish
                    <svg width="14" height="11" viewBox="0 0 14 11" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path d="M0.5 5H12M12 5L7.5 1M12 5L7.5 9.5" stroke="white" stroke-width="2"/>
                    </svg>
                  </button>
                </div>
              </div>
            </div>
          </div>
          <div class="col-xl-6">
            <img class="img_home" src="../assets/img/image.png" alt="">
          </div>
        </div>
      </div>
    </section>
    <section class="statistika">
      <div class="container">
        <div class="row">
          <div class="col-xl-6">
            <div class="st_card">
              <div class="st_title">
                O’z yo’llarini topib ketgan bollalar
              </div>
              <div class="row best_people">
                <div class="col" v-for="item in 10">
                  <div class="people_best">
                    <div class="best_child">
                      <img src="../assets/img/best.png" alt="">
                    </div>
                    <div class="best_title">
                      Madina Bahromova
                    </div>
                  </div>
                </div>
              </div>
              <h5>Bugungi kungacha </h5>
              <b-progress :value="value" :max="max" show-progress></b-progress>
            </div>
          </div>
          <div class="col-xl-6">
            <div class="prosta_title">
              Mehribonlik uylari – doimiy e’tiborda
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="frends_home">
      <div class="container">
          <div class="home_title">
            Mehribonlik uylari
          </div>
      </div>
      <div>
        <VueSlickCarousel v-bind="settengs">
          <div v-for="item in 10">
            <NuxtLink to="/" class="home_card_link">
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

        </VueSlickCarousel>
      </div>
    </section>
    <section class="galery">
      <div class="container">
        <div class="galery_title">
          <div class="galery_text">
            Galeriya
          </div>
          <div class="galery_link">
            <NuxtLink to="/">Barchasi</NuxtLink>
          </div>
        </div>
        <div class="row">
          <div class="col-xl-6">
            <img src="../assets/img/image66.png" class="galery_images" alt="">
          </div>
          <div class="col-xl-6">
            <img src="../assets/img/image68.png" class="galery_images" alt="">
          </div>
          <div class="col-xl-5">
            <img src="../assets/img/image69.png" alt="" class="galery_images">
          </div>
          <div class="col-xl-2">
            <img src="../assets/img/image70.png" alt="" class="galery_images">
          </div>
          <div class="col-xl-5">
            <img src="../assets/img/image71.png" alt="" class="galery_images">
          </div>
        </div>
      </div>
    </section>
    <section class="subscribe">
      <div class="subscribe_bg">
        <div class="sb_form_gr">
          <div class="text_sb">
            Murojat uchun email yuboring
          </div>
          <div class="form_sb">
            <input type="text">
            <button>Subscribe</button>
          </div>
        </div>
      </div>
    </section>
    <Footer></Footer>
  </div>
</template>

<script>
import VueSlickCarousel from 'vue-slick-carousel'
import 'vue-slick-carousel/dist/vue-slick-carousel.css'
// optional style for arrows & dots
import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'
export default {
  name: 'IndexPage',
  data() {
    return {
      value: 45,
      max: 100,
      settengs:{
                "dots": false,
                "infinite": false,
                "speed": 500,
                "slidesToShow": 5.2,
                "slidesToScroll": 4,
                "initialSlide": 0,
                "responsive": [
                {
                  "breakpoint": 1024,
                  "settings": {
                    "slidesToShow": 3,
                    "slidesToScroll": 3,
                    "infinite": true,
                    "dots": true
                  }
                },
                {
                  "breakpoint": 600,
                  "settings": {
                    "slidesToShow": 2,
                    "slidesToScroll": 2,
                    "initialSlide": 2
                  }
                },
                {
                  "breakpoint": 480,
                  "settings": {
                    "slidesToShow": 1,
                    "slidesToScroll": 1
                  }
                }
              ]
              }
    }
  },
  components: { VueSlickCarousel }
}
</script>
