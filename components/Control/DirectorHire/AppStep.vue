<template>
  <section class="Step">
    <div class="container">
      <div class="Step__inner">
        <div class="Step__title">
          Этапы работы
        </div>
        <div class="Step__cards">
          <div class="Step__cardgr">
            <div class="Step__card">
              <div class="Step__img">
                <img src="../../../assets/images/director-hire/Vc1r1.png" alt="Rodoslovnaya">
              </div>
              <div class="Step__text">
                <span class="Step__textl">Договор, предоплата, формирование портрета кандидата</span>
                <br>
                <br>
                Формирование более детального и проработанного портрета кандидата, отвечающего бизнес-целям компании и особенностям корпоративной культуры (при предварительно проведенной полной диагностики вашего бизнеса – мы самостоятельно готовим этот этап. В иных случаях – это глубокий и подробный бриф вместе с заказчиком).
              </div>
            </div>
            <div class="Step__card">
              <div class="Step__img">
                <img src="../../../assets/images/director-hire/Vc1r2.png" alt="Rodoslovnaya">
              </div>
              <div class="Step__text">
                <span class="Step__textl">Гарантия переподбора</span>
                <br>
                <br>
                Гарантированно, бесплатно делаем еще один переподбор, при увольнении директора по Вашей инициативе в течение первых 3х месяцев.
              </div>
            </div>
          </div>
          <div class="Step__cardgr">
            <div class="Step__card">
              <div class="Step__img">
                <img src="../../../assets/images/director-hire/Vc2r1.png" alt="Rodoslovnaya">
              </div>
              <div class="Step__text">
                <span class="Step__textl">Детальное исследование выбранного сегмента рынка</span>
                <br>
                <br>
                Связанное с наличием высоких требований к квалификации, отраслевому опыту.
              </div>
            </div>
            <div class="Step__card">
              <div class="Step__img1">
                <img src="../../../assets/images/director-hire/Vc2r2.png" alt="Rodoslovnaya">
              </div>
              <div class="Step__text">
                <span class="Step__textl">Поиск, подбор, собеседования</span>
                <br>
                <br>
                с кандидатами/директорами; несколько этапов. С самыми сильными кандидатами проводим собеседование уже с участием собственника компании. Время по-думать собственнику, рекомендации по каждому кандидату. Вводим директора в курс дела, (советуем до этого провести полную диагностику всего бизнеса) проводим адаптацию, знакомим со все компанией, получаем от Вас доплату: остаток 30% стоимости услуги. Ведем первые дни работы, при необходимости. Такой полноценный и внимательный подход - позволяет нам выстроить с Вами долгосрочные отношения, поддерживать, консультировать, а Вам не терять время на повторные поиски и зарабатывать.
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
.Step{
  background: #fff;
}
.Step__inner{
  padding: 100px 0 85px 0;
  .Step__title{
    font-family: $ff1;
    font-style: normal;
    font-weight: 700;
    font-size: 28px;
    line-height: 130%;
    color: #1D1D1D;
    padding: 0 0 50px 0;
  }
  .Step__cards{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: flex-start;
    row-gap: 16px;
    column-gap: 5px;
    .Step__cardgr{
      width: 49%;
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      align-items: flex-start;
      row-gap: 16px;
      column-gap: 5px;
    }
    .Step__card{
      padding: 35px 27px 35px 45px;
      min-height: 190px;
      background: #C4C4C44F;
      border-radius: 50px;
      width: 99%;
      .Step__img{
        width: 8%;
        padding: 0 0 30px 0;
      }
      .Step__img1{
        width: 9%;
        padding: 0 0 30px 0;
      }
      .Step__text{
        height: fit-content;
        position: relative;
        font-family: $ff2;
        font-style: normal;
        font-weight: 400;
        font-size: 20px;
        line-height: 26px;
        color: rgba(29, 29, 29, 0.8);
        .Step__textl{
          font-weight: 700;
          font-size: 24px;
          line-height: 130%;
        }
      }
    }
  }
}
@media (max-width: 1024px) {
  .Step{
    box-sizing: content-box;
  }
  .Step__inner{
    padding: 100px 0 103px 0;
    .Step__title{
      padding-bottom: 23px;
    }
    .Step__cards{
      row-gap: 25px;
      .Step__card{
        display: flex;
        justify-content: flex-start;
        align-items: center;
        .Step__text{
          font-size: 18px;
          line-height: 22px;
        }
      }
    }
  }
}

@media (max-width: 768px) {
  .Step__inner{
    padding: 100px 0 65px 0;
    .Step__title{
      padding-bottom: 66px;
    }
    .Step__cards{
      column-gap: normal;
      .Step__card{
        width: 95%;
        min-height: 145px;
        padding: 33px 20px 33px 20px;
        display: block;
        .Step__text{
          width: 90%;
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
  .Step__inner{
    padding-bottom:  64px;
    .Step__title{
      padding-bottom: 42px;
    }
    .Step__cards{
      column-gap: normal;
      row-gap: 20px;
      .Step__cardgr{
        width: 93%;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
        align-items: flex-start;
        row-gap: 16px;
        column-gap: 5px;
      }
      .Step__card{
        width: 95%;
        min-height: 145px;
        padding: 33px 20px 33px 20px;
      }
    }
  }
}
@media (max-width: 360px) {
  .Step__inner{
    padding:  57px 0 72px 0;
    .Step__title{
      font-size: 24px;
      line-height: 29px;
      padding-bottom: 33px;
    }
    .Step__cards{
      column-gap: normal;
      row-gap: 15px;
      .Step__card{
        padding: 30px 12px 30px 40px;
        min-height: 100px;
        .Step__text{
          font-size: 16px;
          line-height: 20px;
          &::before{
            top: 8px;
            left: -15px;
            width: 5px;
            height: 5px;
          }
        }
      }
    }
  }
}
</style>
