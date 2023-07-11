<template>
  <section
    id="recent-projects"
    class="hide-overflow"
  >
    <v-layout>
      <v-flex
        xs12
        md6
        text-xs-center
        pa-5
      >
        
         
        <base-heading>Recent Projects!</base-heading>
        <base-text class="text-justify">
          Having participated in several business projects, I highlight the development of a
          cryptocurrency exchange, works planning system, invoice management system between
          other private projects.
        </base-text>


        <base-bubble-2
          style="transform: rotate(180deg) translate(-100px, -15%)"
        />

      </v-flex>

      <v-flex
        xs12
        md6
        primary
        text-xs-center
        pa-5
        white--text
      >
        
        <base-heading>
          Take a Look
        </base-heading>

        <base-text class="mb-5">
          Some projects for you to access.

        </base-text>

        <v-card color="secondary">
          <v-container
            grid-list-md
            pa-2
          >
            <v-layout wrap>
              <v-flex
                xs12
                md6
              >
                <a href="https://www.bitbase.com.br/#/" target="_blank">
                  <v-img
                    :src="require(`@/assets/bitbase.png`)"
                    max-height="300"
                  />
                </a>
              </v-flex>
              <v-flex
                xs12
                md6
              >
                <a href="https://fechandociclo.com.br/#/" target="_blank">
                  <v-img
                    :src="require(`@/assets/fechando.png`)"
                    max-height="300"
                  />
                </a>
              </v-flex>   
            </v-layout>
          </v-container>
        </v-card>
      </v-flex>
    </v-layout>
  </section>
</template>

<script>
export default {
  data: () => ({
    projects: [
      'project1',
      'project2',
      'project3',
      'project4'
    ]
  })
}
</script>
