<template>
    <v-main>
        <v-container>
            <v-row>
                <v-card class="mx-auto" width="250">
                    <v-img src="@/assets/NFTCollections/cyberhuahua_premium.png" height="250px" cover></v-img>

                    <v-card-title>CYBERHUAHUA</v-card-title>
                    <v-card-title>PREMIUM</v-card-title>

                    <v-card-subtitle> 49 CYBERHUAHUAS </v-card-subtitle>

                    <v-card-actions>
                        <v-btn color="orange-lighten-1" variant="text" href="https://www.stargaze.zone/marketplace/stars1s7uu0v6k83vw9fpfwnc0ugnplhg9uvxn3hvqg8wd678gf7dr38wsglczwg" target="_blank">
                            Explore
                        </v-btn>

                        <v-spacer></v-spacer>

                        <v-btn :icon="show ? 'mdi-chevron-up' : 'mdi-chevron-down'" @click="show = !show"></v-btn>
                    </v-card-actions>
                </v-card>
            </v-row>
        </v-container>
    </v-main>
</template>

<script>

export default {
    data: () => ({
      show: false,
      show1: false,
      show2: false,
      show3: false,
      show4: false,
      show5: false,
      show6: false,
      show7: false,
    }),
  }

</script>

