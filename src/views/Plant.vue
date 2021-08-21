<template>
  <main id="plant-page">
    <header>
        <div @click="router.push('/')" class="arrow">
          <svg width="53" height="24" viewBox="0 0 53 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M0.939339 10.9393C0.353554 11.5251 0.353554 12.4749 0.939339 13.0607L10.4853 22.6066C11.0711 23.1924 12.0208 23.1924 12.6066 22.6066C13.1924 22.0208 13.1924 21.0711 12.6066 20.4853L4.12132 12L12.6066 3.51472C13.1924 2.92893 13.1924 1.97918 12.6066 1.39339C12.0208 0.807608 11.0711 0.807608 10.4853 1.39339L0.939339 10.9393ZM53 10.5L2 10.5L2 13.5L53 13.5L53 10.5Z" fill="black"/>
          </svg>
        </div>
        <!-- <img src="@/assets/img/basil.png" alt=""> -->
        <h1 class="title">Plant Name</h1>
        <h3 class="type">Plant Type</h3>
        <span class="status healthy">Healthy</span>
    </header>
    <div class="plant-care">
      <h3 class="title">Plant Care</h3>
      <span class="icon">#1</span><p>Every 3 weeks</p>
      <article class="water-cycle">
        <p>Next Watering</p>
      </article>
    <h2 class="info-title">Information</h2>
    <p class="info-body">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Totam at deleniti quisquam in culpa minima error, architecto magnam nobis doloribus optio maiores iste impedit ratione consequuntur ducimus ad reprehenderit beatae?</p>
    </div>
  </main>
</template>

<script>
export default {
  name: 'plant',

}
</script>

<style scoped lang="scss">
  #plant-page {
    background: #0B5345; 
    // width: 100vw;
    height: 100vh;
    header {
      width: 100vw;
      height: 383px;
      left: 0px;
      top: -1px;
      background: #FFFFFF;
      border-radius: 0px 0px 40px 40px;
    }
    img {
      position: relative;
      width: 100vw;
      height: 279px;
      left: 200px;
      top: 111px;
      overflow: hidden;
    }
    .status {
      position: absolute;
      width: 135px;
      text-align: center;
      height: 32px;
      left: 20px;
      top: 272px;
      font-weight: bold;
      box-sizing: border-box;
      border-radius: 50px;
      font-size: 21px;
        &.thirsty {
          color: #BEA624;
          border: 1px solid #BEA624;
          background: rgba(190, 166, 36, 0.5);
        }
        &.healthy {
          background: rgba(69, 179, 157, 0.5);
          border: 2px solid #0B5345;
          color: #0B5345;
        }
    }
    .title {
      position: absolute;
      width: 189px;
      height: 42px;
      left: 18px;
      top: 128px;
      font-style: normal;
      font-weight: bold;
      font-size: 36px;
      color: #000000;
    }
    .type {
      position: absolute;
      width: 285px;
      height: 47px;
      left: 20px;
      top: 170px;

      font-style: normal;
      font-weight: bold;
      font-size: 24px;
      line-height: 28px;

      color: #C4C4C4;
    }
    .arrow {
      position: absolute;
      width: 51px;
      height: 0px;
      left: 18px;
      top: 46px;
    }
    .plant-care {
      .title {
        position: absolute;
        left: 20px;
        top: 434px;
        font-style: normal;
        font-weight: bold;
        font-size: 24px;
        line-height: 28px;
        color: #FFFFFF;
      }
      .icon {
        position: absolute;
        width: 40px;
        height: 40px;
        left: 20px;
        border-radius: 50%;
      }
      p {
        position: absolute;
        left: 60px;
        top: 12px;
        font-style: normal;
        font-weight: normal;
        font-size: 18px;
        color: #FFFFFF;
      }
      .water-cycle {
        position: absolute;
        width: 152px;
        height: 165px;
        top: 472px;
        right: 0;
        overflow: hidden;
        background: rgba(69, 179, 157, 0.5);
        border-radius: 20px 0px 0px 20px;
        p {
          left: 10px;
          text-align: center;
          // width: 100%;
        }
      }
      .info-title {
        position: absolute;
        width: 125px;
        height: 28px;
        left: 17px;
        top: 681px;
        font-style: normal;
        font-weight: normal;
        color: #FFFFFF;
      }
      .info-body {
        position: absolute;
        height: 136px;
        left: 18px;
        top: 722px;
        font-style: normal;
        font-weight: normal;
        font-size: 12px;
        line-height: 14px;
        color: #FFFFFF;
      }
    }
  }
</style>