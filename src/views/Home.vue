<template>
  <div class="home">
    <v-app>
      <v-card class="card" style="background-color: red; color: white">
        <v-card-title class="mt-10 ml-10 text-h2 font-weight-bold">
          <span>Contact</span>
        </v-card-title>
      </v-card>
      <v-row>
        <v-spacer></v-spacer>
        <v-col cols="6">
          <v-card>
            <v-card-text>
              <v-row>
                <v-col cols="6">
                  <v-text-field label="First name" outlined> </v-text-field>
                </v-col>

                <v-col cols="6">
                  <v-text-field label="Last name" outlined> </v-text-field>
                </v-col>
              </v-row>
              <v-row>
                <v-col cols="6">
                  <v-text-field label="Company name" outlined> </v-text-field>
                </v-col>

                <v-col cols="6">
                  <v-text-field label="Job title" outlined> </v-text-field>
                </v-col>
              </v-row>
              <v-row>
                <v-col cols="6">
                  <v-text-field label="Phone Number" outlined type="number">
                  </v-text-field>
                </v-col>
                <v-col cols="6">
                  <v-text-field label="Email" outlined> </v-text-field>
                </v-col>
              </v-row>
              <v-col cols="12">
                <v-text-field label="Country/Region" outlined> </v-text-field>
              </v-col>
              <v-col cols="12">
                <v-text-field label="Message" outlined> </v-text-field>
              </v-col>
              <v-btn class="btn">Send</v-btn>
            </v-card-text>
          </v-card>
        </v-col>
        <v-spacer></v-spacer>
      </v-row>
      <v-row>
        <v-col cols="12"> Developers </v-col>
      </v-row>
      <v-row>
        <v-col v-for="card in cards" :key="card.id">
          <v-card class="developer">
            <v-card-title>
              <v-spacer></v-spacer>
              {{ card.title }}
              <v-spacer></v-spacer>
            </v-card-title>
            <v-card-text>
              {{ card.text }}
            </v-card-text>
          </v-card>
          <v-card-actions>
            <v-btn plain> OK </v-btn>
          </v-card-actions>
        </v-col>
      </v-row>
      <v-footer class="footer" app dark>
        <v-row>
          &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
          &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
          <span class="text-h4"> Intelligent Digital Transformation </span
          >&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp;
          &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
          <v-item-group>
            <v-item>
              <v-btn text rounded>
                <span>CARRIERS</span>
                <v-icon color="white" size="large">mdi-account-multiple</v-icon>
              </v-btn> </v-item
            >&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;
            &nbsp;
            <v-item>
              <v-btn text rounded>
                <span>LOCATION</span>
                <v-icon size="large" color="white">mdi-map-marker</v-icon>
              </v-btn> </v-item
            >&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp;
            &nbsp;
            <v-item>
              <v-hover>
                <v-btn text rounded>
                  <span>CONNECT</span>
                  <v-icon color="white" size="large">mdi-forum </v-icon>
                </v-btn>
              </v-hover>
            </v-item>
          </v-item-group>
        </v-row>
        <v-card class="card2">
          <v-btn
            v-for="link in links"
            :key="link"
            color="white"
            text
            rounded
            class="my-100"
          >
            {{ link }}
          </v-btn>
        </v-card>
      </v-footer>
    </v-app>
  </div>
</template>

<script>
export default {
  name: "Home",
  data: () => ({
    links: [
      "Privacy Policy ",
      "Privacy Shield Notice ",
      "Terms of Service ",
      "Sustainability",
      "Modern Salavery System",
      "Employees",
      "Sitemap",
    ],
    cards: [
      {
        id: 0,
        title: "Muhammad Numan",
        text: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequatur et nulla voluptatem quae fuga, dignissimos error.",
      },
      {
        id: 1,
        title: "Muhammad Sufyan",
        text: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequatur et nulla voluptatem quae fuga, dignissimos error.",
      },
      {
        id: 2,
        title: "Muhammad Muqeet",
        text: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequatur et nulla voluptatem quae fuga, dignissimos error.",
      },
    ],
  }),
};
</script>
<style>
.card2 {
  width: 1900px;
  justify-content: center;
  margin-top: 0px;
  height: 40px;
  background: rgb(1, 1, 1);
  background: linear-gradient(
    90deg,
    rgba(1, 1, 1, 1) 25%,
    rgba(119, 3, 4, 1) 100%
  );
}
.footer {
  height: 300px;
  width: 100%;
  background: rgb(1, 1, 1);
  background: linear-gradient(
    90deg,
    rgba(1, 1, 1, 1) 25%,
    rgba(158, 21, 22, 1) 100%
  );
}
.cardheader {
  height: 200px;
  margin-top: 50px;
  justify-content: center;
  background: rgb(1, 1, 1);
  background: linear-gradient(
    90deg,
    rgba(1, 1, 1, 1) 25%,
    rgba(158, 21, 22, 1) 100%
  );
}
.card {
  height: 300px;
  width: 100%;
}
.developer {
  height: 700px;
  widows: 100%;
}
.onedev {
  height: 400px;
  width: 300px;
}
</style>
