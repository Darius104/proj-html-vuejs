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

        </div>
    </main>
</template>

<script>
export default {
    name: "Main",
    props: {
        element: Array
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
    
}
</style>