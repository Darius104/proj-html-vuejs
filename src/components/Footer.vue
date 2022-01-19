<template>
    <footer>
        <div class="_container">
            <div class="top">

            </div>
            <div class="bottom">

            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: "Footer"
}
</script>

<style lang="scss" scoped>
    footer{
        background-color: black;
        
        ._container{
            .top{
                height: 500px;
                border-bottom: 1px solid gray;
            }
            .bottom{
                height: 100px;
            }
        }
    }
</style>