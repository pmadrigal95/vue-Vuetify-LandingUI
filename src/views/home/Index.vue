
<script>
  // Extensions
  import View from '@/views/View'

  // Mixins
  import LoadSections from '@/mixins/load-sections'

  export default {
    name: 'Home',

    metaInfo: { title: 'Inicio' },

    extends: View,

    mixins: [
      LoadSections([
        'hero',
        'theme-features',
        'features',
        'affiliates',
        'social-media',
        'contact-us',
      ]),
    ],

    props: {
      id: {
        type: String,
        default: 'home',
      },
    },
  }
</script>
