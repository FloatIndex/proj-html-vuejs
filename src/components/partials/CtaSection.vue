<template>
    <section id="cta">
        <div class="text-container">
            <div class="text-wrap">
                <h3>we help to deliver the business case</h3>
                <p>When, while the lovely valley teems with vapour around me, and the meridian sun strikes the upper surface of the impenetrable foliage of my trees, and but a thousand unknown</p>
            </div>

            <button class="red">get started</button>
        </div>
    </section>
</template>

<script>
export default {
    name: 'CtaSection'
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/variables.scss';

#cta {
    height: 300px;
    background-color: $blue;

    .text-container {
        width: 90%;
        height: 100%;
        background-color: $aqua;
        position: relative;

        .text-wrap {
            height: 100%;
            color: $blue;
            display: flex;
            align-items: center;
            justify-content: space-evenly;
            

            h3 {
                width: calc(100% / 3);
            }

            p {
                width: calc(100% / 3);
            }
        }

        button {
            position: absolute;
            bottom: 0;
            right: 0;
        }
    }
}
</style>