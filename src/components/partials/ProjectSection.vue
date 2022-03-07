<template>
    <section id="project">
        <div class="container">
            <div class="text-wrap">
                <p class="section-title">project</p>
                <h2>our expert trusted consultants help clients</h2>
            </div>

            <div class="slider">
                <img src="../../assets/images/DRY-1-790x592.jpg" alt="business people working">
                <img src="../../assets/images/221bf0b7-8134-43bb-936a-5acbe42db64a-790x592.jpg" alt="business people working">
                <img src="../../assets/images/z1el4c4p-790x592.jpg" alt="business people working">

                <div class="arrows">
                    <div class="prev"><i class="fa-solid fa-arrow-left"></i></div>
                    <div class="next"><i class="fa-solid fa-arrow-right"></i></div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'ProjectSection'
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/variables.scss';

#project {
    height: 700px;
    background-color: $blue;
    color: $white;

    .container {
        height: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        
        .text-wrap {
            width: 60%;
            margin-bottom: 40px;
        }

        .slider {
            display: flex;
            gap: 20px;
            width: 100%;
            position: relative;

            img {
                width: calc(100% / 3);
                height: auto;
                object-fit: cover;
            }

            .arrows {
                display: flex;
                gap: 5px;
                position: absolute;
                top: -100px;
                right: 0;

                div {
                    width: 40px;
                    height: 40px;
                    line-height: 40px;
                    text-align: center;
                    background-color: $lightBlue;

                    &:hover {
                        cursor: pointer;
                        color: $aqua;
                    }
                }
            }
        }
    }
}
</style>