<template>

    <v-app-bar :elevation="24" color="black">
      
      <v-container class="d-flex align-center">

        <v-img class="mx-2" nmax-height="40" max-width="40" contain src="@/assets/AppBar_Footer/aaa_community_logo.svg">
        </v-img>
        
        <v-toolbar-title class="mx-2">
          AAA Community
        </v-toolbar-title>

      </v-container>

      <v-container class="d-flex align-center">

        <v-hover v-slot:default="{ isHovering, props }">

          <v-card v-bind="props" :color="isHovering ? 'primary' : undefined">

            <v-btn to="/">
              Home
            </v-btn>

          </v-card>

        </v-hover>

        <v-hover v-slot:default="{ isHovering, props }">

          <v-card v-bind="props" :color="isHovering ? 'primary' : undefined">

            <v-btn to="/nftcollections">
              NFT Collections
            </v-btn>

          </v-card>

        </v-hover>

        <v-hover v-slot:default="{ isHovering, props }">

          <v-card v-bind="props" :color="isHovering ? 'primary' : undefined">

            <v-btn to="/communitywallets">
              Community Wallets
            </v-btn>

          </v-card>

        </v-hover>

        <v-hover v-slot:default="{ isHovering, props }">

          <v-card v-bind="props" :color="isHovering ? 'primary' : undefined">

            <v-btn href="https://app.teritori.com/dapp/tori-punks/welcome" target="_blank">
              dApp Toripunks
            </v-btn>

          </v-card>

        </v-hover>

        <v-hover v-slot:default="{ isHovering, props }">

          <v-card v-bind="props" :color="isHovering ? 'primary' : undefined">

            <v-btn to="/about">
              About
            </v-btn>

          </v-card>

        </v-hover>

      </v-container>

      <v-container class="d-flex justify-end">
        <v-img class="mx-2" nmax-height="40" max-width="40" contain src="@/assets/AppBar_Footer/keplr.svg">
        </v-img>
      </v-container>

    </v-app-bar>
    
</template>

<script>
</script>