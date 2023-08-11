<template>
  <section class="WSay">
    <div class="container">
      <div class="WSay__inner">
        <div class="WSay__about">
          <div class="WSay__desc">
            <div class="WSay__Font">
              ЧТО ХОЧЕТСЯ СКАЗАТЬ :
            </div>
            <br>
            <br>
            Количество и темпы развития важных событий в геополитике, экономике и жизни нашей страны, в последний год и месяцы быстро растут и это в любом случае отражается на жизни российского бизнеса. Кризисные ситуации в бизнесе и без того частые явления, а сегодняшняя обстановка не способствует развитию, творческому подходу или открытию чего-то нового. А это необходимо именно сейчас.
            <br>
            <br>
            Не смотря на то, что обеспечивать безопасность, рост и развитие своего бизнеса сегодня много труднее, это необходимо делать именно сейчас – развивать, искать, занимать, осваивать новые ниши.
            <br>
            <br>
            Любому человеку, бизнесмену, компании, необходимо адаптироваться уже сейчас к новым условиям и реалиям и трезво оценивать ситуацию на рынке и главное свои возможности, а их у Вас поверьте предостаточно! Если вовремя не производить анализ и диагностику новых ниш, своего бизнеса, услуг, качества управления и управляемости внутри бизнеса, не применять антикризисных мер - ситуация может оказаться необратимой.
            <br>
            <br>
            Если крупному бизнесу необходимо ускориться, то малому действовать еще быстрее, так как простой в несколько дней для маленькой компании – может оказаться губительным. Собственнику необходимо научится чувствовать все изменения в компании и вовремя проводить эффективный анализ деятельности компании, команды
          </div>
          <div class="WSay__btn">
            Отправить заявку на консультацию менеджера
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import { insertBitrix5 } from '~/assets/js/bitrx-window'
export default {
  mounted () {
    try {
      insertBitrix5('.WSay__about', '.WSay__btn')
    } catch (error) {}
  }
}
</script>

<style lang="scss" scoped>
@import '~/assets/scss/variables.scss';
.WSay {
  @include bgcenter('@/assets/images/control/aboutcompany-page/bg.png');
}
.WSay__inner{
  padding: 125px 0 207px 54px;
  .WSay__about{
    .WSay__desc{
      margin-right: auto;
      padding: 0 0 40px 0;
      width: 820px;
      font-family: $ff2;
      font-size: 20px;
      font-weight: 400;
      font-style: normal;
      line-height: 29px;
      letter-spacing: 0em;
      text-align:left;
      color: #D4D4D4;
      .WSay__Font{
          font-family: $ff2;
          font-size: 24px;
          font-weight: 400;
          line-height: 29px;
          letter-spacing: 0em;
          text-align: left;
      }
    }
    .WSay__btn{
      font-family: $ff1;
      font-style: normal;
      font-weight: 600;
      font-size: 18px;
      line-height: 33px;
      color: rgba(29, 29, 29, 0.9);
      background: #F9FF05;
      box-shadow: 0px 0px 4px rgba(0, 0, 0, 0.15);
      border-radius: 50px;
      padding: 10px 40px;
      width: fit-content;
      &:hover{
        cursor: pointer;
      }
      }
  }
}

@media (max-width: 1024px) {
  .WSay__inner {
    padding: 125px 0 185px 54px;
    .WSay__about{
      max-width: 444px;
      .WSay__title{
        padding-bottom: 25px;
      }
      .WSay__desc{
        padding-bottom: 60px;
      }
    }
    .WSay__show{
      .WSay__window{
        max-width: 480px;
      }
    }
  }
}
@media (max-width: 768px) {
  .WSay__inner{
    padding: 217px 0 202px 20px;
    column-gap: normal;
    row-gap: 59px;
    flex-wrap: wrap;
    width: 100%;
    .WSay__about{
      max-width: none;
      width: 100%;
      .WSay__title{
        padding-bottom: 21px;
      }
      .WSay__desc{
        padding-bottom: 31px;
        padding-right: 10px;
      }
    }
    .WSay__show{
        margin: 0 auto;
        padding: 0 96px;
      .WSay__btn2{
        left: 96px;
      }
    }
  }
}
@media (max-width: 480px) {
  .WSay__inner{
    padding: 82px 0 0 20px;
    row-gap: 30px;
    .WSay__about{
      .WSay__title{
        font-size: 35px;
        line-height: 55px;
      }
      .WSay__btn{
          text-align: center;
          margin-top: 83px;
        }
      .WSay__desc{
        padding-bottom: 21px;
        width: 100%;
      }
    }
    .WSay__show{
      padding: 0;
      margin: 0;
      .WSay__window{
        max-width: none;
        width: 100%;
      }
    }
  }
}
@media (max-width: 360px) {
  .WSay__inner{
    padding-bottom: 55px;
    row-gap: 45px;
    .WSay__about{
      .WSay__title{
        font-size: 30px;
        line-height: 30px;
        padding-bottom: 16;
      }
      .WSay__desc{
        padding-bottom: 19px;
      }
      .WSay__btn{
          font-size: 14px;
          line-height: 21px;
        }
    }
    .WSay__show{
      .WSay__btn2{
        right: 70px;
        .WSay__text{
          font-size: 20px;
          line-height: 24px;
        }
        .WSay__arrow{
          transform: translate(80%);
        }
      }
    }
  }
}
</style>
