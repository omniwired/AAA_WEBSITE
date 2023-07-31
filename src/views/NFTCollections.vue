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

                    <v-expand-transition>
                        <div v-show="show">
                            <v-divider></v-divider>

                            <v-card-text>
                                AAA MetaHuahua validator's premium ticket. This is the design of CyberHuahua, a tribute to the blockchain chihuahua and the superhero of Pop Culture.
                            </v-card-text>
                        </div>
                    </v-expand-transition>
                </v-card>
                <v-card class="mx-auto" width="250">
                    <v-img src="@/assets/NFTCollections/cyberhuahua_zombies.png" height="250px" cover></v-img>

                    <v-card-title>CYBERHUAHUA</v-card-title>
                    <v-card-title>ZOMBIES</v-card-title>

                    <v-card-subtitle> 200 ZOMBIES </v-card-subtitle>

                    <v-card-actions>
                        <v-btn color="orange-lighten-1" variant="text" href="https://www.stargaze.zone/marketplace/stars198yy57r6sym5tngc2xd9k2pctg9v89q36785zc2cqljukqdglalqzdf2k4" target="_blank">
                            Explore
                        </v-btn>

                        <v-spacer></v-spacer>

                        <v-btn :icon="show1 ? 'mdi-chevron-up' : 'mdi-chevron-down'" @click="show1 = !show1"></v-btn>
                    </v-card-actions>

                    <v-expand-transition>
                        <div v-show="show1">
                            <v-divider></v-divider>

                            <v-card-text>
                                Flesh eating Zombies coming for our Heroes! Will you be the lucky one to mint one of the 20 Rare CyberHuahua Zombies and join the 49 Original CyberHuahuas?
                            </v-card-text>
                        </div>
                    </v-expand-transition>
                </v-card>
                <v-card class="mx-auto" width="250">
                    <v-img src="@/assets/NFTCollections/toripunks.png" height="250px" cover></v-img>

                    <v-card-title>TORIPUNKS</v-card-title>
                    <v-card-title>COLLECTION</v-card-title>

                    <v-card-subtitle> 10,000 TORIPUNKS </v-card-subtitle>

                    <v-card-actions>
                        <v-btn color="orange-lighten-1" variant="text" href="https://app.teritori.com/collection/tori-tori1plr28ztj64a47a32lw7tdae8vluzm2lm7nqk364r4ws50rgwyzgsapzezt" target="_blank">
                            Explore
                        </v-btn>

                        <v-spacer></v-spacer>

                        <v-btn :icon="show2 ? 'mdi-chevron-up' : 'mdi-chevron-down'" @click="show2 = !show2"></v-btn>
                    </v-card-actions>

                    <v-expand-transition>
                        <div v-show="show2">
                            <v-divider></v-divider>

                            <v-card-text>
                                #WeAreToriPunks
                            </v-card-text>
                        </div>
                    </v-expand-transition>
                </v-card>
                <v-card class="mx-auto" width="250">
                    <v-img src="@/assets/NFTCollections/comic_books.png" height="250px" cover></v-img>

                    <v-card-title>COMIC</v-card-title>
                    <v-card-title>BOOKS</v-card-title>

                    <v-card-subtitle> 3092 COMICS </v-card-subtitle>

                    <v-card-actions>
                        <v-btn color="orange-lighten-1" variant="text" href="https://app.teritori.com/collection/tori-tori1syx6q5rxhntng93pmk9xep25638dqy3dcnppvvytnccxrp7urt7s2570jc" target="_blank">
                            Explore
                        </v-btn>

                        <v-spacer></v-spacer>

                        <v-btn :icon="show3 ? 'mdi-chevron-up' : 'mdi-chevron-down'" @click="show3 = !show3"></v-btn>
                    </v-card-actions>

                    <v-expand-transition>
                        <div v-show="show3">
                            <v-divider></v-divider>

                            <v-card-text>
                                5 exclusive comics for minters, collect all 5 to win a portion of the Early Punks wallet rewards.
                            </v-card-text>
                        </div>
                    </v-expand-transition>
                </v-card>
                
            </v-row>
        </v-container>
        <v-container>
            <v-row>
                <v-card class="mx-auto" width="250">
                    <v-img src="@/assets/NFTCollections/chadpunks.png" height="250px" cover></v-img>

                    <v-card-title>CHADPUNKS</v-card-title>
                    <v-card-title>COLLECTION</v-card-title>

                    <v-card-subtitle> 1,000 CHADS </v-card-subtitle>

                    <v-card-actions>
                        <v-btn color="orange-lighten-1" variant="text" href="https://app.teritori.com/collection/tori-tori1a8h38nsxu254trpfm0z65mrvguhp544mf9e36670ltm4s89y5wjq7mqevy/mint" target="_blank">
                            Explore
                        </v-btn>

                        <v-spacer></v-spacer>

                        <v-btn :icon="show4 ? 'mdi-chevron-up' : 'mdi-chevron-down'" @click="show4 = !show4"></v-btn>
                    </v-card-actions>

                    <v-expand-transition>
                        <div v-show="show4">
                            <v-divider></v-divider>

                            <v-card-text>
                                The ChadPunks, mysterious men in black, are group of extraordinary individuals within the ranks of the Toripunks community who come and restore faith and balance in the Teritori ecosystem.
                            </v-card-text>
                        </div>
                    </v-expand-transition>
                </v-card>
                <v-card class="mx-auto" width="250">
                    <v-img src="@/assets/NFTCollections/metahuahua.png" height="250px" cover></v-img>

                    <v-card-title>METAHUAHUA</v-card-title>
                    <v-card-title>BATCH #1</v-card-title>

                    <v-card-subtitle> 3,333 METAHUAHUAS </v-card-subtitle>

                    <v-card-actions>
                        <v-btn color="orange-lighten-1" variant="text" href="https://market.passage3d.com/mint/juno15yalm0qgg0wzs4etkzzputy7hum8ryzc0rrfzfplnqjeyfrpufwq9u2zwd" target="_blank">
                            Explore
                        </v-btn>

                        <v-spacer></v-spacer>

                        <v-btn :icon="show5 ? 'mdi-chevron-up' : 'mdi-chevron-down'" @click="show5 = !show5"></v-btn>
                    </v-card-actions>

                    <v-expand-transition>
                        <div v-show="show5">
                            <v-divider></v-divider>

                            <v-card-text>
                                The Woofiest passport to the metaverse.
                            </v-card-text>
                        </div>
                    </v-expand-transition>
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
