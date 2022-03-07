<template>
    <section id="blog">
        <div class="container">
            <div class="header-text-wrap">
                <p class="section-title">blog</p>
                <div class="sub-text-wrap">
                    <h2>the recent news you must read it</h2>
                    <button class="aqua">view all</button>
                </div>
            </div>

            <div class="news-row">
                <div class="news">
                    <img src="../../assets/images/startup-business-people-and-strategy-board-PAJ3P9K-1390x1042.jpg" alt="startup business people">
                    <div class="card">
                        <div class="date-author">
                            <span>july 4, 2019</span>
                            <span>by paul</span>
                        </div>
                        <p class="news-title">Canadian Consulting firm acquired by UK Giant</p>
                        <p class="news-snippet">When, while the lovely valley teems with vapour around me, and the meridian sun strikes the upper surface of the impenetrable foliage of my trees, and but a ...</p>
                    </div>
                </div>
                <div class="news">
                    <img src="../../assets/images/business-people-working-together-on-project-and-5FHSKBL-1390.jpg" alt="business people working">
                    <div class="card">
                        <div class="date-author">
                            <span>july 4, 2019</span>
                            <span>by paul</span>
                        </div>
                        <p class="news-title">Canadian Consulting firm acquired by UK Giant</p>
                        <p class="news-snippet">When, while the lovely valley teems with vapour around me, and the meridian sun strikes the upper surface of the impenetrable foliage of my trees, and but a ...</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'BlogSection'
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/variables.scss';

#blog {
    background-color: $blue;
    padding-bottom: 200px;

    .header-text-wrap {
        color: $white;
        position: relative;
        margin-bottom: 60px;

        .sub-text-wrap {
            display: flex;
            justify-content: space-between;
            align-items: baseline;

            button {
                flex-shrink: 0;
            }
        }
    }

    .news-row {
        display: flex;
        justify-content: space-between;

        .news {
            width: 49%;
            height: 450px;
            position: relative;

            img {
                width: 100%;
                height: 100%;
                object-fit: cover;
            }

            .card {
                width: 80%;
                background: $white;
                padding: 40px 100px 40px 60px;
                position: absolute;
                top: 65%;
                right: 0;
                
                .date-author {
                    color: $red;
                    margin-bottom: 20px;

                    span {
                        margin-right: 20px;
                    }
                }

                .news-title {
                    font-size: 1.6rem;
                    margin-bottom: 30px;
                }

                .news-snippet {
                    color: $lightGrey;
                }
            }
        }
    }
}
</style>