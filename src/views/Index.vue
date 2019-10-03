<template>
  <div id="index">
    <section id="video" class="fs-bg">
      <video class="fs-bg_video" playsinline autoplay muted>
        <source src="../assets/images/hero-video.mp4" type="video/mp4" />
      </video>
    </section>

    <section id="news">
      <v-container class="py-2">
        <v-row class="mt-5">
          <v-card dark max-width="344" class="mx-auto" raised elevation="20">
            <v-card-title
              class="title text-justify"
              style="word-break: break-word;"
            >
              AuctionTime.com Sets New September Record, Selling Over $75
              Million in Equipment, Trucks &amp; Trailers
            </v-card-title>

            <v-card-text>
              September 27, 2019
              <br />
              <br />In the final two-day, online-only auction for the month,
              AuctionTime.com sold more than $18 million (gross auction
              proceeds) in construction equipment, agricultural equipment,
              trucks, and trailers....
            </v-card-text>
          </v-card>

          <v-card dark max-width="344" class="mx-auto" raised elevation="20">
            <v-card-title
              class="title text-justify"
              style="word-break: break-word;"
            >
              Over $16.1 Million in Auction Goods Sold Through HiBid.com This
              Week
            </v-card-title>

            <v-card-text>
              September 24, 2019
              <br />
              <br />HiBid.com sold more than $16.1 million (gross auction
              proceeds) of equipment and other auction goods in this week’s
              online-only and webcast auctions. An average of more than 404,000
              bidders per day participated in the current week’s auctions,
              bidding on nearly 170,000 lots....
            </v-card-text>
          </v-card>

          <v-card dark max-width="344" class="mx-auto" raised elevation="20">
            <v-card-title
              class="title text-justify"
              style="word-break: break-word;"
            >
              AuctionTime.com Sells Over $21 Million in Equipment, Trucks, &amp;
              Trailers in its Biggest Two-Day Auction of 2019
            </v-card-title>

            <v-card-text>
              September 20, 2019
              <br />
              <br />In its largest auction yet this year, held September 18th
              and 19th, AuctionTime.com sold over $21 million (gross auction
              proceeds) in construction equipment, agricultural equipment,
              trucks, and trailers. More than 5,800 bidders from 49 states and
              31 countries worldwide participated in the auction, and over 2,000
              assets were sold....
            </v-card-text>
          </v-card>
        </v-row>

        <v-row>
          <div class="my-5 flex">
            <v-hover>
              <template v-slot="{ hover }">
                <v-btn
                  min-width="144px"
                  ripple
                  x-large
                  :elevation="hover ? 24 : 6"
                  >View All News</v-btn
                >
              </template>
            </v-hover>
          </div>
        </v-row>
      </v-container>
    </section>

    <section id="brands">
      <v-container class="py-2">
        <v-row class="mt-5">
          <v-card class="mx-2" max-width="250">
            <v-img class="white--text" src="../assets/images/mat.png"></v-img>
          </v-card>

          <v-card class="mx-2" max-width="250">
            <v-img class="white--text" src="../assets/images/tho.png"></v-img>
          </v-card>

          <v-card class="mx-2" max-width="250">
            <v-img class="white--text" src="../assets/images/trk.png"></v-img>
          </v-card>

          <v-card class="mx-2" max-width="250">
            <v-img class="white--text" src="../assets/images/cnt.png"></v-img>
          </v-card>

          <v-card class="mx-2" max-width="250">
            <v-img class="white--text" src="../assets/images/at.png"></v-img>
          </v-card>
        </v-row>

        <v-row>
          <div class="my-5 flex">
            <v-hover>
              <template v-slot="{ hover }">
                <v-btn
                  min-width="144px"
                  ripple
                  x-large
                  :elevation="hover ? 24 : 6"
                  >View All News</v-btn
                >
              </template>
            </v-hover>
          </div>
        </v-row>
      </v-container>
    </section>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Index"
};
</script>

<style lang="scss">
.flex {
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: center;
  align-content: flex-start;
  align-items: stretch;
}

.fs-bg {
  background: #000;
  position: relative;
  width: 100vw;
  height: 100vh;
  overflow: hidden;
  min-height: auto !important;
  .fs-bg_video {
    width: 100%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
    object-fit: fill;
  }
}

#news {
  background-image: url("../assets/images/news-bg.jpg");
  background-size: cover;
  // height: 500px;
  .theme--dark {
    background-color: hsla(0%, 0%, 0%, 0.5);
    &:hover {
      background-color: hsla(0%, 0%, 0%, 1);
    }
  }
}

#brands {
  background-image: url("../assets/images/brands-bg.jpg");
  background-size: cover;
  height: 400px;
}
</style>
