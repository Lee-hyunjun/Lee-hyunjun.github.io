<template>
  <div>
    <div class="slideButton">
      <img class="arrow1" src="../assets/arrow.png" alt="arrow">
      <img class="arrow2" src="../assets/arrow.png" alt="arrow">
    </div>
    <div class="slides">
      <div class="slide1">
        <div class="slide1Text">
          <span>Why Business Design Lab?</span>
          <p>잘하는 것을 더 잘하게, </p>
          <p>하고 싶은 것을 시작할 수 있게,</p>
          <p>전문가들의 노하우와 빅데이터 분석을 통해 </p>
          <p>나아갈 방향을 제시합니다.</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  components: {
  }
}
</script>

<style lang="scss">
    .slideButton{
      position: absolute;
      top:37%;
      padding: 0 58px;
      width: 100%;
      display: flex;
      align-items: center;
      justify-content: space-between;

      img:hover{
        cursor: pointer;
      }

      .arrow1{
        transform: rotate(180deg);
      }

    }
    .slides{
        max-height: 797px;
        width: 100%;
        height: 798px;
        overflow: hidden;

        .slide1{
          background-image: url("../assets/slide/slide1.png");
          width: 100%;
          height: 100%;

          .slide1Text{
            padding-top: 240px;
            max-width: 1200px;
            width: 100%;
            max-height: 246px;
            height: 100%;
            margin: 0 auto;

            span{
              display: block;
              color: white;
              font-size: 20px;
              margin-bottom: 25px;
              font-family: GmarketSansTTFMedium ,sans-serif;
              font-size: 1.25rem;
            }

            p{
              font-size: 2.8125rem;
              font-weight: bold;
              color: #01bc9a;
              font-family: GmarketSansTTFBold ,sans-serif;
            }
            
          }
        }
    }
</style>
