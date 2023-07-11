<template>
  <section
    id="welcome"
    class="hide-overflow"
  >
    <v-layout>
      <v-flex
        hidden-sm-and-down
        md6
        class="background-grad"
      >
        <v-img
          :src="require('@/assets/portifolio-img.jpeg')"
          class="style-avatar"
        /> 
      </v-flex>

      <v-flex
        xs12
        md6
        align-content-space-between
        layout
        :pa-5="$vuetify.breakpoint.smAndDown"
        wrap
      >
        <base-bubble-1
          style="transform: rotate(180deg) translateY(25%)"
        />

        <v-layout
          align-center
          justify-center
        >
          <v-flex
            xs10
            md6
          >
            <base-heading>Welcome!</base-heading>
            <base-text class="text-justify">
              Welcome, my name is Gabriel Takahashi and this is my online portfolio, below you can follow a brief 
              description about me and my professional experience!
            </base-text>
            <v-btn 
              class="info width-button"
              href="https://api.whatsapp.com/send?l=pt_BR&phone=5501299619-1600"
              target="_blank"
            > 
              Talk with me 
              <v-icon class="ml-2" dark> mdi-whatsapp </v-icon>
            </v-btn>
            

          </v-flex>
        </v-layout>

        <base-bubble-2
          style="transform: rotate(180deg) translate(-200px, -15%)"
        />
      </v-flex>
    </v-layout>
  </section>
</template>


<style scoped>
  .style-avatar {
    width: 400px;
    border-radius: 50%;
    position: relative;
    left: 15%;
    top: 15%;
  }

  .background-grad {
    background-image: linear-gradient(to bottom right, #b3d4fc, #000);
  }
  .width-button {
    width: 100%;
  }
</style>


