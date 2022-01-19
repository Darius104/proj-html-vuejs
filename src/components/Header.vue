<template>
    <header>
        <div class="row _container">
            <div class="col-4">
                <img src="../assets/logo.png" alt="">
            </div>
            <div class="col-8">
                <span :class="el.active ? 'active' :null" v-for="(el, index) in element" :key="index">{{ el.name }}</span>
                <div class="new"> new </div>
                <div class="_btn">
                    Schedule a workout
                </div>
                <i class="fas fa-shopping-cart"></i>
                <i class="fas fa-search"></i>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: "Header",
    props: {
        element: Array
    }
}
</script>

<style lang="scss" scoped>
@import '../style/container.scss';
@import '../style/color.scss';
@import '../style/btn.scss';

header{
    width: 100%;
    height: 100px;
    top: 0;
    background-color: black;
    color: $gray;
    display: flex;
    align-items: center;
    position: fixed;
    z-index: 10;

    .active{
        color: $white;
    }
    .new{
        background-color: $yellow;
        color: black;
        display: inline-block;
        margin-left: 5px;
        padding: 4px;
        border-radius: 10%;

        &:hover{
            cursor: pointer;
        }
    }
    span{
        margin-left: 40px;
        font-weight: bold;

        &:hover{
            cursor: pointer;
        }
    }
    ._btn{
        background-color: $semiBlue;
    }
    i{
        padding: 0 25px;

        &:hover{
            cursor: pointer;
        }
    }
}

</style>