<template>
  <section class="WhatIn">
    <div class="container">
      <div class="WhatIn__inner">
        <div class="WhatIn__cards">
          <div class="WhatIn__card">
            <div class="Visit_card">
              <div class="WhatIn__img">
                <img src="../../../assets/images/control/aboutcompany-page/what-cards/card-01.png" alt="cards-img">
              </div>
              <div class="WhatIn__about">
                <div class="WhatIn__about_Vis">
                  <div class="WhatIn__text">
                    Мещерякова Наталья,
                  </div>
                  <div class="WhatIn__desc">
                    основатель EDUPARTNER и Приуральского центра
                  </div>
                </div>
              </div>
            </div>
            <div class="WhatIn__about">
              <div class="WhatIn__desc">
                Дорогие друзья!
                <br>
                <br>
                Я работаю в сфере образования, предпринимательства и управления с 2008 года. И это важный период моей жизни. С 2016 года исследую, изучаю и применяю различные методы и приемы в управлении. С 2017 года запущен и активно работает проект «Стажировка для выпускников» в Республике Башкортостан, за этот период прособеседовано более 3000 тысяч квалифицированных кандидатов после ВУЗов, отобрано и трудоустроено более 100 человек. На сегодняшний день под личным управлением 6 бизнесов.
                <br>
                <br>
                Вся команда EduPartner применяет современные технологии для комплексного продвижения бизнеса, как в интернет пространстве, так и для настройки эффективной работы внутри бизнеса.
                <br>
                <br>
                <div class="WhatIn__desc__yell">
                  Мы бережно и внимательно относимся к каждому собственнику и его бизнесу!
                </div>
              </div>
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
    font-weight: 700;
    font-size: 28px;
    line-height: 34px;
    color: #000000;
    padding-bottom: 91px;
  }
  .WhatIn__cards{
    display: flex;
    flex-wrap: wrap;
    justify-content: flex-start;
    align-items: flex-start;
    row-gap: 50px;
    .WhatIn__card{
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
      justify-content: space-between;
      column-gap: 20px;
      width: 100%;
      .WhatIn__img{
        width: 310px;
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
