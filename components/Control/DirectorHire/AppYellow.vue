<template>
  <section class="HForm">
    <div class="container">
      <div class="H__inner">
        <div class="H__about">
          <div class="H__titletext">
            Работать с нами выгодно
          </div>
          <div class="H_cart">
            <div class="H__yelltext">
              <div class="H__text">
                широкий кругозор, так как работаем с разными компаниями, в разных направлениях бизнеса, разных городах
              </div>

              <div class="H__text">
                более глубокая погруженность в Ваш бизнес, сложившийся коллектив, корпоративную культуру, по итогам проведения полной диагностики бизнеса. Обычно, после этого, происходит более целевой поиск и собственники именно нам доверяют подбор директора
              </div>
              <div class="H__text">
                в случае хантинга проще и надежнее обращаться к нам, так как искать самому неэтично
              </div>

              <div class="H__text">
                кандидаты охотно откликаются на наш бренд, так как мы российская компания и позиционируем честное, открытое и порядочное ведение бизнеса
              </div>

              <div class="H__text">
                высокая оперативность, корректировка параметров не требует дополнительного времени
              </div>

              <div class="H__text">
                стоимость услуг ниже рынка, всегда с дополнительной скидкой в 30.000–50.000 рублей после диагностики бизнеса
              </div>
            </div>
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
    .H__titletext{
        padding: 10px 0 50px 0;
        font-family: $ff1;
        font-style: normal;
        font-weight: 700;
        font-size: 28px;
        line-height: 130%;
        color: #1D1D1D;
        }
    .H_cart{
      padding: 31px 50px 31px 50px;
      width: 100%;
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
        .H__text{
        padding: 0 0 10px 40px;
        text-align: left;
        height: fit-content;
        position: relative;
        font-family: $ff2;
        font-style: normal;
        font-weight: 400;
        font-size: 20px;
        line-height: 130%;
        color: #1D1D1D;
        &::before{
          content: '\2605';
          font-size: 40px;
          position: absolute;
          top: 0px;
          left: -20px;
        }
      }
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
    padding: 227px 0 185px 0;
    .H__about{
      .H_cart{
        width: 90%;
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
    padding: 100px 20px 100px 20px;
    // margin-top: 152px;
  }
  .H__inner{
    padding: 0 0 0 0;
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
          .H__text{
            &::before{
              left: 0;
            }
          }
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
