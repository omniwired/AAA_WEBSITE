<template>
  <v-container>
    <v-row justify="space-around">
      <v-card width="400">
        <v-card-text>
          <div class="font-weight-bold ms-1 mb-2">
            Phase 1
          </div>

          <v-timeline density="compact" align="start">
            <v-timeline-item
              v-for="message in messages"
              :key="message.time"
              :dot-color="message.color"
              fill-dot
              size="x-small"
            >
              <div class="mb-4">
                <div class="font-weight-normal">
                  <strong>{{ message.from }}</strong>{{ message.time }}
                </div>
                <div>{{ message.message }}</div>
              </div>
            </v-timeline-item>
          </v-timeline>
        </v-card-text>
      </v-card>
      <v-card width="400">
        <v-card-text>
          <div class="font-weight-bold ms-1 mb-2">
            Phase 2
          </div>

          <v-timeline density="compact" align="start">
            <v-timeline-item
              v-for="message in messages1"
              :key="message.time"
              :dot-color="message.color"
              fill-dot
              size="x-small"
            >
              <div class="mb-4">
                <div class="font-weight-normal">
                  <strong>{{ message.from }}</strong>{{ message.time }}
                </div>
                <div>{{ message.message }}</div>
              </div>
            </v-timeline-item>
          </v-timeline>
        </v-card-text>
      </v-card>
      <v-card width="400">
        <v-card-text>
          <div class="font-weight-bold ms-1 mb-2">
            Phase 3
          </div>

          <v-timeline density="compact" align="start">
            <v-timeline-item
              v-for="message in messages2"
              :key="message.time"
              :dot-color="message.color"
              fill-dot
              size="x-small"
            >
              <div class="mb-4">
                <div class="font-weight-normal">
                  <strong>{{ message.from }}</strong>{{ message.time }}
                </div>
                <div>{{ message.message }}</div>
              </div>
            </v-timeline-item>
          </v-timeline>
        </v-card-text>
      </v-card>
      <v-card width="400">
        <v-card-text>
          <div class="font-weight-bold ms-1 mb-2">
            Phase 4
          </div>

          <v-timeline density="compact" align="start">
            <v-timeline-item
              v-for="message in messages3"
              :key="message.time"
              :dot-color="message.color"
              fill-dot
              size="x-small"
            >
              <div class="mb-4">
                <div class="font-weight-normal">
                  <strong>{{ message.from }}</strong>{{ message.time }}
                </div>
                <div>{{ message.message }}</div>
              </div>
            </v-timeline-item>
          </v-timeline>
        </v-card-text>
      </v-card>
    </v-row>
  </v-container>
  
</template>

<script>
  export default {
    data: () => ({
      messages: [
        {
          from: 'CYBERHUAHUA PREMIUM',
          message: `49 NFTs - Sold out`,
          time: ' - $HUAHUA',
          color: 'green-accent-3',
        },
        {
          from: 'HUAHUA VALIDATOR',
          message: `Top 20`,
          time: '',
          color: 'green-accent-3',
        },
        {
          from: 'CYBERHUAHUA ZOMBIES',
          message: `200 NFTs - Sold out`,
          time: ' - $TORI',
          color: 'green-accent-3',
        },
        {
          from: 'TERITORI VALIDATOR',
          message: `Top 10`,
          time: '',
          color: 'green-accent-3',
        },
        {
          from: 'PREMIUMS AND ZOMBIES LOTTERY',
          message: `1 draw per month`,
          time: '',
          color: 'green-accent-3',
        },
        {
          from: 'TORIPUNKS',
          message: `10,000 NFT - Sold out`,
          time: ' - $TORI',
          color: 'green-accent-3',
        },
        {
          from: 'TORIPUNKS dApp',
          message: `2 games`,
          time: '',
          color: 'green-accent-3',
        },
      ],
      messages1: [
        {
          from: '',
          message: ``,
          time: '',
          color: 'orange-darken-1',
        },
        
      ],
      messages2: [
        {
          from: '',
          message: ``,
          time: '',
          color: 'deep-orange-accent-3',
        },
        
      ],
      messages3: [
        {
          from: '',
          message: ``,
          time: '',
          color: 'deep-orange-accent-3',
        },
        
        ],
    }),
  }
</script>
<style>
</style>