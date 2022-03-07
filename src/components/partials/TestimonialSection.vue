<template>
    <section id="testimonial">

        <div class="container">
            <div class="text-wrap">
                <p>testimonial</p>
                <h2>what's the customers say about our work</h2>
            </div>
        </div>

        <div class="card-container">
            <div class="column">
                <div class="card">
                    <p>When, while the lovely valley teems with vapour around me, and the meridian sun strikes the upper surface of the impenetrable foliage of my trees, and but a few stray gleams steal into the inner sanctuary, I throw myself down among the tall grass by the trickling stream.</p>
                    <span class="customer-name">vera duncan</span>
                    <span class="customer-company">amazon inc.</span>
                </div>
                <img src="../../assets/images/oliver-ragfelt-488196-2.jpg" alt="customer vera duncan">
            </div>

            <div class="column">
                <div class="card">
                    <p>When, while the lovely valley teems with vapour around me, and the meridian sun strikes the upper surface of the impenetrable foliage of my trees, and but a few stray gleams steal into the inner sanctuary, I throw myself down among the tall grass by the trickling stream.</p>
                    <span class="customer-name">oliver ragfelt</span>
                    <span class="customer-company">amazon inc.</span>
                </div>
                <img src="../../assets/images/oliver-ragfelt-488196-unsplash.jpg" alt="customer oliver ragfelt">
            </div>

            <div class="column">
                <div class="card">
                    <p>When, while the lovely valley teems with vapour around me, and the meridian sun strikes the upper surface of the impenetrable foliage of my trees, and but a few stray gleams steal into the inner sanctuary, I throw myself down among the tall grass by the trickling stream.</p>
                    <span class="customer-name">john doe</span>
                    <span class="customer-company">amazon inc.</span>
                </div>
                <img src="../../assets/images/12679.jpg" alt="customer john doe">
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'TestimonialSection'
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/variables.scss';

#testimonial {
    background-color: $blue;
    color: $white;
    height: 600px;
    display: flex;
    flex-direction: column;

    .container {
        display: flex;
        justify-content: flex-end;

        .text-wrap {
            width: 60%;
            display: flex;
            flex-direction: column;

            p {
                text-transform: uppercase;
                margin-bottom: 20px;
                position: relative;

                &::after {
                    content: "";
                    display: block;
                    width: 40px;
                    height: 2px;
                    background-color: $aqua;
                    position: absolute;
                    right: 0;
                    top: 50%;
                }
            }

            h2 {
                width: 80%;
                text-align: right;
                margin-bottom: 30px;
                align-self: flex-end;
            }
        }
    }

    .card-container {
        width: 90%;
        height: 280px;
        background-color: $white;
        align-self: flex-end;
        display: flex;

        .column {
            width: calc(100% / 3);

            &:hover .card {
                display: none;
            }

            &:hover img {
                display: block;
            }

            img {
                display: none;
                width: 100%;
                height: 100%;
                object-fit: cover;
            }

            .card {
                width: 65%;
                margin: 40px auto 0 auto;
                display: flex;
                flex-direction: column;

                p {
                    color: $lightGrey;
                    margin-bottom: 30px;
                }

                .customer-name {
                    color: $black;
                    text-transform: capitalize;
                    font-weight: bold;
                    font-size: 1.3rem;
                    margin-bottom: 10px;
                }

                .customer-company {
                    color: $lightGrey;
                    text-transform: capitalize;
                }

            }
        }
    }
}
</style>