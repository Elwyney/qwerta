<template>
  <div>
    <AppMain />
    <AppWhat />
    <AppWantSay />
    <AppHelp />
    <AppReseive />
    <AppPrices />
    <AppProjects />
  </div>
</template>

<script>
import AppMain from '~/components/Control/AboutCompany/AppMain.vue'
import AppWhat from '~/components/Control/AboutCompany/AppWhat.vue'
import AppWantSay from '~/components/Control/AboutCompany/AppWantSay.vue'
import AppHelp from '~/components/Control/AboutCompany/AppHelp.vue'
import AppReseive from '~/components/Control/AboutCompany/AppReseive.vue'
import AppPrices from '~/components/Control/AboutCompany/AppPrices.vue'
import AppProjects from '~/components/MainPage/AppProjects.vue'
export default {
  name: 'AboutCompanyPage',
  components: { AppMain, AppWhat, AppWantSay, AppHelp, AppReseive, AppPrices, AppProjects },
  head () {
    return {
      title: 'О компании EduPartner',
      meta: [
        {
          name: 'description',
          content: 'Узнайте больше о компании EduPartner - ведущей организации по услугам бизнес-диагностики и консалтинга. Мы специализируемся на кадровом аудите, финансовой, маркетинговой и IT-диагностике, а также диагностике управленческого учета, включая продажи. Обратитесь к нам для оптимизации вашего бизнеса и достижения новых высот. Поможем вашему бизнесу расти и развиваться! ⭐Бесплатная консультация. Звоните!☎ +7 (347) 214-51-29',
          keywords: 'Компания EduPartner-диагностики вашего предприятия: кадровый аудит, финансовая диагностика, маркетинговая и it-диагностика, диагностика управленческого учета, включая продажи. Команда высококлассных специалистов. Поможем вашему бизнесу расти и развиваться! ⭐Бесплатная консультация. Звоните!☎ +7 (347) 214-51-29'
        }
      ]
    }
  },
  mounted () {
    this.$store.commit('bredcrumbs/changeAmountBredcrumbs', { value: 1 })
    this.$store.commit('bredcrumbs/changeBredcrumbs', {
      values: ['О компании'],
      paths: ['/about-company']
    })
  }
}
</script>
