<template>
    <section id="final-cta">
        <div class="text-wrap">
            <h2>let's talk about work</h2>
            <p>A wonderful serenity has taken possession far far away, behind the word mountains</p>
        </div>

        <button class="blue">get started</button>
    </section>
</template>

<script>
export default {
    name: 'FinalCtaSection'
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/variables.scss';

#final-cta {
    height: 400px;
    background-image: url('../../assets/images/business-people-working-together-on-project-and-B3MZ4TX.jpg');
    background-size: cover;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    .text-wrap {
        text-align: center;
        color: $white;
        width: 40%;
        margin-bottom: 20px;

        p {
            margin: 0 60px;
        }
    }
}
</style>