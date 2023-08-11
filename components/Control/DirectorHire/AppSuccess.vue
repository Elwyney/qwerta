<template>
  <section class="Receive">
    <div class="container">
      <div class="Receive__inner">
        <div class="Receive__title">
          Успешно подобрали <span class="Receive__white">директора и сотрудников для</span>
        </div>
        <div class="Receive__cards">
          <div class="Receive__img1">
            <img src="../../../assets/images/director-hire/LOGO_ufaritual.png" alt="UfaRitual">
          </div>
          <div class="Receive__card">
            <div class="Receive__text">
              Отобрали и наняли директора
            </div>
            <br>
            <div class="Receive__text">
              Помогли адаптироваться на рабочем месте
            </div>
            <br>
            <div class="Receive__text">
              Сделали полную диагностику бизнеса
            </div>
          </div>
          <div class="Receive__img2">
            <img src="../../../assets/images/director-hire/LOGO_rodoslovnaya.png" alt="Rodoslovnaya">
          </div>
          <div class="Receive__card">
            <div class="Receive__text">
              Полностью поменяли штат сотрудников компании
            </div>
            <br>
            <div class="Receive__text">
              За 6 месяцев управления:
              построили бизнесс процессы и увеличили доход на 400%
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
.Receive{
  @include bgcenter('../../../assets/images/control/business-diag/receive_bg.png');
}
.Receive__inner{
  padding: 100px 0 85px 0;
  .Receive__title{
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
  .Receive__cards{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: flex-start;
    row-gap: 16px;
    column-gap: 5px;
    .Receive__img1{
      width: 15.5%;
    }
    .Receive__img2{
      width: 15.5%;
    }
    .Receive__card{
      display: block;
      padding: 35px 27px 35px 45px;
      width: 27.5%;
      min-height: 190px;
      background: linear-gradient(122.93deg, rgba(100, 100, 100, 0.71) 1.7%, rgba(72, 71, 71, 0.12) 48.4%, rgba(115, 106, 106, 0.17) 94.76%);
      border-radius: 50px;
      .Receive__text{
        height: fit-content;
        position: relative;
        font-family: $ff2;
        font-style: normal;
        font-weight: 400;
        font-size: 18px;
        line-height: 125%;
        color: #FFFFFF;
        &::before{
          content: '';
          position: absolute;
          width: 8px;
          height: 8px;
          background: #FFFFFF;
          border-radius: 50%;
          top: 7px;
          left: -20px;
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
      .Receive__card{
        justify-content: flex-start;
        align-items: center;
        .Receive__text{
          font-size: 18px;
          line-height: 22px;
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
      .Receive__img1{
        width: 90%;
      }
      .Receive__img2{
        width: 90%;
      }
      .Receive__card{
        width: 90%;
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
    padding-bottom:  64px;
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
      }
    }
  }
}
@media (max-width: 360px) {
  .Receive__inner{
    padding:  57px 0 72px 0;
    .Receive__title{
      font-size: 24px;
      line-height: 29px;
      padding-bottom: 33px;
    }
    .Receive__cards{
      column-gap: normal;
      row-gap: 15px;
      .Receive__card{
        padding: 30px 12px 30px 40px;
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
      }
    }
  }
}
</style>
