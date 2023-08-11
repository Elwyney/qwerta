<template>
  <section class="Receive">
    <div class="container">
      <div class="Receive__inner">
        <div class="Receive__cards">
          <div class="Receive__card">
            <div class="Receive__title">
              Помощь в управлении
            </div>
            <br>
            <br>
            <div class="Receive__text">
              Если Вы не хотите нанимать директора, а хотите управлять бизнесом самостоятельно и при этом эффективно, предлагаю воспользоваться нашей услугой, которая заключается в помощи учредителю в настройке управленческого учета. Вместе с вами, еженедельно, я буду проводить оперативки. После оперативки у Вас будет свое видение, мнение и профессиональные рекомендации.
            </div>
            <br>
            <div class="Receive__lefttext">
              <span class="Receive__leftleft">120 000 ₽</span>
              - 40%
            </div>
            <div class="Receive__yelltext">
              72 000 ₽ в месяц
            </div>
            <div class="Receive__text">
              В рассрочку  платежей 50/50  при заключении договора на 3 мес.
            </div>
            <div class="reseive__btngroup1">
              <div class="reseive__btn1">
                Подать заявку сейчас
                <span class="reseive_right">&rarr;</span>
              </div>
              <a href="/business-diagnostics">
                <div class="reseive__btn2">
                  Все услуги для бизнеса
                  <span class="reseive_right">&rarr;</span>
                </div>
              </a>
            </div>
          </div>
          <div class="Receive__card">
            <div class="Receive__title">
              Подбор директора
            </div>
            <br>
            <br>
            <div class="Receive__text">
              Если Вы наоборот, хотите нанять операционного директора, мы проведем поиск, отбор кандидатов на должность директора/управляющего. После диагностики бизнеса, сможем провести его адаптацию/ввести в курс дел компании, познакомить со всем коллективом и консультировать в течение первых дней работы - это бесплатно оказывает только Edupartner.
            </div>
            <div class="reseive__btngroup2">
              <div class="reseive__btn1">
                Подать заявку сейчас
                <span class="reseive_right">&rarr;</span>
              </div>
              <a href="/business-diagnostics">
                <div class="reseive__btn2">
                  Цены на полную диагностику <span class="bisn">бизнеса</span>
                  <span class="reseive_right">&rarr;</span>
                </div>
              </a>
              <!-- <div class="reseive__btn2">
                Цены на подбор директора
                <span class="reseive_right">&rarr;</span>
              </div> -->
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
}
</script>
<script>
import { insertBitrix5 } from '~/assets/js/bitrx-window'
export default {
  mounted () {
    try {
      insertBitrix5('.reseive__btngroup1', '.reseive__btn1')
      insertBitrix5('.reseive__btngroup2', '.reseive__btn1')
    } catch (error) {}
  }
}
</script>
<style lang="scss" scoped>
@import '~/assets/scss/variables.scss';
.Receive{
  @include bgcenter('../../../assets/images/control/business-diag/receive_bg.png');
}
.Receive__inner{
  padding: 100px 0 85px 0;
  .Receive__title{
    font-family: $ff1;
    font-style: normal;
    font-weight: 500;
    font-size: 24px;
    line-height: 24px;
    color: #FAFF00;
    text-transform: uppercase;
  }
  .Receive__cards{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: flex-start;
    row-gap: 16px;
    column-gap: 5px;
    .Receive__card{
      height: 631px;
      padding: 35px 27px 35px 45px;
      width: 49.5%;
      min-height: 190px;
      background: linear-gradient(122.93deg, rgba(100, 100, 100, 0.71) 1.7%, rgba(72, 71, 71, 0.12) 48.4%, rgba(115, 106, 106, 0.17) 94.76%);
      border-radius: 50px;
      .Receive__text{
        height: fit-content;
        position: relative;
        font-family: $ff2;
        font-style: normal;
        font-weight: 500;
        font-size: 20px;
        line-height: 24px;
        color: #FFFFFF;
      }
      .Receive__lefttext{
        padding: 0 45px 0 0;
        text-align: right;
        font-family: $ff1;
        font-style: normal;
        font-weight: 400;
        font-size: 25px;
        line-height: 50px;
        color: #FAFF00;
        .Receive__leftleft{
          margin-right: 14px;
          text-decoration-line: line-through;
          color: #C4C4C4;
        }
      }
      .reseive_right{
        float: right;
        font-size: 33px;
      }
      .Receive__yelltext{
        font-family: $ff1;
        font-style: normal;
        font-weight: 700;
        font-size: 28px;
        line-height: 25px;
        color: #FAFF00;
      }
      .reseive__btngroup1{
        margin-top: 45px;
      }
      .reseive__btngroup2{
        margin-top: 184px;
      }
      .reseive__btn1{
        font-style: normal;
        font-weight: 500;
        font-size: 20px;
        line-height: 33px;
        color: #2E2D2C;
        margin-top: 16px;
        font-family: $ff1;
        color: rgba(29, 29, 29, 0.9);
        background: #F9FF05;
        box-shadow: 0px 0px 4px rgba(0, 0, 0, 0.15);
        border-radius: 50px;
        padding: 10px 40px;
        width: 100%;
        height: 54px;
        &:hover{
          cursor: pointer;
        }
      }
      .reseive__btn2{
        margin-top: 16px;
        font-family: $ff1;
        font-style: normal;
        font-weight: 600;
        font-size: 18px;
        line-height: 33px;
        color: #FAFF00;
        background: #181816;
        box-shadow: 0px 0px 4px rgba(0, 0, 0, 0.15);
        border: 1px solid #FAFF00;
        border-radius: 50px;
        padding: 10px 40px;
        width: 100%;
        height: 54px;
        &:hover{
          cursor: pointer;
        }
      }
    }
  }
}
@media (max-width: 1024px) {
  .Receive__inner{
    padding: 100px 0 103px 0;
    .Receive__title{
      padding-bottom: 23px;
    }
    .Receive__cards{
      row-gap: 25px;
      flex-direction: column;
      .Receive__card{
        display: flex;
        flex-direction: column;
        justify-content: flex-start;
        align-items: center;
        width: 99%;
        .Receive__text{
          font-size: 18px;
          line-height: 22px;
        }
        .reseive__btngroup1{
        margin: auto;
        }
        .reseive__btngroup2{
        margin: auto;
        }
      }
    }
  }
}

@media (max-width: 768px) {
  .Receive__inner{
    padding: 100px 0 65px 0;
    .Receive__title{
      padding-bottom: 66px;
    }
    .Receive__cards{
      column-gap: 10px;
      .Receive__card{
        width: 49%;
        min-height: 145px;
        padding: 33px 27px 33px 45px;
        .Receive__text{
          font-size: 21px;
          line-height: 26px;
          &::before{
            top: 12px;
          }
        }
      }
    }
  }
}
@media (max-width: 480px) {
  .Receive__inner{
    padding: 83px 0 65px 0;
    .Receive__title{
      padding-bottom: 42px;
    }
    .Receive__cards{
      column-gap: normal;
      row-gap: 20px;
      .Receive__card{
        width: 100%;
        padding: 35px 33px 35px 45px;
        min-height: 116px;
        .Receive__text{
          font-size: 17px;
          line-height: 24px;
          &::before{
            top: 12px;
          }
        }
        .reseive__btn1{
          font-size: 12px;
          padding: 10px 8px;
        }
        .reseive__btn2{
          font-size: 12px;
          padding: 10px 8px;
        }
        .reseive_right{
          padding: 0 0 0 40px;
        }
      }
    }
  }
}
@media (max-width: 360px) {
  .Receive__inner{
    padding:  57px 0 10px 0;
    .Receive__title{
      font-size: 24px;
      line-height: 29px;
      padding-bottom: 10px;
      text-align: center;
    }
    .Receive__cards{
      column-gap: normal;
      row-gap: 15px;
      .Receive__card{
        padding: 30px 20px 30px 20px;
        min-height: 100px;
        .Receive__text{
          font-size: 16px;
          line-height: 20px;
          &::before{
            top: 8px;
            left: -15px;
            width: 5px;
            height: 5px;
          }
        }
        .reseive__btn1{
          font-size: 16px;
          padding: 10px 9px;
        }
        .reseive__btn2{
          font-size: 16px;
          padding: 10px 9px;
        }
        .bisn{
          visibility: hidden;
        }
        .reseive_right{
          visibility: hidden;
        }
        .reseive__btngroup1{
        width: 100vw;
        height: 100vh;
        padding-right: 75px;
        }
        .reseive__btngroup2{
        width: 100vw;
        height: 100vh;
        padding-right: 75px;
        padding-top: 80px;
        }
      }
    }
  }
}
</style>
