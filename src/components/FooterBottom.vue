<template>
    <div class="footer-bottom">
            <div class="container d-flex justify-content-between align-items-center">
                <div>
                    <button class="button-signup">Sign-up now!</button>
                </div>
                <div class="social">
                    <ul class="d-flex align-items-center ">
                        <span class="follow-us">Follow Us</span>
                        <li>
                            <a href=""><img src="../assets/img/footer-facebook.png" alt=""></a>
                        </li>
                        <li>
                            <a href=""><img src="../assets/img/footer-twitter.png" alt=""></a>
                        </li>
                        <li>
                            <a href=""><img src="../assets/img/footer-youtube.png" alt=""></a>
                        </li>
                        <li>
                            <a href=""><img src="../assets/img/footer-pinterest.png" alt=""></a>
                        </li>
                        <li>
                            <a href=""><img src="../assets/img/footer-periscope.png" alt=""></a>
                        </li>
                    </ul>
                </div>
            </div>
    </div>
</template>

<script>
    export default {
        name: 'FooterBottom'
    }
</script>

<style lang="scss" scoped>
    @use '../assets/styles/partials/_variables.scss' as *;
    .footer-bottom{
        position: relative;
        background-color: $headertext;
        margin-top: -80px;

        .follow-us{
            color: $bluetext;
            text-transform: uppercase;
            margin-right: 40px;
            font-size: 20px;
        }

        .container{
            padding: 30px;

            .button-signup{
            border: 3px solid $bluetext;
            padding: 8px 15px;
            text-transform: uppercase;
            background-color: $headertext;
            color: $white;
            }
            
            .social{

                ul{
                    list-style: none;
                    
                    li{
                        margin-left: 10px;
                    }
                }
            }
        }
    }
</style>