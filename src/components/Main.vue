<template>
    <main>
        <div class="jumbo-img">
            <div class="_container">
                <div class="row">
                    <div class="col-10">
                        <div class="jumbo-texts">
                            <span id="firstSpan">Certified fitness professional</span>
                            <h1>Take control of your health</h1>
                            <span id="secondSpan">Curabitur non nulla sit amet nisl tempus convallis quis ac lectus dolor sit amet.</span>
                            <div class="buttons">
                                <div class="youTube-btn _btn"><i class="fab fa-youtube"></i> Visit my YouTube channel</div>
                                <div class="_btn buyBtn">Buy Avada today <i class="fas fa-arrow-right"></i> </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-2 play">
                        <div class="tasto">
                            <i class="fas fa-play"></i>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="challenge-bk">
            <div class="_container">
                <div class="container-challenge-card">
                    <div class="challenge-card" v-for="(el, index) in element" :key="index">
                        <img class="challenge-img" :src="el.image" alt="">
                        <div class="challenge-card-text">
                            <h2>{{el.title}}</h2>
                            <h3>{{el.subtitle}}</h3>
                        </div>
                    </div>
                </div>
            </div>
            <div class="main-title-challenge">
                <h2>
                    "How you respond to the challenge in the second half <br>
                    will determine what you become after the game, <br>
                    whether you are a winner or a loser."
                </h2>
                <div class="subheader-profile">
                    <img class="subheader-profile-picture" src="../assets/avatar-1-2x.jpg" alt="">
                    <span id="nickname">Brad Hohnson</span>
                    <span id="town">Las Vegas</span>
                </div>
            </div>
        </div>
        <div class="section-container">
            <div class="row">
                <div class="col-6">
                    <div class="card-left-training">
                        <img class="training" src="../assets/service15-2x.jpg" alt="">
                    </div>
                </div>
                <div class="col-6">
                    <div class="card-right-training">
                        <span id="firstSpan">Tune up your workouts</span>
                        <h2>The best health & fitness advice online</h2>
                        <div class="youTube-card">
                            <img class="youtube-logo" src="../assets/unnamed.jpg" alt="">
                            <div>
                                <span>ThemeFusion <br> </span>
                                <div class="youtube-channel"><i class="fab fa-youtube"></i> Youtube</div>
                                <div class="subscribers">999+</div>
                            </div>
                        </div>
                        <p id="secondP">Arcu eu facilisi ut quisque placerat nunc habitant. Megna semper mauris, venenatis, leo integer sit pellentesque.</p>
                        <div class="btn youtubeBTN"> <i class="fab fa-youtube"></i> Visit my YouTube channel </div>
                    </div>
                </div>
            </div>
        </div>

        <div class="_container">
            
            <div class="row">
                <div class="col-10">
                    <h2>Featured playlist</h2>
                </div>
                <div class="col-2">
                    <span>View all videos ></span>
                </div>
            </div>

            <div class="featured-playlist">
                <div class="card-playlist" v-for="(el, index) in playlist" :key="index">
                    <img class="playlist-image" :src="el.image" alt="">
                    <div class="playlist-text">
                        <h4>{{el.title}}</h4>
                        <h5>{{el.subtitle}}</h5>
                    </div>
                </div>
            </div>
        </div>

        <div class="jambo-subscribe">
            <div class="_container">
                <div class="text-subscribe">
                    <span> Join our mailing list today </span>
                    <h2> Insider offers & flash sales in your <br>
                        inbox every week
                    </h2>
                    <div class="input-subscribe">
                        <input type="email" placeholder="Insert your email ...*">
                        <div class="_btn">Subscribe</div>
                    </div>
                    <p>
                        Curabitur non nulla sit amet nisl tempus convallis quis ac lectus dolor sit amet, <br> consectetur
                        adipiscing elit sed porttitor lectus
                    </p>
                </div>
            </div>
        </div>

        <div class="cards-subscribe-container">
            <div class="_container">
                <div class="card-subscribe" v-for="(ele, index) in subscribe" :key="index">
                    <h3>{{ele.title}}</h3>
                    <h4>{{ele.subtitle}}</h4>
                    <p>{{ele.desc}}</p>
                    <span>{{ele.span}}</span>
                </div>
            </div>
        </div>

        <div class="_container">
            <div class="title-subscribe">
                <h4>Latest articles</h4>
                <h5>Read all aricles ></h5>
            </div>
            <div class="container-cards-subscribe">
                <div class="card-buy" v-for="(e, index) in buy" :key="index">
                    <img :src="e.image" alt="">
                    <h2>{{e.title}}</h2>
                    <span>{{e.subtitle}}</span>
                </div>
            </div>
        </div>

        <div class="last-jambo">
            <div class="linear">
                <div class="jambo-text">
                    <h2>"I've faild over and over again in my <br> life. And that is why I succeed."</h2>
                    <p>Arcu auctor gravida nisl, congue sit nisi tincidunt eget proin. in lacinia lacus donec sed massa <br> in ipsum eros, tristique. Gravida suspendisse etiam in iaculis</p>
                    <div class="_btn">Buy Avada today</div>
                </div>
            </div>
        </div>

        <div class="_container">
            <div class="row text-center">
                <div class="col-3" v-for="(elem, index) in gym" :key="index">
                    <div class="card-gym">
                        <img :src="elem.image" alt="">
                        <p>
                            {{elem.text}}
                        </p>
                        <span>{{elem.last}}</span>
                    </div>
                </div>
            </div>
        </div>

        <div class="ultim-jambo">
            <div class="linear">           
                <div class="text">
                    <div class="play">
                        <i class="fas fa-play"></i>
                    </div>
                    <h2>Crossfit workout of the day</h2>
                    <h3>November 15th, 2019</h3>
                    <span>View all videos</span>
                </div>
            </div>
        </div>
    </main>
</template>

<script>
export default {
    name: "Main",
    props: {
        element: Array,
        playlist: Array,
        subscribe: Array,
        buy: Array,
        gym: Array
    }
}
</script>

<style lang="scss" scoped>
@import '../style/container.scss';
@import '../style/color.scss';
@import '../style/btn.scss';

.jumbo-img{
    width: 100%;
    height: 700px;
    background-image: url('../assets/slider.jpg');
    background-repeat: no-repeat;
    background-size: 100%;
    margin-top: 100px;

    .jumbo-texts{
        height: 700px;
        display: flex;
        flex-direction: column;
        justify-content: center;

        #firstSpan{
            color: #ff414b;
            font-weight: bold;
            font-size: 25px;
        }
        h1{
            color: $white;
            font-size: 60px;
        }
        #secondSpan{
            font-size: 17px;
            color: $gray;
            margin-bottom: 40px;
        }
        .youTube-btn{
            width: 25%;
            background-color: $semiBlue;
            padding: 15px;
            text-align: center;
            margin-left: 0;

            &:hover{
                background-color: #ff414b;
            }
        }
        .buyBtn{
            width: 20%;
            border: 2px solid gray;
            text-align: center;
        }

    }
    .play{
        display: flex;
        justify-content: center;
        align-items: center;

        .tasto{
            background-color: white;
            padding: 45px 50px;
            border-radius: 100%;

            &:hover{
                color: blue;
                cursor: pointer;
            }
        }
    }
}

.challenge-bk{
    width: 100%;
    height: 900px;
    background: linear-gradient(300deg, red, blue);
    position: relative;
    .container-challenge-card{
        display: flex;
    }
    .challenge-card{
        position: relative;
        top: -60px;
        width: 30%;
        margin: auto;

        .challenge-img{
            width: 100%;
            border-radius: 5px 5px 40px 5px;
            overflow: hidden;
            cursor: pointer;
        } 
        .challenge-card-text{
            position: absolute;
            left: 20px;
            bottom: 20px;
            
            h2{
                color: white;
            }
            h3{
                color: $yellow
            }
        }
    }

    .main-title-challenge{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        text-align: center;
        h2{
            color: $white;
            font-size: 50px;
            margin-bottom: 100px;
        }
        .subheader-profile-picture{
            border-radius: 50%;
            overflow: hidden;
            width: 20%;
        }
        #nickname{
            color: $white;
            font-weight: bold;
            margin: 0 30px;
            font-size: 20px;
        }
        #town{
            color: $gray;
            font-weight: bold;
            font-size: 20px;
        }
    }
}
.row{
    width: 100%;
}
.section-container{
    position: relative;
    top: -50px;
    .card-left-training{
        .training{
            width: 80%;    
            border-radius: 5px 5px 40px 5px;
            overflow: hidden;
        } 
    }
    .card-right-training{
        margin-top: 150px;
        #firstSpan{
            color: $semiBlue;
            font-size: 30px;
        }
        h2{
            font-size: 60px;
        }
        .youtube-logo{
            display: inline-block;
            margin-right: 10px;
        }
        .youTube-card{
            display: flex;
            margin: 30px 0;
            .youtube-channel{
                display: inline-block;
                background-color: red;
                border: 1px solid gray;
                border-radius: 2px;
                padding: 0 5px;
            }
            .subscribers{
                display: inline-block;
                background-color: white;
                border-right: 1px solid gray;
                border-top: 1px solid gray;
                border-bottom: 1px solid gray;
                border-radius: 2px;
                padding: 0 3px;
                width: 40px;
            }
        }
        #secondP{
            font-size: 25px;
            color: $gray;
            margin-bottom: 80px;
        }
        .youtubeBTN{
            background-color: red;
            border-radius: 50px;
            padding: 15px 40px;
            color: white;

            &:hover{
                background-color: #ff414b;
                cursor: pointer;
            }
        }
    } 
}
.featured-playlist{
    margin-top: 50px;
    display: flex;

    .card-playlist{
        width: 30%;
        margin-right: 50px;
    }
    .playlist-image{
        width: 100%;
        margin-bottom: 20px;
        border-radius: 5px 5px 40px 5px;
        overflow: hidden;
    }
    .playlist-text{
        text-align: center;

        h5{
            color: $semiBlue;
        }
    }
}
.jambo-subscribe{
    background-image: url('../assets/banner1-2x.jpg');
    width: 100%;
    height: 800px;
    background-size: cover;
    background-repeat: no-repeat;
    background-position-x: right;
    margin-top: 100px;

    .text-subscribe{
        height: 800px;
        display: flex;
        flex-direction: column;
        justify-content: center;

        span{
            color: #ff414b;
            font-size: 25px;
            font-weight: bold;
        }
        h2{
           color: $white; 
           font-size: 60px;
           margin-bottom: 40px;
        }
        .input-subscribe{
            margin-bottom: 40px;

            input{
                padding: 20px;
                border-radius: 50px;
                border: none;
                width: 40%;
            }
            ._btn{
                background-color: $semiBlue;
                padding: 20px;
                width: 15%;
                text-align: center;
                font-weight: bold;

                &:hover{
                    cursor: pointer;
                    background-color: #ff414b;
                }
            }
        }
        p{
            font-size: 25px;
            color: $gray;
        }
    }
}
.cards-subscribe-container{
    background-color: #060608;
    width: 100%;
    color: white;

    ._container{
        display: flex;
        justify-content: space-between;

    }
    .card-subscribe{
        width: calc(100% / 3.5);
        text-align: center;
        border: 5px solid $semiBlue;
        border-radius: 10px;
        padding: 100px 30px;
        display: inline-block;
        margin: 100px 0;

        h3{
            color: $white;
        }
        h4{
            color: $yellow;
            margin-bottom: 30px;
        }
        span{
            font-weight: bold;
        }
    }
}

._container{
    margin-bottom: 100px;

    .title-subscribe{
        display: flex;
        justify-content: space-between;
        margin-top: 120px;
        margin-bottom: 30px;
    }
    .container-cards-subscribe{
        display: flex;
        justify-content: space-between;
    }
    .card-buy{
        width: calc(100% / 3.5);
        h2{
            margin-left: 20px;
            margin-top: 20px;
        }
        span{
            margin-left: 20px;
        }
    }
}

.last-jambo{
    background-image: url('../assets/banner2-2x.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    height: 700px;

    .linear{
        background: linear-gradient(to top, #010014, #04022c11);
        height: 100%;
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        text-align: center;

        h2{
            color: white;
            font-size: 50px;
            margin-bottom: 40px;
        }
        p{
            color: white;
            font-size: 20px;
            margin-bottom: 40px;
        }
        ._btn{
            background-color: $semiBlue;
            padding: 15px 35px;
            font-weight: bold;

            &:hover{
                background-color: #ff414b;
            }
        }
    }
}
.card-gym{
    margin-top: 120px;

    img{
        margin-bottom: 30px;
    }
    p{
        margin-bottom: 20px;
    }
    span{
        font-weight: bold;
    }
}

.ultim-jambo{
    height: 700px;
    background-image: url('../assets/banner14-2x.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    
    .linear{
        background: linear-gradient(300deg, rgba(63, 9, 9, 0.815), rgba(8, 8, 122, 0.794));
        width: 100%;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        .text{
            text-align: center;
            .play{
                background-color: $white;
                display: inline-block;
                padding: 35px 40px;
                border-radius: 100%;
                margin-bottom: 50px;
            }
            h2{
                color: $white;
                font-size: 50px;
            }
            h3{
                color: $yellow;
                font-size: 30px;
            }
            span{
                color: $white;
                font-weight: bold;
                font-size: 20px;
            }
        }        
    }
}
</style>