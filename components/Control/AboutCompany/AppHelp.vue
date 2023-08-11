<template>
  <section class="HForm">
    <div class="container">
      <div class="H__inner">
        <div class="H__about">
          <div class="H_cart">
            <div class="H__yelltext">
              Помощь в управлении. Оперативки так уж нужны?
              <br>
              Когда учредитель/собственник работает директором.
            </div>
            <br>
            <br>
            Я лично и команда EduPartner поможем Вам настроить управление так, чтобы управлять было эффективно и легко!
            <br>
            Поможем расписать задачи, перейти только к важным и стратегическим, делегировать текущие дела, что приведёт к высвобождению самого дорогого ресурса в компании – времени собственника, который займется развитием бизнеса и стратегическим управлением. Увеличение выручки достаточно естественный процесс (как и уменьшение), уделяя этому должное внимание.
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
.HForm {
  @include bgcenter('@/assets/images/control/aboutcompany-page/bghelp.png');
  background-size: auto;
}
.H__inner{
  padding: 207px 0 207px 0;
  .H__about{
    .H_cart{
      padding: 35px 27px 35px 45px;
      width: 100%;
      min-height: 190px;
      background: #000000;
      border-radius: 50px;
      margin: auto;
      font-family: $ff2;
      font-style: normal;
      font-weight: 400;
      font-size: 22px;
      line-height: 26px;
      border: 1px solid #000000;
      .H__yelltext{
        font-family: $ff2;
        font-style: normal;
        font-weight: 400;
        font-size: 24px;
        line-height: 26px;
        color: #FAFF00;
      }
    }
    .H__desc{
      background: #000000;
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
      .H__Font{
          font-family: $ff2;
          font-size: 24px;
          font-weight: 400;
          line-height: 29px;
          letter-spacing: 0em;
          text-align: left;
      }
    }
    .H__btn{
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
  .H__inner {
    padding: 227px 0 185px 0;
    .H__about{
      .H__title{
        padding-bottom: 25px;
      }
      .H__desc{
        padding-bottom: 60px;
      }
    }
    .H__show{
      .H__window{
        max-width: 480px;
      }
    }
  }
}
@media (max-width: 768px) {
  .H__inner{
    padding: 217px 0 202px 0;
    column-gap: normal;
    row-gap: 59px;
    flex-wrap: wrap;
    .H__about{
      max-width: none;
      width: 100%;
      .H__title{
        padding-bottom: 21px;
      }
      .H__desc{
        padding-bottom: 31px;
      }
    }
    .H__show{
        margin: 0 auto;
        padding: 0 96px;
      .H__btn2{
        left: 96px;
      }
    }
  }
}
@media (max-width: 480px) {
  .H__inner{
    padding: 160px 0 185px 0;
    row-gap: 30px;
    .H__about{
      .H__title{
        font-size: 35px;
        line-height: 55px;
      }
      .H_cart{
        font-size: 18px;
        padding: 35px 10px 35px 10px;
        .H__yelltext{
          font-size: 18px;
        }
      }
      .H__desc{
        padding-bottom: 21px;
      }
    }
    .H__show{
      padding: 0;
      margin: 0;
      .H__window{
        max-width: none;
        width: 100%;
      }
      .H__btn2{
        left: auto;
        right: 90px;
        transform: translate(0, 70%);
        .H__text{
          text-align: right;
          padding-top: 40px;
        }
      }
    }
  }
}
@media (max-width: 360px) {
  .H__inner{
    padding-bottom: 216px;
    row-gap: 45px;
    .H__about{
      .H__title{
        font-size: 30px;
        line-height: 30px;
        padding-bottom: 16;
      }
      .H__desc{
        padding-bottom: 19px;
      }
    }
    .H__show{
      .H__btn2{
        right: 70px;
        .H__text{
          font-size: 20px;
          line-height: 24px;
        }
        .H__arrow{
          transform: translate(80%);
        }
      }
    }
  }
}
</style>
