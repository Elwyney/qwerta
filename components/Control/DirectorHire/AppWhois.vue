<template>
  <section class="HForm">
    <div class="container">
      <div class="H__inner">
        <div class="H__about">
          <div class="H_cart">
            <div class="H__yelltext">
              «Директор может вести тактику и выиграть бой за боем, собственник — всю войну.
              Потому поберегите силы для более масштабных дел!»
            </div>
          </div>
          <div class="H_middle">
            <div class="H_left">
              <div class="H_lefttext">
                Кто такой директор?
                <br>
                Что это за человек?
                <br>
                Где его искать?
                <br>
                Как контролировать его работу?
              </div>
            </div>
            <div class="H_right">
              Это тот, кто управляет процессами и людьми!
              <br>
              Это тот, с кого мы начинаем диагностику бизнеса, (если он есть к компании).
              <br>
              Это тот, от знаний и умений которого зависит в компании все!
              <br>
              <div class="H_short">
                <br>
                Весь управленческий учет, планирование, организация, контроль, и выполнение планов зависят от него. И конечно же доходы, расходы и прибыль для собственника и бизнеса.
                <br>
              </div>
              <br>
              <b><i>Мы знаем где его искать, как отбирать и какие задачи ставить.</i></b>
              <br>
            </div>
          </div>
          <div class="H_bottom">
            Часто бывает так, что должность директора занимает сам собственник. Хорошо это или плохо — показывают цифры вашего бизнеса. Но то, что совместить в себе две серьёзные должности: учредителя и директора — точно не просто. И порой полезно отдыхать, смотреть на бизнес издалека, отходить от операционных и неотложных дел, развивать широту взгляда и стратегическое мышление.
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
  background-color: #FFFFFF;
}
.H__inner{
  padding: 75px 0 75px 0;
  .H__about{
    .H_cart{
      padding: 31px 50px 31px 50px;
      width: 920px;
      background: #FAFF00;
      border-radius: 20px;
      margin: auto;
      font-family: $ff2;
      font-style: normal;
      font-weight: 400;
      font-size: 22px;
      line-height: 26px;
      .H__yelltext{
        font-family: $ff2;
        font-style: italic;
        font-weight: 400;
        font-size: 20px;
        line-height: 24px;
        text-align: center;
        color: #1D1D1D;
      }
    }
    .H_middle{
      padding-top: 75px;
      padding-bottom: 20px;
    }
    .H_left{
      position: absolute;
      padding: 31px 50px 31px 50px;
      width: 1767px;
      background: rgb(0, 0, 0);
      border-radius: 40px;
      margin-right: auto;
      margin-left: -1315px;
      font-family: $ff2;
      font-style: normal;
      font-weight: 400;
      font-size: 22px;
      line-height: 26px;
      .H_lefttext{
        font-family: $ff1;
        margin-left: 76%;
        margin-bottom: 0px;
        font-style: normal;
        font-weight: 700;
        font-size: 28px;
        line-height: 175%;
      }
    }
    .H_right{
      padding: 15px 50px 31px 50px;
      width: 660px;
      border-radius: 20px;
      margin-left: auto;
      font-family: $ff2;
      font-style: normal;
      font-weight: 400;
      font-size: 18px;
      line-height: 160%;
      color: #1D1D1D;
      .H_short{
        line-height: 100%;
      }
    }
    .H_bottom{
      font-family: $ff2;
      font-style: normal;
      font-weight: 400;
      font-size: 20px;
      line-height: 130%;
      color: #000000;
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
    padding: 75px 0 100px 0;
    .H__about{
      .H_cart{
        width: 90%;
      }
      .H_right{
          padding: 0px 50px 31px 50px;
          width: 522px;
        }
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
  .container{
    margin-top: 152px;
  }
  .H__inner{
    padding: 100px 0 100px 0;
    row-gap: 30px;
    .H__about{
      .H__title{
        font-size: 35px;
        line-height: 55px;
      }
      .H_cart{
        // width: 390px;
        font-size: 18px;
        padding: 35px 10px 35px 10px;
        .H__yelltext{
          font-size: 18px;
        }
      }
      .H__desc{
        padding-bottom: 21px;
      }
      .H_middle{
        .H_right{
          padding: 296px 0px 31px 0px;
          width: 100%;
        }
        .H_left{
          width: 1648px;
          .H_lefttext{
            margin-left: 81%;
            font-size: 22px;
          }
        }
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
      .H_cart{
        // width: 300px;
      }
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
