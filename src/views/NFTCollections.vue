<template>
    <v-main>
        <v-container>
            <v-row>
                <v-card class="mx-auto" width="250" v-for="title1 in content">
                    <v-img v-bind:src=title1.image
                    height="250px" cover></v-img> 

                    <v-card-title>{{title1.title1}}</v-card-title>
                    <v-card-title>{{title1.title2}}</v-card-title>

                    <v-card-subtitle> {{title1.amount}} </v-card-subtitle>

                    <v-card-actions>
                        <v-btn color="orange-lighten-1" variant="text" v-bind:href=title1.marketplace target="_blank">Explore</v-btn>
                        <v-btn color="orange-lighten-1" variant="text" v-bind:href=title1.medium target="_blank">Medium</v-btn>
                    </v-card-actions>

                    <v-expand-transition>
                        <div v-show="show">
                            <v-divider></v-divider>
                            <v-card-text>{{title1.description}}</v-card-text>
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
      show: true,
      content: [
        {
            title1: "CYBERHUAHUA",
            title2: "PREMIUM",
            image: "https://nftstorage.link/ipfs/bafybeiebzxz47qwjspv262sowtzzzmqm373k76kzmgq7v3z7gy4b6q7jlm",
            amount: "49 CYBERHUAHUAS",
            marketplace: "https://www.stargaze.zone/marketplace/stars1s7uu0v6k83vw9fpfwnc0ugnplhg9uvxn3hvqg8wd678gf7dr38wsglczwg",
            medium: "https://medium.com/@aaa.metahuahua/cyberhuahua-nft-tools-story-bark-40c1329611db",
            description: "AAA MetaHuahua validator's premium ticket. This is the design of CyberHuahua, a tribute to the blockchain chihuahua and the superhero of Pop Culture.",
        },
        {
            title1: "CYBERHUAHUA",
            title2: "ZOMBIES",
            image: "https://nftstorage.link/ipfs/bafybeibfyvv5wt5lxpbarakqzadd4bviusmjd7euc72qwp6wen5qb3m4iy",
            amount: "200 ZOMBIES",
            marketplace: "https://www.stargaze.zone/marketplace/stars198yy57r6sym5tngc2xd9k2pctg9v89q36785zc2cqljukqdglalqzdf2k4",
            medium: "https://medium.com/@aaa.metahuahua/cyberhuahua-zombies-edition-e98ac50f97e0",
            description: "Flesh eating Zombies coming for our Heroes! Will you be the lucky one to mint one of the 20 Rare CyberHuahua Zombies and join the 49 Original CyberHuahuas?",
        },
        {
            title1: "TORIPUNKS",
            title2: "COLLECTION",
            image: "https://nftstorage.link/ipfs/bafybeie57ct2hb4rkg2nujc2la6yekw6z2tvfl454sl2tufn6mtslorv6y",
            amount: "10,000",
            marketplace: "https://app.teritori.com/collection/tori-tori1plr28ztj64a47a32lw7tdae8vluzm2lm7nqk364r4ws50rgwyzgsapzezt",
            medium: "https://medium.com/@aaa.metahuahua/toripunks-578167f88582",
            description: "",
        },
        {
            title1: "COMIC",
            title2: "BOOKS",
            image: "https://nftstorage.link/ipfs/bafybeia2eeejyya2357gsj5w4xuomjhfhalhjpufihjzlch4csafkrqdv4",
            amount: "3,092",
            marketplace: "https://app.teritori.com/collection/tori-tori1syx6q5rxhntng93pmk9xep25638dqy3dcnppvvytnccxrp7urt7s2570jc",
            medium: "https://medium.com/@aaa.metahuahua/toripunks-minters-winners-620278a7c761",
            description: "5 exclusive comics for minters, collect all 5 to win a portion of the Early Punks wallet rewards.",
        },
        {
            title1: "CHADPUNKS",
            title2: "COLLECTION",
            image: "https://nftstorage.link/ipfs/bafkreibfnzo3skf6srlt3zn2blq5zddxmiecwtpisu7bdhnqfzzubftx3a",
            amount: "1,000",
            marketplace: "https://app.teritori.com/collection/tori-tori1a8h38nsxu254trpfm0z65mrvguhp544mf9e36670ltm4s89y5wjq7mqevy/mint",
            medium: "https://medium.com/@aaa.metahuahua/the-chadpunks-mint-details-unveiling-the-path-to-a-thriving-ecosystem-923fbda63c48",
            description: "The ChadPunks, mysterious men in black, are group of extraordinary individuals within the ranks of the Toripunks community who come and restore faith and balance in the Teritori ecosystem.",
        },
        {
            title1: "METAHUAHUA",
            title2: "BATCH #1",
            image: "https://nftstorage.link/ipfs/bafybeihpjtqlxnbqmeefa5zjwnf4jg3vudkzd4z5a42fvtcdxw2gnd32ku",
            amount: "3,333",
            marketplace: "https://market.passage3d.com/mint/juno15yalm0qgg0wzs4etkzzputy7hum8ryzc0rrfzfplnqjeyfrpufwq9u2zwd",
            medium: "https://medium.com/@aaa.metahuahua/get-your-metahuahua-nft-and-explore-the-huahuaverse-b725ad49154d",
            description: "The Woofiest passport to the metaverse.",
        },
      ]
    }),
    //computed: {
    //    imgPath() {
    //        return require(`../assets/NFTCollections/${title1.image}`);
    //    }
    //}
  }
</script>
