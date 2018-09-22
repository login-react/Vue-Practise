
<!--class取一个，返回一个字符串-->
<template>
    <div>
        <div v-bind:class="isRead ? 'red': 'green'">123</div>
    </div>
</template>
<script>
    export default {
        data(){
            return{
                isRead: false
            }
        }
    }
</script>
<style>
    .red {
        background-color: red;
    }
    .green{
        background-color: green;
    }
    .big{
        font-size: 30px;
    }
</style>


<!--取多个返回一个对象-->
<template>
    <div>
        <div :class="{'red': true, 'big': true}"></div>
    </div>
</template>
<script>
    export default {
        data(){
            return{
                isRead: false
            }
        }
    }
</script>
<style>
    .red {
        background-color: red;
    }
    .green{
        background-color: green;
    }
    .big{
        font-size: 30px;
    }
</style>
