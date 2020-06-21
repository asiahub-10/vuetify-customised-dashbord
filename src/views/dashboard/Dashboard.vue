<template>
  <v-container
    id="dashboard"
    fluid
    tag="section"
  >
    <v-row>
      <v-col cols="12">
        <v-card
          class="card"
        >
          <v-img
            src="../../assets/pngfuel.png"
            width="100%"
            max-height="auto"
            class="image"
          >
            <v-row>
              <v-col
                cols="12"
                lg="6"
                md="8"
                sm="10"
                class="mx-auto"
              >
                <v-card
                  class="py-5 px-5 overlay"
                >
                  <v-row>
                    <v-col
                      cols="12"
                      md="6"
                      sm="12"
                      class="text-center"
                    >
                      <v-icon
                        class="top-icon"
                      >
                        <!--{{ icons.clients }}-->
                        mdi-account-supervisor-circle
                      </v-icon>
                      <h1 class="">Clients</h1>
                      <p class="number">101</p>
                      <v-btn
                        class="btn mx-auto"
                      >
                        <v-icon>
                          mdi-eye
                        </v-icon>
                        <span class="ml-2">View Details</span>
                      </v-btn>
                    </v-col>
                    <v-col
                      cols="12"
                      md="6"
                      class="text-center"
                    >
                      <v-icon
                        class="top-icon"
                      >
                        <!--{{ icons.invitation }}-->
                        mdi-alert-octagon
                      </v-icon>
                      <h1 class="">Invitation Pending</h1>
                      <p class="number">302</p>
                      <v-btn
                        class="btn mx-auto"
                      >
                        <v-icon>
                          mdi-eye
                        </v-icon>
                        <span class="ml-2">View Details</span>
                      </v-btn>
                    </v-col>
                    <v-col
                      cols="12"
                      class="px-5"
                    >
                      <v-text-field
                        label="Search"
                        color="white"
                        append-icon="mdi-magnify"
                        dark
                      >
                      </v-text-field>
                      <!--<v-btn-->
                        <!--class="btn-search transparent mt-4 mr-0"-->
                        <!--elevation="1"-->
                        <!--fab-->
                        <!--small-->
                      <!--&gt;-->
                        <!--<v-icon-->
                          <!--color="#fff"-->
                          <!--size="x-large"-->
                        <!--&gt;-->
                          <!--mdi-magnify-->
                        <!--</v-icon>-->
                      <!--</v-btn>-->
                    </v-col>
                  </v-row>
                </v-card>
              </v-col>
            </v-row>
          </v-img>
        </v-card>
      </v-col>

      <v-col
        cols="12"
        sm="6"
        class="mb-10"
      >
        <v-card
          class="custom-card px-5 py-5 info-img"
        >
          <v-icon
            color="#fff"
            icon="mdi-account-cog"
            class="icon bg-info"
          >
            mdi-account-cog
          </v-icon>
          <h1 class="text-muted">KYC Approvals Pending</h1>
          <p class="number mb-0 text-dark">+245</p>
        </v-card>
      </v-col>

      <v-col
        cols="12"
        sm="6"
        class="mb-10"
      >
        <v-card
          class="custom-card pink-img px-5 py-5"
        >
          <v-icon
            color="#fff"
            :icon="icons.check"
            class="icon bg-pink"
          >
            {{ icons.check }}
          </v-icon>
          <h1 class="text-muted">Suitability Approvals Pending</h1>
          <p class="number mb-0 text-dark">75.521</p>
        </v-card>
      </v-col>

      <v-col
        cols="12"
        sm="6"
        class="mb-10"
      >
        <v-card
          class="custom-card green-img px-5 py-5"
        >
          <v-icon
            color="#fff"
            icon="mdi-cash-usd-outline"
            class="icon bg-green"
          >
            mdi-cash-usd-outline
          </v-icon>
          <h1 class="text-muted">Indication of Interest</h1>
          <p class="number mb-0 text-dark">$ 34,245</p>
        </v-card>
      </v-col>

      <v-col
        cols="12"
        sm="6"
        class="mb-10"
      >
        <v-card
          class="custom-card orange-img px-5 py-5"
        >
          <v-icon
            color="#fff"
            icon="mdi-inbox-arrow-down"
            class="icon bg-orange"
          >
            mdi-inbox-arrow-down
          </v-icon>
          <h1 class="text-muted">Transaction Pending</h1>
          <p class="number mb-0 text-dark">184</p>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  export default {
    name: 'DashboardDashboard',

    data () {
      return {
        icons: {
          clients: 'mdi-account-group',
          arrowRight: 'mdi-arrow-right',
          invitation: 'mdi-account-alert',
          magnify: 'mdi-magnify',
          kyc: 'mdi-account-cog',
          check: 'mdi-bookmark-check',
        },
      }
    },
  }
</script>

<style scoped>
  .card {
    /*box-shadow: 0px 3px 1px -2px rgba(0, 0, 0, 0.2), 0px 2px 2px 0px rgba(0, 0, 0, 0.14), 0px 1px 5px 0px rgba(0, 0, 0, 0.12);*/
    padding: 20px !important;
    /*border-radius: 5px;*/
    background-image: linear-gradient(to right, #363855 , #2c2f49) !important;
  }
  .image {
    display: flex !important;
    justify-content: center !important;
    align-items: center !important;
  }
  .number {
    font-size: 25px !important;
    font-weight: bold !important;
  }
  .btn {
    border-radius: 50px !important;
    text-decoration: none !important;
  }
  /*.btn-search {*/
    /*box-shadow: none !important;*/
  /*}*/
  /*.stats {*/
    /*box-shadow: none !important;*/
    /*background: transparent;*/
  /*}*/
  /*.stats hr {*/
    /*background: transparent !important;*/
  /*}*/
  .custom-card {
    /*background: #fb8c00;*/
    background-size: cover !important;
    background-repeat: no-repeat !important;
    background-position: right top !important;
    height: 100% !important;
  }
  .text-muted {
    color: #9e9e9e !important;
    font-weight: 500 !important;
  }
  .text-dark {
    color: rgba(0, 0, 0, 0.7) !important;
  }
  /*.v-card .v-divider {*/
    /*border-color: red !important;*/
  /*}*/
  .v-divider {
    /*display: none !important;*/
  }
  /*box-shadow: 0px 3px 5px -1px rgba(0, 0, 0, 0.2), 0px 6px 10px 0px rgba(0, 0, 0, 0.14), 0px 1px 18px 0px rgba(0, 0, 0, 0.12) !important;*/
  .icon {
    padding: 28px !important;
    font-size: 35px !important;
    border-radius: 5px !important;
    box-shadow: 0px 3px 5px -1px rgba(0, 0, 0, 0.2), 0px 6px 10px 0px rgba(0, 0, 0, 0.14), 0px 1px 18px 0px rgba(0, 0, 0, 0.12) !important;
    margin-bottom: 30px !important;
    margin-top: -37px !important;
  }
  h1 {
    font-weight: 400 !important;
    font-size: 18px !important;
  }
  .top-icon {
    font-size: 40px !important;
    color: rgba(255, 255, 255, 0.8) !important;
  }
  .overlay {
    background: rgba(32, 35, 61, 0.85) !important;
  }
  .overlay h1 {
    color: rgba(255, 255, 255, 0.5) !important;
  }
  .overlay .number {
    color: rgba(255, 255, 255, 0.8) !important;
    font-size: 32px !important;
  }
  .overlay .btn {
    background-color: transparent !important;
    border: 1px solid white !important;
  }
  .bg-info {
    background: #00cae3 !important;
  }
  .bg-pink {
    background: #e91e63 !important;
  }
  .bg-green {
    background: #4caf50 !important;
  }
  .bg-orange {
    background: #fb8c00 !important;
  }
  .info-img {
    background-image: url("../../assets/info.png") !important;
  }
  .pink-img {
    background-image: url("../../assets/pink.png") !important;
  }
  .green-img {
    background-image: url("../../assets/green.png") !important;
  }
  .orange-img {
    background-image: url("../../assets/orange.png") !important;
  }
  /*#settings {*/
    /*z-index: -10;*/
  /*}*/
</style>
