<template>
    <div>
       <p>History</p>
       <span  class="number" v-for="(number,index) in history" :key="index" 
        :class="showNumber(parseInt(value)).includes(index) && 'bold'">
         {{ number }}
       </span>
    </div>
    <!-- {{ showNumber(number) }} -->
    <input type="number" v-model="number" />
</template>

<script>
import {mapState, mapGetters} from 'vuex';

    export default {
        name:'HistoryComponent',
        data(){
            return{
                value: ''
            }
        },
        computed:{
            ...mapState(['history','number']),
            ...mapGetters(['showNumber'])
        }
    }
</script>

<style scoped>

.number{
    margin-right: 20px;
}
.bold{
    font-weight: bold;
}

</style>