<template>
  <v-app>
    <v-row>
      <v-col cols="3">
        <v-navigation-drawer absolute permanent left>
          <template v-slot:prepend>
            <v-row class="justify-center mt-12">
              <v-avatar size="100">
                <img
                  src="https://cdn.vuetifyjs.com/images/john.jpg"
                  alt="John"
                />
              </v-avatar>
            </v-row>

            <div class="text-center mt-4 font_1">Hello, Toby</div>
          </template>

          <v-list class="mt-10" shaped dense>
            <v-list-item-group v-model="item" color="#A70026">
              <v-list-item class="font_1">
                Dashboard
              </v-list-item>
              <v-list-item class="font_1">
                Users
              </v-list-item>
              <v-list-item class="font_1">
                Communications
              </v-list-item>
              <v-list-item class="font_1">
                Settings
              </v-list-item>
            </v-list-item-group>
          </v-list>
          <template v-slot:append>
            <div>
              <v-row align="center" justify="center">
                <v-btn depressed color="white">
                  <v-icon left dark>mdi-power</v-icon>
                  Log Out
                </v-btn>
              </v-row>
            </div>
          </template>
        </v-navigation-drawer>
      </v-col>
      <v-col cols="9">
        <v-container>
          <v-row class="mt-n3">
            <v-text-field
              disabled
              label="search"
              prepend-icon="mdi-magnify"
              style="max-width: 200px;"
            ></v-text-field>
            <v-spacer />
            <v-btn class="mx-3" icon>
              <v-icon dark>mdi-bell</v-icon>
            </v-btn>
            <v-btn class="mr-7" icon>
              <v-icon>mdi-menu</v-icon>
            </v-btn>
          </v-row>
          <v-row>
            <v-col class="col-4 mt-12 mx-auto">
              <div><p class="font_2">Transcations</p></div>
              <div class="row font_3  mt-3">
                <v-btn text small>Today</v-btn>
                <v-btn text small>week</v-btn>
                <v-btn text small>Month</v-btn>
                <v-btn text small>All Time</v-btn>
              </div>
              <div class="row mt-3">
                <v-card width="300" outlined>
                  <v-card-text>
                    <p class="font_4 ">
                      Volume
                    </p>
                  </v-card-text>
                  <v-card-text>
                    <p class="font_5">
                      1230
                    </p>
                  </v-card-text>
                  <v-card-text>
                    <p class="font_6">
                      Ideal transcation no: 5000
                    </p>
                  </v-card-text>
                </v-card>
              </div>
            </v-col>
            <v-col class="col-4 mt-12 mx-auto">
              <p class="font_2">Donations</p>
              <div class="row font_3 mt-3">
                <v-btn text small>Today</v-btn>
                <v-btn text small>week</v-btn>
                <v-btn text small>Month</v-btn>
                <v-btn text small>All Time</v-btn>
              </div>
              <div class="row mt-3">
                <v-card width="300" outlined>
                  <v-card-text>
                    <p class="font_4">
                      Today
                    </p>
                  </v-card-text>
                  <v-card-text>
                    <p class="font_5">
                      200
                    </p>
                  </v-card-text>
                  <v-card-text>
                    <p class="font_6">
                      21 in the past hour
                    </p>
                  </v-card-text>
                </v-card>
              </div>
            </v-col>
            <v-col class="col-4 mx-auto">
              <div class="row">
                <v-btn text small>Today</v-btn>
                <v-btn text small>week</v-btn>
                <v-btn text small>Month</v-btn>
                <v-btn text small>All Time</v-btn>
              </div>
              <div class="row mt-3">
                <v-card width="300" color="#A70026" outlined>
                  <v-card-text>
                    <p class="font_7">
                      Wallet
                    </p>
                  </v-card-text>
                  <v-card-text>
                    <p class="font_8">
                      NGN 500,000
                    </p>
                  </v-card-text>
                </v-card>
              </div>
              <div class="row mt-5">
                <v-card width="300" color="#A70026" outlined>
                  <v-card-text>
                    <p class="font_7">
                      Users
                    </p>
                  </v-card-text>
                  <v-card-text class="ml-n4">
                    <v-list-item>
                      <v-list-item-content>
                        <span class="font_8">
                          800
                        </span>
                      </v-list-item-content>
                      <v-list-item-action>
                        <v-btn small tile class="button_font">Add User</v-btn>
                      </v-list-item-action>
                    </v-list-item>
                  </v-card-text>
                </v-card>
              </div>
            </v-col>
          </v-row>
          <div class="row mt-5 mx-auto">
            <div class="col-4">
              <div class="font_9">Recent Transcations</div>
              <v-list-item class="ml-n4" two-line>
                <v-list-item-content>
                  <v-list-item-title>NGN 100,000</v-list-item-title>
                  <v-list-item-subtitle class="credit">
                    <span class="credit"> Credit </span>
                    <span class="push">12-12-19 | 9:23am</span>
                  </v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
              <v-list-item class="ml-n4" two-line>
                <v-list-item-content>
                  <v-list-item-title>NGN 25,000</v-list-item-title>
                  <v-list-item-subtitle>
                    <span class="debit">Debit</span>
                    <span class="push">12-12-19 | 9:23am</span>
                  </v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
              <v-list-item class="ml-n4" two-line>
                <v-list-item-content>
                  <v-list-item-title>NGN 22,000</v-list-item-title>
                  <v-list-item-subtitle>
                    <span class="credit">Credit</span>
                    <span class="push">12-12-19 | 9:23am</span>
                  </v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
              <v-list-item class="ml-n4" two-line>
                <v-list-item-content>
                  <v-list-item-title>NGN 50,000</v-list-item-title>
                  <v-list-item-subtitle>
                    <span class="debit">Debit</span>
                    <span class="push">12-12-19 | 9:23am</span>
                  </v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
            </div>
            <div class="col-4 mx-auto">
              <div><p class="font_9">Recent Users</p></div>
              <v-list-item class="ml-n3">
                <v-list-item-avatar>
                  <v-img
                    src="https://cdn.vuetifyjs.com/images/lists/1.jpg"
                  ></v-img>
                </v-list-item-avatar>
                <v-list-item-content>
                  <v-list-item-title>Toby okeke</v-list-item-title>
                  <v-list-item-subtitle
                    >toby.okeke@expample.com</v-list-item-subtitle
                  >
                </v-list-item-content>
              </v-list-item>
              <v-list-item class="ml-n3">
                <v-list-item-avatar>
                  <v-img
                    src="https://cdn.vuetifyjs.com/images/lists/2.jpg"
                  ></v-img>
                </v-list-item-avatar>
                <v-list-item-content>
                  <v-list-item-title>Ugochukuwu Okafor</v-list-item-title>
                  <v-list-item-subtitle
                    >Ugochukwu.okafor@expample.com</v-list-item-subtitle
                  >
                </v-list-item-content>
              </v-list-item>
              <v-list-item class="ml-n3">
                <v-list-item-avatar>
                  <v-img
                    src="https://cdn.vuetifyjs.com/images/lists/3.jpg"
                  ></v-img>
                </v-list-item-avatar>
                <v-list-item-content>
                  <v-list-item-title>Nene kimoji</v-list-item-title>
                  <v-list-item-subtitle
                    >Nene.kimoji@expample.com</v-list-item-subtitle
                  >
                </v-list-item-content>
              </v-list-item>
              <v-list-item class="ml-n3">
                <v-list-item-avatar>
                  <v-img
                    src="https://cdn.vuetifyjs.com/images/lists/4.jpg"
                  ></v-img>
                </v-list-item-avatar>
                <v-list-item-content>
                  <v-list-item-title>Dianne Okoli</v-list-item-title>
                  <v-list-item-subtitle
                    >Dianne.okoli@expample.com</v-list-item-subtitle
                  >
                </v-list-item-content>
              </v-list-item>
              <v-list-item class="ml-n3">
                <v-list-item-avatar>
                  <v-img
                    src="https://cdn.vuetifyjs.com/images/lists/5.jpg"
                  ></v-img>
                </v-list-item-avatar>
                <v-list-item-content>
                  <v-list-item-title>Promise Lawrence</v-list-item-title>
                  <v-list-item-subtitle
                    >Promise.lawrence@expample.com</v-list-item-subtitle
                  >
                </v-list-item-content>
              </v-list-item>
            </div>
            <div class="col-4 mx-auto">
              <v-list-item>
                <v-list-item-content>
                  <span class="font_9">
                    Wallet Activity
                  </span>
                </v-list-item-content>
                <v-list-item-action>
                  <v-btn small outlined color="#7188A4" class="button_font">withdrawal</v-btn>
                </v-list-item-action>
              </v-list-item>
              <hr class="mt-2" />
              <v-list-item class="ml-n3">
                <v-list-item-avatar>
                  <v-img
                    src="https://cdn.vuetifyjs.com/images/lists/4.jpg"
                  ></v-img>
                </v-list-item-avatar>
                <v-list-item-content>
                  <v-list-item-title>NGN 4000</v-list-item-title>
                  <v-list-item-subtitle>withdrawal</v-list-item-subtitle>
                </v-list-item-content>
                <v-list-item-action>
                  <v-btn icon>
                    <v-icon color="grey lighten-1">mdi-plus</v-icon>
                  </v-btn>
                </v-list-item-action>
              </v-list-item>
              <v-list-item class="ml-n3">
                <v-list-item-avatar>
                  <v-img
                    src="https://cdn.vuetifyjs.com/images/lists/4.jpg"
                  ></v-img>
                </v-list-item-avatar>
                <v-list-item-content>
                  <v-list-item-title>NGN 3000</v-list-item-title>
                  <v-list-item-subtitle>withdrawal</v-list-item-subtitle>
                </v-list-item-content>
                <v-list-item-action>
                  <v-btn icon>
                    <v-icon color="grey lighten-1">mdi-plus</v-icon>
                  </v-btn>
                </v-list-item-action>
              </v-list-item>
              <v-list-item class="ml-n3">
                <v-list-item-avatar>
                  <v-img
                    src="https://cdn.vuetifyjs.com/images/lists/4.jpg"
                  ></v-img>
                </v-list-item-avatar>
                <v-list-item-content>
                  <v-list-item-title>NGN 5000</v-list-item-title>
                  <v-list-item-subtitle>withdrawal</v-list-item-subtitle>
                </v-list-item-content>
                <v-list-item-action>
                  <v-btn icon>
                    <v-icon color="grey lighten-1">mdi-plus</v-icon>
                  </v-btn>
                </v-list-item-action>
              </v-list-item>
              <v-list-item class="ml-n3">
                <v-list-item-avatar>
                  <v-img
                    src="https://cdn.vuetifyjs.com/images/lists/4.jpg"
                  ></v-img>
                </v-list-item-avatar>
                <v-list-item-content>
                  <v-list-item-title>NGN 5000</v-list-item-title>
                  <v-list-item-subtitle>withdrawal</v-list-item-subtitle>
                </v-list-item-content>
                <v-list-item-action>
                  <v-btn icon>
                    <v-icon color="grey lighten-1">mdi-plus</v-icon>
                  </v-btn>
                </v-list-item-action>
              </v-list-item>
              <v-list-item class="ml-n3">
                <v-list-item-avatar>
                  <v-img
                    src="https://cdn.vuetifyjs.com/images/lists/4.jpg"
                  ></v-img>
                </v-list-item-avatar>
                <v-list-item-content>
                  <v-list-item-title>NGN 1000</v-list-item-title>
                  <v-list-item-subtitle>withdrawal</v-list-item-subtitle>
                </v-list-item-content>
                <v-list-item-action>
                  <v-btn icon>
                    <v-icon color="grey lighten-1">mdi-plus</v-icon>
                  </v-btn>
                </v-list-item-action>
              </v-list-item>
            </div>
          </div>
        </v-container>
      </v-col>
    </v-row>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      item: 1,
      items: [
        { title: 'Home', icon: 'mdi-home-city' },
        { title: 'My Account', icon: 'mdi-account' },
        { title: 'Users', icon: 'mdi-account-group-outline' }
      ]
    }
  }
}
</script>

<style>
.push {
  margin-left: 100px;
}

.font_1 {
  font-family: Proxima Nova;
  color: #a70026;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 21px;
}

.font_2 {
  font-family: Wes FY;
  font-style: normal;
  font-weight: bold;
  font-size: 24px;
  line-height: 21px;
  color: #a70026;
}

.font_5 {
  font-family: Wes FY;
  font-style: normal;
  font-weight: bold;
  font-size: 36px;
  line-height: 21px;
  color: #a70026;
}
.credit {
  color: #44b8c3;
}
.debit {
  color: #a70026;
}
.font_9 {
  font-family: Wes FY;
  font-style: normal;
  font-weight: bold;
  font-size: 20px;
  line-height: 21px;
  color: #170d42;
}
.font_8 {
  font-family: Wes FY;
  font-style: normal;
  font-weight: bold;
  font-size: 36px;
  line-height: 21px;
  color: #ffffff;
}
.font_7 {
  font-family: Proxima Nova;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 21px;
  color: #ffffff;
}
.button_font {
  font-family: Proxima Nova;
  font-style: normal;
  font-weight: normal;
  font-size: 12px;
  line-height: 21px;
  color: #7188a4;
}
.font_6 {
  font-family: Proxima Nova;
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 21px;
  color: #7188a4;
}

.font_3 {
  font-family: Proxima Nova;
  font-style: normal;
  font-weight: normal;
  font-size: 12px;
  line-height: 21px;
  color: #a70026;
}

.font_4 {
  font-family: Proxima Nova;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 21px;
  color: #a70026;
}
</style>
