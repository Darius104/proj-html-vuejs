<template>
    <footer>
        <div class="_container">
            <div class="top">
                <div class="row">
                    <div class="col-4">
                        <img src="../assets/logo.png" alt="">
                        <p>
                            Ac aliquam neque sagittis diam faucibus vitae purus turipis phasellus. pallentesque consectetur amet purus ultrices mauris.
                        </p>
                        <ul>
                            <li><i class="fab fa-facebook-f"></i></li>
                            <li><i class="fab fa-twitter"></i></li>
                            <li><i class="fab fa-youtube"></i></li>
                            <li><i class="fab fa-instagram"></i></li>
                            <li><i class="fab fa-linkedin-in"></i></li>
                        </ul>
                    </div>

                    <div class="col-4">
                        <h3>RECENT POST</h3>
                        <span> > The best protein shake</span><br>
                        <span> > Ultimate cardio workout</span><br>
                        <span> > New juices available now</span><br>
                        <span> > Tips to find training partners</span><br>
                        <span> > 20 best healthy recipes</span><br>
                    </div>

                    <div class="col-4">
                        <h3>CONTATC INFORMATIONS</h3>
                        <span>4746 Tipple Road Michigan 48449</span><br>
                        <span>Mobile: 1.800.000.0000</span><br>
                        <span>Email: info@your-company.com</span><br>
                    </div>
                </div>
            </div>
        </div>
        <div class="bottom">
            Copyright 2012 - 2020 | Avada theme by  <span>  ThemeFusion</span> | All rights reserved | Power by  <span>  WordPress</span>
        </div>
    </footer>
</template>

<script>
export default {
    name: "Footer",
}
</script>

<style lang="scss" scoped>
@import '../style/container.scss';
@import '../style/color.scss';
@import '../style/btn.scss';

    footer{
        background-color: black;
        
        ._container{
            .top{
                height: 500px;
                text-align: center;
                padding-top: 100px;

                img{
                    margin-bottom: 30px;
                }
                p{
                    color: $white;
                    font-size: 20px;
                }
                ul{
                    list-style-type: none;
                    display: flex;
                    justify-content: center;

                    li{
                        margin: 10px;
                        font-size: 25px;
                        color: #ff414b;
                    }
                }
            }
            h3{
                color: $white;
            }
            span{
                color: $white;
            }
        }
        .bottom{
            height: 100px;
            border-top: 1px solid gray;
            display: flex;
            justify-content: center;
            align-items: center;
            color: #5b819f;

            span{
                color: $white;
            }
        }
    }
</style>