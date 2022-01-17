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

header{
    width: 100%;
    height: 100px;
    background-color: black;
    color: $gray;
    display: flex;
    align-items: center;

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
    }
    span{
        margin-left: 40px;
        font-weight: bold;
    }
    ._btn{
        color: $white;
        display: inline-block;
        margin-left: 40px;
        background-color: $semiBlue;
        padding: 10px;
        border-radius: 30px;

        &:hover{
            background-color: #ff414b;
            cursor: pointer;
        }
    }
    i{
        padding: 0 25px;
    }
}

</style>