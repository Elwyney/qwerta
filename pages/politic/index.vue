<template>
  <div>
    <AppWantSay />
  </div>
</template>

<script>
import AppWantSay from '~/components/Control/PoliticPage/AppWantSay.vue'
export default {
  name: 'Politic',
  components: { AppWantSay },
  head () {
    return {
      title: 'Политика конфиденциальности',
      meta: [
        {
          name: 'description',
          content: 'Политика конфиденциальности'
        }
      ]
    }
  },
  mounted () {
    this.$store.commit('bredcrumbs/changeAmountBredcrumbs', { value: 1 })
    this.$store.commit('bredcrumbs/changeBredcrumbs', {
      values: ['Политика конфиденциальности'],
      paths: ['/politic']
    })
  }
}
</script>
