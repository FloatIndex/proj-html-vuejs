<template>
    <footer>
        <!-- inizio container -->
        <div class="container">


            <!-- inizio footer top -->
            <div class="footer-top">
                <nav>
                    <!-- logo -->
                    <a href="#"><img class="logo" src="../assets/images/logotype-2-139x23.png" alt=""></a>
                    
                    <!-- menu -->
                    <MyMenu :menu="menu"/>

                    <!-- icone social -->
                    <div class="socials">
                        <a href="#"><i class="fa-brands fa-instagram"></i></a>
                        <a href="#"><i class="fa-brands fa-linkedin-in"></i></a>
                        <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
                        <a href="#"><i class="fa-brands fa-twitter"></i></a>
                    </div>

                </nav>
            </div>
            <!-- fine footer top -->


            <!-- inizio footer bottom -->
            <div class="footer-bottom">
                <div class="terms-privacy">
                    <a href="#"><p>Terms of use</p></a>
                    <a href="#"><p>Privacy Environmental Policy</p></a>
                </div>
                <p class="copyright">copyright &copy; 2020 phlox consulting. all rights reserved.</p>
            </div>
            <!-- fine footer bottom -->


        </div>
        <!-- fine container -->
    </footer>
</template>

<script>
import MyMenu from './partials/MyMenu.vue';
export default {
    name: 'MyFooter',
    props: {
        menu: Array
    },
    components: {
        MyMenu
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';

footer {
    height: 300px;
    background-color: $blue;
    color: $opaque;

    .container {
        height: 100%;

        .footer-top {
            height: 60%;
            border-bottom: 1px solid rgba(255, 255, 255, 0.2);

            nav {
                height: 100%;
                display: flex;
                justify-content: space-between;
                align-items: center;

                .logo {
                    height: 12px;
                }

                .socials a {
                    margin-left: 15px;
                    color: $white;
                }
            }
        }

        .footer-bottom {
            height: 40%;
            display: flex;
            justify-content: space-between;
            align-items: center;

            .terms-privacy p {
                margin-bottom: 10px;
            }

            .copyright {
                text-transform: capitalize;
            }
        }
    }
}
</style>