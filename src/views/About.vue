<template>
  <div class="about">
    <div>
      <v-app>
        <v-app-bar dark app class="ml-16 pl-16">
          <h2>Heading</h2>
        </v-app-bar>
        <v-footer class="footer" app dark>
          <v-footer-text>
            <v-card class="cardheader">
              <v-row>
                &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
                &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
                &nbsp; &nbsp;
                <span class="text-h4"> Intelligent Digital Transformation </span
                >&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
                &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
                <v-footer-content class="test">
                  <v-item-group>
                    <v-item>
                      <v-btn text rounded>
                        <span>CARRIERS</span>
                        <v-icon color="white" size="large"
                          >mdi-account-multiple</v-icon
                        >
                      </v-btn> </v-item
                    >&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp;
                    &nbsp; &nbsp;
                    <v-item>
                      <v-btn text rounded>
                        <span>LOCATION</span>
                        <v-icon size="large" color="white"
                          >mdi-map-marker</v-icon
                        >
                      </v-btn> </v-item
                    >&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp;
                    &nbsp; &nbsp;
                    <v-item>
                      <v-hover>
                        <v-btn text rounded>
                          <span>CONNECT</span>
                          <v-icon color="white" size="large">mdi-forum </v-icon>
                        </v-btn>
                      </v-hover>
                    </v-item>
                  </v-item-group>
                </v-footer-content>
              </v-row>
            </v-card>
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
          </v-footer-text>
        </v-footer>
      </v-app>
    </div>
  </div>
</template>
<script lang="ts">
export default {
  name: "About",
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
</style>