<template>
    <section id="consulting">

        <!-- titolo -->
        <div class="title-wrap">
            <h3>our consultants can help you</h3>
        </div>

        <!-- contenuto -->
        <div class="cards-container">

            <div class="card">
                <div class="icon-box">
                    <i class="fa-solid fa-chart-line"></i>
                </div>

                <div class="text-box">
                    <h4>statistical consulting</h4>
                    <p>When, while the lovely valley teems with vapour around me, and the meridian sun strikes the upper surface of the impenetrable foliage of my trees, and but a</p>
                </div>
            </div>
            
            <div class="card">
                <div class="icon-box">
                    <i class="fa-solid fa-bullhorn"></i>
                </div>

                <div class="text-box">
                    <h4>digital consulting</h4>
                    <p>When, while the lovely valley teems with vapour around me, and the meridian sun strikes the upper surface of the impenetrable foliage of my trees, and but a</p>
                </div>
            </div>
            
            <div class="card">
                <div class="icon-box">
                    <i class="fa-solid fa-wallet"></i>
                </div>

                <div class="text-box">
                    <h4>banking consulting</h4>
                    <p>When, while the lovely valley teems with vapour around me, and the meridian sun strikes the upper surface of the impenetrable foliage of my trees, and but a</p>
                </div>
            </div>
            
            <div class="card">
                <div class="icon-box">
                    <i class="fa-solid fa-bullseye"></i>
                </div>

                <div class="text-box">
                    <h4>enterprise consulting</h4>
                    <p>When, while the lovely valley teems with vapour around me, and the meridian sun strikes the upper surface of the impenetrable foliage of my trees, and but a</p>
                </div>
            </div>
            
        </div>
        <!-- fine contenuto -->

    </section>
</template>

<script>
export default {
    name: 'ConsultingSection'
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/variables.scss';

#consulting {
    width: 65%;
    margin: 80px auto 130px auto;

    h3 {
        font-size: 1.3rem;
        position: relative;

        &::after {
            content: '';
            display: block;
            width: 84%;
            height: 2px;
            background-color: $aqua;
            position: absolute;
            left: 400px;
            top: 50%;
        }
    }

    .cards-container {
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;

        .card {
            width: 40%;
            margin-top: 100px;
            display: flex;

            .icon-box {
                width: 45px;
                height: 45px;
                border-radius: 50%;
                background-color: $red;
                color: $white;
                line-height: 45px;
                text-align: center;
                margin-right: 30px;
                flex-shrink: 0;

                svg {
                    transform: scale(1.6);
                }
            }

            h4 {
                margin-top: 5px;
                margin-bottom: 15px;
            }

            p {
                color: $lightGrey;
            }
        }
    }
}
</style>