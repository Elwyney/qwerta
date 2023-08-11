<template>
  <section class="BigTitle">
    <div class="container">
      <div class="BDiag__inner">
        <div class="BigText">
          <h1>
            EDUPARTNER
          </h1>
        </div>
        <div class="Smalltext">
          Мы занимаемся полной диагностикой малого бизнеса, услугами в области управления бизнеса, поиском и подбором персонала и топ-менеджемента. Основатель и руководитель компании предприниматель Наталья Мещерякова.
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
      insertBitrix5('.BDiag__about', '.BDiag__btn')
    } catch (error) {}
  }
}
</script>

<style lang="scss" scoped>
@import '~/assets/scss/variables.scss';
.BDiag {
  @include bgcenter('@/assets/images/control/business-diag/bg.png');
}

.Smalltext{
  padding: 140px 0 0 12px;
  width: 766px;
  font-family: $ff2;
  font-size: 20px;
  font-weight: 400;
  line-height: 24px;
  letter-spacing: 0em;
  text-align: left;
  color: #C4C908;

}
.BigText {
  font-family: $ff1;
  font-size: 150px;
  font-weight: 700;
  line-height: 110px;
  letter-spacing: 0em;
  text-align: left;
  background: linear-gradient(0deg, #34341D 0%, #C4C908 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
.BigText1 {
  font-family: $ff1;
  font-size: 150px;
  font-weight: 700;
  line-height: 110px;
  letter-spacing: 0em;
  text-align: left;
  background: linear-gradient(0deg, #dce407 0%, rgba(255, 255, 255, 0.897) 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
.BDiag__inner {
  padding: 346px 0 100px 0;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: flex-start;
  column-gap: 34px;
  .BDiag__about{
    max-width: 580px;
    .BDiag__title{
      font-family: $ff1;
      font-style: normal;
      font-weight: 700;
      font-size: 45px;
      line-height: 55px;
      color: #FFFFFF;
      padding-bottom: 37px;
    }
    .BDiag__desc{
      font-family: $ff2;
      font-style: normal;
      font-weight: 400;
      font-size: 20px;
      line-height: 24px;
      color: #D4D4D4;
      padding-bottom: 50px;
    }
    .BDiag__btn{
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
  .BDiag__show{
    position: relative;
    .BDiag__window{
      max-width: 480px;
      height: auto;
    }
    .BDiag__btn2{
      position: absolute;
      bottom: 0;
      left: 0;
      transform: translate(-30%, 70%);
      .BDiag__video{
        width: 88px;
        height: 88px;
        margin: 0 0 0 auto;
      }
      .BDiag__text{
        font-family: $ff2;
        font-style: normal;
        font-weight: 700;
        font-size: 24px;
        line-height: 29px;
        color: #FFFFFF;
        padding-top: 50px;
        span{
          color: #FAFF00;
        }
      }
      .BDiag__arrow{
        width: 76px;
        height: 87px;
        position: absolute;
        bottom: 0;
        right: 0;
        transform: translateX(100%);
      }
    }
  }
}
@media (max-width: 1024px) {
  .BDiag__inner {
    padding: 227px 0 185px 54px;
    .BigText{
      font-size: 120px;
    }
    .BDiag__about{
      max-width: 444px;
      .BDiag__title{
        padding-bottom: 25px;
      }
      .BDiag__desc{
        padding-bottom: 60px;
      }
    }
    .BDiag__show{
      .BDiag__window{
        max-width: 480px;
      }
    }
  }
}
@media (max-width: 768px) {
  .BDiag__inner{
    padding: 217px 0 202px 0;
    column-gap: normal;
    row-gap: 59px;
    flex-wrap: wrap;
    .BigText{
      font-size: 100px;
    }
    .Smalltext{
      padding: 10px 0 0 12px;
      width: 660px;
      font-family: $ff2;
      font-size: 20px;
      font-weight: 400;
      line-height: 24px;
      letter-spacing: 0em;
      text-align: left;

    }
    .BDiag__about{
      max-width: none;
      width: 100%;
      .BDiag__title{
        padding-bottom: 21px;
      }
      .BDiag__desc{
        padding-bottom: 31px;
      }
    }
    .BDiag__show{
        margin: 0 auto;
        padding: 0 96px;
      .BDiag__btn2{
        left: 96px;
      }
    }
  }
}
@media (max-width: 480px) {
  .BDiag__inner{
    padding: 217px 0 120px 0;
    row-gap: 30px;
    .BigText{
      margin: auto;
      font-size: 50px;
    }
    .Smalltext{
      margin: auto;
      width: 100%;
      padding: 0 0 0 0;
      margin: 0;
      font-size: 16px;
    }
    .BDiag__about{
      .BDiag__title{
        font-size: 35px;
        line-height: 55px;
      }
      .BDiag__desc{
        padding-bottom: 21px;
      }
    }
    .BDiag__show{
      padding: 0;
      margin: 0;
      .BDiag__window{
        max-width: none;
        width: 100%;
      }
      .BDiag__btn2{
        left: auto;
        right: 90px;
        transform: translate(0, 70%);
        .BDiag__text{
          text-align: right;
          padding-top: 40px;
        }
      }
    }
  }
}
@media (max-width: 360px) {
  .BDiag__inner{
    padding-bottom: 60px;
    row-gap: 45px;
    .BDiag__about{
      .BDiag__title{
        font-size: 30px;
        line-height: 30px;
        padding-bottom: 16;
      }
      .BDiag__desc{
        padding-bottom: 19px;
      }
    }
    .BDiag__show{
      .BDiag__btn2{
        right: 70px;
        .BDiag__text{
          font-size: 20px;
          line-height: 24px;
        }
        .BDiag__arrow{
          transform: translate(80%);
        }
      }
    }
  }
}
</style>
