<template>
    <section id="about">
        <div class="left">
            <img src="../../assets/images/business-people-working-together-on-project-and-5FHSKBL.jpg" alt="business people working">
        </div>

        <div class="right">
            <div class="text-wrap">
                <p class="section-title">about us</p>
                <h2>we make your strategy work</h2>
                <p class="sub-txt">When, while the lovely valley teems with vapour around me, and the meridian sun strikes the upper surface of the impenetrable foliage of my trees, and but a few stray gleams steal into the inner sanctuary, I throw myself down among the tall grass by the trickling stream; and, as I lie close to the earth, a thousand unknown plants are noticed by me: when I hear the buzz of the little world among the stalks, and grow familiar with the countless indescribable forms of the insects and flies, then I feel the presence of the Almighty</p>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'AboutSection'
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/variables.scss';

#about {
    height: 600px;
    background-color: $blue;
    display: flex;

    .left {
        width: 55%;
        height: 100%;

        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
    }

    .right {
        width: 45%;
        height: 100%;
        display: flex;
        align-items: center;

        .text-wrap {
            width: 65%;
            color: $white;
            margin-left: 50px;
        }

        h2 {
            text-transform: uppercase;
            margin-bottom: 30px;
            font-size: 2.8rem;
        }

        .sub-txt {
            color: $lightGrey;
        }
    }
}
</style>