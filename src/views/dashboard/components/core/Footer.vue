<template>
  <v-footer
    id="dashboard-core-footer"
  >
    <v-container>
      <v-row
        align="center"
        no-gutters
      >
        <!--<v-col-->
          <!--v-for="(link, i) in links"-->
          <!--:key="i"-->
          <!--class="text-center mb-sm-0 mb-5"-->
          <!--cols="auto"-->
        <!--&gt;-->
          <!--<a-->
            <!--:href="link.href"-->
            <!--class="mr-0 grey&#45;&#45;text text&#45;&#45;darken-3"-->
            <!--rel="noopener"-->
            <!--target="_blank"-->
            <!--v-text="link.text"-->
          <!--/>-->
        <!--</v-col>-->

        <v-spacer class="hidden-sm-and-down" />

        <v-col
          cols="12"
          md="auto"
        >
          <div class="body-1 font-weight-light pt-6 pt-md-0 text-center">
            Dashboard Customised
            by <v-icon
            size="18"
            color="red"
          >
            mdi-heart
          </v-icon>
            Asia R.
          </div>
        </v-col>
      </v-row>
    </v-container>
  </v-footer>
</template>

<script>
  export default {
    name: 'DashboardCoreFooter',

    data: () => ({
      links: [
        {
          href: '#',
          text: 'Creative Tim',
        },
        {
          href: '#',
          text: 'About Us',
        },
        {
          href: '#',
          text: 'Blog',
        },
        {
          href: '#',
          text: 'Licenses',
        },
      ],
    }),
  }
</script>

<style lang="sass">
  #dashboard-core-footer
    a
      font-size: .825rem
      font-weight: 500
      text-decoration: none
      text-transform: uppercase
</style>
