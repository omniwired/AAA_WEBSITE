<template>
  <v-main>
    <v-container>
      <v-row>
        <v-card
          class="mx-auto"
          width="250"
          v-for="title1 in urls"
          :key="title1"
        >
          <v-img v-bind:src="title1.image" height="250" cover></v-img>

          <v-card-title>{{ title1.title1 }}</v-card-title>
          <v-card-title>{{ title1.amount }}</v-card-title>

          <v-card-subtitle> {{ title1.denom }} </v-card-subtitle>

          <v-card-actions>
            <v-btn
              color="orange-lighten-1"
              variant="text"
              v-bind:href="title1.wallet"
              target="_blank"
              >Explore</v-btn
            >
          </v-card-actions>

          <v-expand-transition>
            <div v-show="show">
              <v-divider></v-divider>
              <v-card-text>{{ title1.description }}</v-card-text>
            </div>
          </v-expand-transition>
        </v-card>
      </v-row>
    </v-container>
  </v-main>
</template>

<script setup>
import { computed, ref, onMounted } from "vue";

const show = ref(true);
const urls = ref([
  {
    title1: "PREMIUM WALLET",
    amount: "",
    url: "https://api.chihuahua.wtf/cosmos/staking/v1beta1/delegations/chihuahua1avfdl66z7ce3v6drr49s84qfdw8jwq0s6jky9v",
    denom: " $HUAHUA",
    image: "",
    wallet: "",
    description: "Test",
  },
  {
    title1: "ZOMBIES WALLET",
    amount: "",
    url: "https://rest-teritori.ecostake.com/cosmos/staking/v1beta1/delegations/tori1u0vepvps5h56l9hejccyg9x5aux3m557dl7g77",
    denom: " $TORI",
    image: "",
    wallet: "",
    description: "",
  },
  {
    title1: "PUNK GAMES",
    amount: "",
    url: "https://rest-teritori.ecostake.com/cosmos/staking/v1beta1/delegations/tori1g2nuu04v4ckhvknuadudcwz7dpefftzuud9839",
    denom: " $TORI",
    image: "",
    wallet: "",
    description: "",
  },
  {
    title1: "EARLY PUNK",
    amount: "",
    url: "https://rest-teritori.ecostake.com/cosmos/staking/v1beta1/delegations/tori1m7lst3e4e3nrgc4ftulryntstt4qx2zztvvmxh",
    denom: " $TORI",
    image: "",
    wallet: "",
    description: "",
  },
  // {
  //   title1: "METAHUAHUA LOTTERY",
  //   amount: "",
  //   url: "",
  //   denom: " $ATOM",
  //   image: "",
  //   wallet: "",
  //   description: "",
  // },
  // {
  //   title1: "METAHUAHUA METAVERSE",
  //   amount: "",
  //   url: "",
  //   denom: " $ATOM",
  //   image: "",
  //   wallet: "",
  //   description: "",
  // },
  // {
  //   title1: "METAHUAHUA MARKETING",
  //   amount: "",
  //   url: "",
  //   denom: " $ATOM",
  //   image: "",
  //   wallet: "",
  //   description: "",
  // },
  // {
  //   title1: "PASG AIRDROP",
  //   amount: "",
  //   url: "",
  //   denom: " $ATOM",
  //   image: "",
  //   wallet: "",
  //   description: "",
  // },
]);

onMounted(async () => {
  urls.value = await Promise.all(
    urls.value.map((urlObj) =>
      fetch(urlObj.url)
        .then((response) => response.json())
        .then((data) => {
          const amount = Math.floor(
            parseFloat(data.delegation_responses[0].balance.amount) / 1000000
          );
          return {
            ...urlObj,
            amount: amount,
          };
        })
        .catch((error) => console.error(error))
    )
  );
  console.log(urls.value);
});

//    {
//            name: "Wallet Zombies",
//            url: "",
//            selector: ".zombies-text-api-block",
//            denom: " $TORI",
//        },
//        {
//            name: "Wallet Punk Games Wallet",
//            url: "https://rest-teritori.ecostake.com/cosmos/staking/v1beta1/delegations/tori1g2nuu04v4ckhvknuadudcwz7dpefftzuud9839",
//            selector: ".punk-games-text-api-block",
//            denom: " $TORI",
//        },
//        {
//            name: "Wallet Early Punk Games Wallet",
//            url: "",
//            selector: ".early-punk-games-text-api-block",
//            denom: " $TORI",
//        },
//        {
//            name: "Wallet Lottery MetaHuahua",
//            url: "",
//            selector:".lottery-text-api-block",
//            denom: " $ATOM",
//        },
//        {
//            name: "Wallet Metaverse Improvement",
//            url: "https://rest.cosmos.directory/cosmoshub/cosmos/staking/v1beta1/delegations/cosmos1j3jmy29n4svhrnmqqel4x89p44u55mtzn0nfhs",
//            selector:".metaverse-text-api-block",
//            denom: " $ATOM",
//        },
//        {
//            name: "Wallet Marketing & Communication",
//            url: "https://rest.cosmos.directory/cosmoshub/cosmos/staking/v1beta1/delegations/cosmos1adxapj0y5gwlctlfh4f03weuy233l582ljlg26",
//            selector:".communication-text-api-block",
//            denom: " $ATOM",
//        },
//        {
//            name: "Wallet PASG Airdrop",
//            url: "https://rest.cosmos.directory/cosmoshub/cosmos/staking/v1beta1/delegations/cosmos1u2fslkjzcrxn3cpu8dnkd2ugy7zalja7erj9ay",
//            selector:".pasg-text-api-block",
//            denom: " $ATOM",
//        },
</script>
