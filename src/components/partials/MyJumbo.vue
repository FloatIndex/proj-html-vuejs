<template>
  <div id="jumbotron">
      <div class="left-jumbo">
          <div class="text-wrap">
              <p class="section-title">always the best way you need it</p>
              <h1>the best business consulting</h1>
              <button class="aqua">read more</button>
              <div class="play-button"><i class="fa-solid fa-play"></i></div>
          </div>
      </div>

      <div class="right-jumbo">
          <img src="../../assets/images/portrait-of-young-architect-woman-on-meeting-KFZCE3A.jpg" alt="two young people on meeting">
      </div>
  </div>
</template>

<script>
export default {
    name: 'MyJumbo'
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/variables.scss';

#jumbotron {
    height: 700px;
    display: flex;
    background-color: $blue;
    position: relative;

    .left-jumbo {
        height: 100%;
        width: 35%;

        .text-wrap {
            color: $white;
            text-transform: uppercase;
            position: absolute;
            top: 55%;
            left: calc(15% / 2);
            transform: translateY(-50%);
            width: 40%;

            h1 {
                font-size: 4.5rem;
                margin-bottom: 30px;
            }

            .play-button {
                width: 40px;
                height: 40px;
                border-radius: 50%;
                border: 1px solid $white;
                line-height: 40px;
                text-align: center;
                display: inline-block;
                margin-left: 30px;
                color: $aqua;

                &:hover {
                    cursor: pointer;
                    color: $red;
                }
            }
        }
    }

    .right-jumbo {
        height: 100%;
        width: 65%;
        background-color: $blue;

        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: top;
        }
    }
}
</style>