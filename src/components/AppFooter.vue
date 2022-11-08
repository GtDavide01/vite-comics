<script>
    export default{
        data(){
            return{

            }
        }
    }
</script>

<template>
    <footer>
        <div class="footer-top">
            <div class="container">
                <div class="allfooter">
                    <div class="footer-info">
                    <ul>
                        <h2>DC COMICS</h2>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>Games</li>
                        <li>Vidoes</li>
                        <li>News</li>
                        <h2>SHOP</h2>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                    <ul>
                        <h2>DC</h2>
                        <li>Terms Of use</li>
                        <li>Privacy policy (New)</li>
                        <li>Ad Choices</li>
                        <li>Advertsing</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshop</li>
                        <li>CPSC Certificates</li>
                        <li>ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                    <ul>
                        <h2>SITES</h2>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>
                <div class="footer-logo">
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </div>
                </div>
                
            </div>
        </div>
        <div class="footer-bottom">
            <div class="container">
                <div class="allfooter">
                    <div class="button-left">
                        <button> SIGN-UP NOW! </button>
                    </div>
                    <div class="info-footer-right">
                        <h2>FOLLOW US</h2>
                        <ul>
                            <li>
                             <img src="../assets/img/footer-facebook.png" alt="">
                            </li>
                            <li>
                                <img src="../assets/img/footer-twitter.png" alt="">
                            </li>
                            <li>
                                <img src="../assets/img/footer-youtube.png" alt="">
                            </li>
                            <li>
                                <img src="../assets/img/footer-pinterest.png" alt="">
                            </li>
                            <li>
                                <img src="../assets/img/footer-periscope.png" alt="">
                            </li>
                            
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
    .footer-top{
        background-image: url(../assets/img/footer-bg.jpg);
        .footer-info{
            display: flex;
            width: 50%;
            ul{
                list-style: none;
                padding: 2rem;
                h2{
                    margin-top: 10px;
                    color: white;
                }
                li{
                    color: grey;
                    font-size: .8rem;
                    padding: .2rem 0 ; 
                }
            }
        }
        .footer-logo{
            height: 350px;
            overflow: hidden;
            display: flex;
            align-items: center;
            width: 50%;
            img{
                width: 80%;
                background-position: top;
            }
        }
        .allfooter{
            display: flex;
        }
    }
    .footer-bottom{
            background-color: #303030;
            .allfooter{
            display: flex;
        }
            .button-left{
                padding: 2rem 0;
                display: flex;
                align-items: center;
                width: 50%;
                button{
                    margin-left: 1rem;
                    font-size: 1.1rem;
                    color: white;
                    padding: 15px;
                    border: 2px solid #0282f9;
                    background-color: #303030;
                }
            }
            .info-footer-right{
                
                width: 50%;
                display: flex;
                align-items: center;
                justify-content: end;
                h2{
                    color: #0282f9;
                }
                ul{
                    display: flex;
                    list-style: none;
                    li{
                        padding: 0 .5rem;
                    }
                };
            }
        }

</style>