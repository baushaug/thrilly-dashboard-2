<template>
  <v-row justify="center" align="center">
    <v-col cols="12" sm="8" md="6">
      <v-card class="logo py-4 d-flex justify-center">
        <NuxtLogo />
        <VuetifyLogo />
      </v-card>
      <v-card>
        <v-card-title class="headline">
          Bot Status: {{botCount}} currently running.
        </v-card-title>
        <v-card-text>
          <p>See how many bots are currently running and add/remove processes.</p>
          <p>
            Remember you are charged for proxy usage. Also too many bots running at once all of a sudden looks suspicious. Be smart.
          </p>

          </p>

        </v-card-text>
        <v-card-actions>
          <v-spacer />
          <v-btn
            color="primary"
            @click="addBot"
          >
            Add Bot
          </v-btn>

          <v-btn
            color="danger"
            @click="removeBot"
          >
            Remove Bot
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'IndexPage',
  data() {
    return {
      botCount: 0
    }
  },
  methods: {
    addBot () {
      alert('New process running on random proxy IP')
      ++this.botCount;
    },
    removeBot () {
      alert('Killing a bot process!')
      this.botCount > 0 ? --this.botCount : this.botCount = 0
    }
  }
}
</script>
