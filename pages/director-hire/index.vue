<template>
  <div>
    <AppSpace />
    <AppWhois />
    <AppSuccess />
    <AppStep />
    <AppWhat />
    <AppYellow />
    <AppChoose />
  </div>
</template>

<script>
import AppSpace from '~/components/Control/DirectorHire/AppSpace.vue'
import AppWhois from '~/components/Control/DirectorHire/AppWhois.vue'
import AppSuccess from '~/components/Control/DirectorHire/AppSuccess.vue'
import AppStep from '~/components/Control/DirectorHire/AppStep.vue'
import AppWhat from '~/components/Control/DirectorHire/AppWhat.vue'
import AppYellow from '~/components/Control/DirectorHire/AppYellow.vue'
import AppChoose from '~/components/MainPage/AppChoose.vue'
export default {
  name: 'DirectorHire',
  components: { AppSpace, AppWhois, AppSuccess, AppStep, AppWhat, AppYellow, AppChoose },
  head () {
    return {
      title: 'Подбор руководителя в Уфе - профессиональные услуги по подбору директоров | EduPartner',
      meta: [
        {
          name: 'description',
          content: 'Подберем и наймем высококлассного директора или руководителя для вашего отдела/компании. Наши эксперты помогут вам найти опытного и квалифицированного директора, отвечающего требованиям вашего бизнеса - сами проводим поиск, подбор, собеседования ⭐ Детальное исследование выбранного сегмента рынка⭐Бесплатная консультация. Звоните!☎ +7 (347) 214-51-29',
          keywords: 'Компания EduPartner-диагностики вашего предприятия: кадровый аудит, финансовая диагностика, маркетинговая и it-диагностика, диагностика управленческого учета, включая продажи. Команда высококлассных специалистов. Поможем вашему бизнесу расти и развиваться! ⭐Бесплатная консультация. Звоните!☎ +7 (347) 214-51-29'
        }
      ]
    }
  },
  mounted () {
    this.$store.commit('bredcrumbs/changeAmountBredcrumbs', { value: 1 })
    this.$store.commit('bredcrumbs/changeBredcrumbs', {
      values: ['Подбор директора'],
      paths: ['/director-hire']
    })
  }
}
</script>
