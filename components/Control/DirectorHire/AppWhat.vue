<template>
  <section class="WhatIn">
    <div class="container">
      <div class="WhatIn__inner">
        <div class="WhatIn__title">
          Получи скидку в 50 000 ₽ <span class="Receive__white">в мае на подбор директора</span>
        </div>
        <div class="WhatIn__cards">
          <div class="WhatIn__card">
            <div class="Visit_card">
              <div class="WhatIn__img">
                <img src="../../../assets/images/director-hire/nam.png" alt="Natalia">
              </div>
            </div>
            <div class="WhatIn__about">
              <div class="WhatIn__desc">
                Если вы, наконец-то, созрели нанять операционного директора/управляющего, мы проведём поиск, отбор кандидатов на руководящую должность.
                <br>
                <br>
                Компании, в которых мы до этого проводили диагностику бизнеса, бесплатно составим мотивацию для директора, проведём его адаптацию/введём директора в курс дел компании и будем консультировать в течение первых дней работы.
                <br>
                <div class="Whatin__righttext">
                  без скидки 190 000 ₽
                </div>
                <div class="Whatin__lefttext">
                  140 000 ₽
                </div>
                <div class="Whatin__btn">
                  Нанять директора
                </div>
              </div>
            </div>
          </div>
          <div class="Whatin__bottomtext">
            *Срок выполнения работы — от 1 недели до 1–2х месяцев. В эксклюзивных случаях позицию в топ-менеджменте закрывают за 3–5 месяцев. Такой срок обусловлиется региональностью, редкостью, и нужный кандидат может быть занят, тогда необходимо приступить к хантингу кандидата в личных переговорах
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
      insertBitrix5('.WhatIn__desc', '.Whatin__btn')
    } catch (error) {}
  }
}
</script>
<style lang="scss" scoped>
@import '~/assets/scss/variables.scss';
.WhatIn{

}
.Visit_card{
flex-direction: column;
}
.WhatIn__inner{
  padding: 100px 0;
  .WhatIn__title{
    font-family: $ff1;
    font-style: normal;
    font-weight: 600;
    font-size: 28px;
    line-height: 34px;
    color: #FAFF00;
    padding-bottom: 50px;
    .Receive__white{
      color: #FFFFFF;
    }
  }
  .WhatIn__cards{
    display: flex;
    flex-wrap: wrap;
    justify-content: flex-start;
    align-items: flex-start;
    row-gap: 50px;
    .Whatin__bottomtext{
      font-family: $ff2;
      font-style: italic;
      font-weight: 400;
      font-size: 20px;
      line-height: 130%;
      /* or 26px */
      color: #D4D4D4;
    }
    .WhatIn__card{
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
      justify-content: space-between;
      column-gap: 20px;
      width: 100%;
      .WhatIn__img{
        width: 80%;
        height: auto;
        border-radius: 50px;
        img{
          border-radius: 50px;
        }
      }
      .WhatIn__about{
        max-width: 580px;
        .WhatIn__about_Vis{
          padding: 41px 0 0 0;
          width: 251px;
        }
        .WhatIn__text{
          font-family: $ff2;
          font-style: normal;
          font-weight: 600;
          font-size: 20px;
          line-height: 24px;
          color: #FAFF00;
        }
        .WhatIn__desc{
          font-family: $ff2;
          font-style: normal;
          font-weight: 400;
          font-size: 20px;
          line-height: 24px;
          color: #D4D4D4;
          .WhatIn__desc__yell{
            color: #FAFF00;
          }
          .Whatin__righttext{
            padding: 0 45px 0 0;
            text-align: right;
            font-family: $ff1;
            font-style: normal;
            font-weight: 400;
            font-size: 25px;
            line-height: 50px;
            color: #C4C4C4;
            margin-left: 40%;
          }
          .Whatin__lefttext{
          font-family: $ff1;
          font-style: normal;
          font-weight: 700;
          font-size: 36px;
          line-height: 130%;
          /* identical to box height, or 47px */
          color: #FF004D;
          padding: 0 0 25px 0;
          }
          .Whatin__btn{
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
    }
  }
}
@media (max-width: 1024px) {
  .WhatIn__inner{
    padding: 51px 0 53px 54px;
    .WhatIn__title{
      padding-bottom: 38px;
    }
    .WhatIn__cards{
      row-gap: 24px;
      .WhatIn__card{
        .WhatIn__img{
          width: 70%;
          height: 70%;
        }
        .WhatIn__about{
          max-width: 435px;
          // .WhatIn__about_Vis{
          //   padding: 147px 0 0 0;
          //   width: 251px;
          // }
          .WhatIn__desc{
            padding: 0 0;
          }
        }
      }
    }
  }
}
@media (max-width: 768px) {
  .container{
    padding-right: 0%;
  }
  .Visit_card{
   width: 45%;
  }
  .WhatIn__inner{
    padding: 42px 0 52px 20px;
    .WhatIn__cards{
      row-gap: 35px;
      .WhatIn__card{
        column-gap: 10px;
        .WhatIn__img{
          width: 100%;
        }
        .WhatIn__about{
          width: 48%;
          .WhatIn__text{
            font-size: 22px;
            line-height: 33px;
          }
          .WhatIn__desc{
            font-size: 18px;
            line-height: 27px;
          }
        }
      }
    }
  }
}
@media (max-width: 480px) {
  .container{
    padding: 100px 0 0px 20px;
  }
  .WhatIn__inner{
    padding: 0 0 57px 0;
    .WhatIn__title{
      padding-bottom: 31px;
    }
    .WhatIn__cards{
      row-gap: 20px;
      .Visit_card{
        order:1;
      }
      .WhatIn__card{
        flex-wrap: wrap;
        row-gap: 20px;
        &:first-child{
          flex-direction: column-reverse;
        }
        .WhatIn__img{
          width: 100%;
        }
        .WhatIn__about{
          width: 100%;
          .WhatIn__desc{
            margin: auto;
          }
        }
      }
    }
  }
}
@media (max-width: 360px) {
  .WhatIn__inner{
    padding: 51px 0 48px 0;
    .WhatIn__title{
      font-size: 24px;
      line-height: 29px;
      padding-bottom: 36px;
    }
    .WhatIn__cards{
      .WhatIn__card{
        margin: auto;
        width: 80%;
        .WhatIn__img{
          width: 200%;
        }
      }
    }
  }
}
</style>
