<template>
    <v-main>
        <v-container>
            <v-row>
                <v-card class="mx-auto" width="250">
                    <v-img src="@/assets/NFTCollections/cyberhuahua_premium.png" height="250px" cover></v-img>

                    <v-card-title>PREMIUM WALLET</v-card-title>
                    <v-card-title class="premium"></v-card-title>

                    <v-card-actions>
                        <v-btn color="orange-lighten-1" variant="text" href="https://www.mintscan.io/chihuahua/account/chihuahua1avfdl66z7ce3v6drr49s84qfdw8jwq0s6jky9v" target="_blank">
                            Link
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

//urls.forEach((urlObj) => {
//    fetch(urlObj.url)
//        .then((response) => response.json())
//        .then((data) => {
//        const amount = Math.floor(
//            parseFloat(data.delegation_responses[0].balance.amount) / 1000000
//        );
//        const container = document.querySelector(urlObj.selector);
//        container.textContent = amount + urlObj.denom;
//        })
//        .catch((error) => console.error(error));
//    });
//
//    const urls = [
//    {
//        name: "Wallet Premium",
//        url: "https://api.chihuahua.wtf/cosmos/staking/v1beta1/delegations/chihuahua1avfdl66z7ce3v6drr49s84qfdw8jwq0s6jky9v",
//        selector: "premium",
//        denom: " $HUAHUA",
//    },
//    {
//        name: "Wallet Zombies",
//        url: "https://rest-teritori.ecostake.com/cosmos/staking/v1beta1/delegations/tori1u0vepvps5h56l9hejccyg9x5aux3m557dl7g77",
//        selector: ".zombies-text-api-block",
//        denom: " $TORI",
//    },
//    {
//        name: "Wallet Punk Games Wallet",
//        url: "https://rest-teritori.ecostake.com/cosmos/staking/v1beta1/delegations/tori1g2nuu04v4ckhvknuadudcwz7dpefftzuud9839",
//        selector: ".punk-games-text-api-block",
//        denom: " $TORI",
//    },
//    {
//        name: "Wallet Early Punk Games Wallet",
//        url: "https://rest-teritori.ecostake.com/cosmos/staking/v1beta1/delegations/tori1m7lst3e4e3nrgc4ftulryntstt4qx2zztvvmxh",
//        selector: ".early-punk-games-text-api-block",
//        denom: " $TORI",
//    },
//    {
//        name: "Wallet Lottery MetaHuahua",
//        url: "https://rest.cosmos.directory/cosmoshub/cosmos/staking/v1beta1/delegations/cosmos1kgmlvpn4dja9zmknms0kpsv5pw3wkvfqcx0fqf",
//        selector:".lottery-text-api-block",
//        denom: " $ATOM",
//    },
//    {
//        name: "Wallet Metaverse Improvement",
//        url: "https://rest.cosmos.directory/cosmoshub/cosmos/staking/v1beta1/delegations/cosmos1j3jmy29n4svhrnmqqel4x89p44u55mtzn0nfhs",
//        selector:".metaverse-text-api-block",
//        denom: " $ATOM",
//    },
//    {
//        name: "Wallet Marketing & Communication",
//        url: "https://rest.cosmos.directory/cosmoshub/cosmos/staking/v1beta1/delegations/cosmos1adxapj0y5gwlctlfh4f03weuy233l582ljlg26",
//        selector:".communication-text-api-block",
//        denom: " $ATOM",
//    },
//    {
//        name: "Wallet PASG Airdrop",
//        url: "https://rest.cosmos.directory/cosmoshub/cosmos/staking/v1beta1/delegations/cosmos1u2fslkjzcrxn3cpu8dnkd2ugy7zalja7erj9ay",
//        selector:".pasg-text-api-block",
//        denom: " $ATOM",
//    },
//    ];
//
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
  };
</script>

