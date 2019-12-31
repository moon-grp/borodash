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

            <div class="text-center mt-4">Hello, jordan</div>
          </template>

          <v-list shaped dense>
            <v-list-item-group v-model="item" color="primary">
              <v-list-item>
                Dashboard
              </v-list-item>
              <v-list-item>
                Users
              </v-list-item>
              <v-list-item>
                Communications
              </v-list-item>
              <v-list-item>
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
          <v-row>
            <v-text-field
              label="search"
              prepend-icon="mdi-magnify"
              style="max-width: 200px;"
            ></v-text-field>
            <v-spacer />
            <v-btn icon>
              <v-icon dark>mdi-bell</v-icon>
            </v-btn>
            <v-btn icon>
              <v-icon>mdi-heart</v-icon>
            </v-btn>
          </v-row>
          <v-row>
            <v-col class="col-4 mt-12 mx-auto">
              <div><p>Transcations</p></div>
              <div class="row mt-3">
                <v-btn text small>Today</v-btn>
                <v-btn text small>week</v-btn>
                <v-btn text small>Month</v-btn>
                <v-btn text small>All Time</v-btn>
              </div>
              <div class="row mt-3">
                <v-card width="300" outlined>
                  <v-card-text>
                    <p class="text--primary">
                      Volume
                    </p>
                  </v-card-text>
                  <v-card-text>
                    <p class="display-1 text--primary">
                      1230
                    </p>
                  </v-card-text>
                  <v-card-text>
                    <p class="text--primary">
                      Ideal transcation no:5000
                    </p>
                  </v-card-text>
                </v-card>
              </div>
            </v-col>
            <v-col class="col-4 mt-12 mx-auto">
              <p>Donations</p>
              <div class="row">
                <v-btn text small>Today</v-btn>
                <v-btn text small>week</v-btn>
                <v-btn text small>Month</v-btn>
                <v-btn text small>All Time</v-btn>
              </div>
              <div class="row mt-3">
                <v-card width="300" outlined>
                  <v-card-text>
                    <p class="text--primary">
                      Today
                    </p>
                  </v-card-text>
                  <v-card-text>
                    <p class="display-1 text--primary">
                      200
                    </p>
                  </v-card-text>
                  <v-card-text>
                    <p class="text--primary">
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
              <div class="row">
                <v-card width="300" outlined>
                  <v-card-text>
                    <p class="text--primary">
                      wallet
                    </p>
                  </v-card-text>
                  <v-card-text>
                    <p class="display-1 text--primary">
                      NGN 500,000
                    </p>
                  </v-card-text>
                </v-card>
              </div>
              <div class="row mt-5">
                <v-card width="300" outlined>
                  <v-card-text>
                    <p class="text--primary">
                      Users
                    </p>
                  </v-card-text>

                  <v-list-item two-line>
                    <v-list-item-content>
                      <p class="text--primary">
                        800
                      </p>
                      <v-list-item-action>
                        <v-btn icon>
                          <v-icon color="grey lighten-1"
                            >mdi-information</v-icon
                          >
                        </v-btn>
                      </v-list-item-action>
                    </v-list-item-content>
                  </v-list-item>
                </v-card>
              </div>
            </v-col>
          </v-row>
          <div class="row mt-5 mx-auto">
            <div class="col-4">
              <div>Recent Transcations</div>
              <v-list-item class="ml-n4" two-line>
                <v-list-item-content>
                  <v-list-item-title>NGN 100,000</v-list-item-title>
                  <v-list-item-subtitle>
                    Credit
                    <span class="push">12-12-19 | 9:23am</span>
                  </v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
              <v-list-item class="ml-n4" two-line>
                <v-list-item-content>
                  <v-list-item-title>NGN 25,000</v-list-item-title>
                  <v-list-item-subtitle>
                    Debit
                    <span class="push">12-12-19 | 9:23am</span>
                  </v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
              <v-list-item class="ml-n4" two-line>
                <v-list-item-content>
                  <v-list-item-title>NGN 22,000</v-list-item-title>
                  <v-list-item-subtitle>
                    Credit
                    <span class="push">12-12-19 | 9:23am</span>
                  </v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
              <v-list-item class="ml-n4" two-line>
                <v-list-item-content>
                  <v-list-item-title>NGN 50,000</v-list-item-title>
                  <v-list-item-subtitle>
                    Debit
                    <span class="push">12-12-19 | 9:23am</span>
                  </v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
            </div>
            <div class="col-4 mx-auto">
              <div><p>Recent Users</p></div>
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
              <div><p>Wallet Activity</p></div>
              <hr />
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
                    <v-icon color="grey lighten-1">mdi-information</v-icon>
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
                    <v-icon color="grey lighten-1">mdi-information</v-icon>
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
                    <v-icon color="grey lighten-1">mdi-information</v-icon>
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
                    <v-icon color="grey lighten-1">mdi-information</v-icon>
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
                    <v-icon color="grey lighten-1">mdi-information</v-icon>
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
</style>
