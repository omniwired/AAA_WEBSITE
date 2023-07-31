<template> 
   <v-footer class="text-center d-flex flex-column" elevation="24" app="1" color="black">
        <div class="pt-0">
          Born to build a Web 3.
        </div>

        <v-divider></v-divider>
        <v-divider></v-divider>
        <v-divider></v-divider>
        <div>
        {{ new Date().getFullYear() }} — <strong>AAA Community</strong>
        </div>
        <v-divider></v-divider>
        <v-divider></v-divider>
        <v-divider></v-divider>
        <div>
          <v-container>
            <v-row :align?="center" justify="center">

              <v-col cols="auto">
                <v-btn density="default" href="https://twitter.com/AAAMetaHuahua" target="_blank">
                  <v-avatar size="x-small">
                  
                    <v-img alt="Discord" src="@/assets/AppBar_Footer/x.png"></v-img>

                  </v-avatar>
                </v-btn>  
              </v-col>

              <v-col cols="auto">
                <v-btn density="default" href="https://discord.com/invite/n6QdEXXGzP" target="_blank">
                  <v-avatar size="x-small">
                  
                    <v-img alt="Discord" src="@/assets/AppBar_Footer/discord.png"></v-img>

                  </v-avatar>
                </v-btn>  
              </v-col>

              <v-col cols="auto">
                <v-btn density="default" href="https://medium.com/@aaa.metahuahua" target="_blank">
                  <v-avatar size="x-small">
                  
                    <v-img alt="Discord" src="@/assets/AppBar_Footer/medium.png"></v-img>

                  </v-avatar>
                </v-btn>  
              </v-col>

            </v-row>
          </v-container>  
        </div>
    </v-footer>
</template>  

<script>
  export default {
    data: () => ({
      icons: [
        'mdi-discord',
        'mdi-twitter',
        'mdi-medium',
      ],
    }),
  }
</script>