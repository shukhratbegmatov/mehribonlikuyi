<template>
  <div>
    <Navbar></Navbar>
    <div class="container">
      <div class="col-xl-12 main_images">
        <img src="../assets/img/image72.png" alt="">
      </div>
      <div class="row">
        <div class="col-xl-3 main_images" v-for="item in 24">
          <img src="../assets/img/image74.png" alt="">
        </div>
      </div>
      <div class="button_home">
        <button>More</button>
      </div>
    </div>
    <Footer></Footer>
  </div>
</template>
