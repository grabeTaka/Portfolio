<template>
  <div>
    <v-btn
      v-for="(item, i) in items.slice(0, large ? items.length : 3)"
      :key="i"
      fab
      class="ma-2"
      :large="large"
      color="info"
      :href="item.ref"
      target="_blank"
    >
      <v-icon
        dark
        v-text="item.icon"
      />
    </v-btn>
  </div>
</template>

<script>
export default {
  props: {
    large: {
      type: Boolean,
      default: false
    }
  },

  data: () => ({
    items: [
      {
        name: 'Whatsapp',
        icon: 'mdi-whatsapp',
        ref: 'https://api.whatsapp.com/send?l=pt_BR&phone=5501299619-1600'

      },
      {
        name: 'Linkdedin',
        icon: 'mdi-linkedin',
        ref: 'https://www.linkedin.com/in/gabriel-takahashi-754802152/'
      },
      {
        name: 'Github',
        icon: 'mdi-github-circle',
        ref: 'https://github.com/GabrielTaka'
      }
    ]
  })
}
</script>
