<template>
    <div>
        <ul>
            <li v-for="stu in stus" :class="{'A':'red', 'B':'green'}"></li>
        </ul>
    </div>
</template>

<script>
    export default {
        data(){
            return{
                stus:[
                    {name: 'jack',score: 'A'},
                    {name: 'rows',score: 'B'}
                ]
            }
        }
    }
</script>
