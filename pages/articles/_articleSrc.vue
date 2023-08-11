<template>
  <div>
    <TheBredcrumbs />
    <AppArticle />
    <AppMightLike />
  </div>
</template>

<script>
import { mapGetters } from 'vuex'
import TheBredcrumbs from '~/components/TheBredcrumbs'
import AppArticle from '~/components/articles/AppArticle'
import AppMightLike from '~/components/articles/AppMightLike.vue'

export default {
  name: 'CorpArticle',
  components: { TheBredcrumbs, AppArticle, AppMightLike },
  computed: mapGetters('artic', ['getAllArticles']),
  mounted () {
    this.$store.commit('bredcrumbs/changeAmountBredcrumbs', { value: 2 })
    this.$store.commit('artic/setRandomCards')
  },
  unmounted () {
    this.$store.commit('bredcrumbs/hideBredcrumb')
  }
}
</script>

<style>

</style>
