<template>
  <section
    id="about"
    class="hide-overflow"
  >
    <v-layout white>
      <v-flex
        xs12
        md6
        pa-5
      >
        <base-bubble-1
          style="transform: translate(5%, -5%)"
        />
        <base-heading class="info--text">
          About Me
        </base-heading>

        <base-text class="mb-5">
          My name is Gabriel Frederico Takahashi Vargas, I have a degree in System Analysis and Development from Fatec Jessen Vidal - SJC, I work with full-stack web development and apps for about 2 years. 
        </base-text>

        <base-subheading class="info--text">
          Skills
        </base-subheading>
        <base-text class="mb-5">
          Below is a chart ranking my skills as a software developer.
        </base-text>

        <v-alert
          outlined
          color="info"
        >
          <v-layout
            v-for="(skill, i) in skills"
            :key="i"
            style="color: #69A1BB;"
            wrap
          >
            <v-flex
              xs6
              text-uppercase
              v-text="skill.name"
            />
            <v-flex
              xs6
              text-xs-right
              v-text="`${skill.value}%`"
            />
            <v-progress-linear
              :value="skill.value"
              color="info"
              height="8"
            />
          </v-layout>
        </v-alert>
      </v-flex>
      <v-flex
        hidden-sm-and-down
        md6
      >
        <v-img
          :src="require('@/assets/aboutme.png')"
          height="100%"
        />
      </v-flex>
    </v-layout>
  </section>
</template>

<script>
export default {
  data: () => ({
    skills: [
      {
        name: 'Web Development',
        value: 100
      },
      {
        name: 'Apps',
        value: 80
      },
      {
        name: 'Web Support',
        value: 75
      },
      {
        name: 'Web Design',
        value: 50
      },
    ]
  })
}
</script>
