<template>
  <v-row justify="center" align="center">
    <v-col cols="12" sm="8" md="6">
      <v-card class="logo py-4 d-flex justify-center">
        <NuxtLogo />
        <VuetifyLogo />
      </v-card>
      <v-card>
        <v-card-title class="headline">
          Thrilly Bot Tutorial
        </v-card-title>
        <v-card-text>
          <p>Dashboard for deploying Thrilly Bots for porno goodness</p>
          <p>
            Find a bug? Report it on the github <a
              href="https://github.com/mastashake08/thrilly-dashboard/issues"
              target="_blank"
              rel="noopener noreferrer"
              title="contribute"
            >
              issue board
            </a>.
          </p>
          <p>Thank you for developing with me and I look forward to bringing more exciting features in the future.</p>
          <div class="text-xs-right">
            <em><small>&mdash; Jyrone Parker</small></em>
          </div>
          <hr class="my-3">
          <a
            href="https://jyroneparker.com/"
            target="_blank"
            rel="noopener noreferrer"
          >
            My Website
          </a>
          <br>
          <a
            href="https://github.com/mastashake08"
            target="_blank"
            rel="noopener noreferrer"
          >
            Mastashake GitHub
          </a>
        </v-card-text>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'TutorialPage'
}
</script>
