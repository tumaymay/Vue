<template>
  <div>
   子组件
   <input type="text" v-model="num">
   <button @click="sendMsg">传递数据</button>
    
  </div>
</template>

<script>
    


    export default{
        name:"child",
        data(){
            return{
                msg:"我是子组件数据"
            }
        },
        computed:{
            addNum(){
                return this.num * 5;
            }
        },
        methods:{
            sendMsg(event){
                this.$emit("sendmsg",this.addNum);

            }
        },
        props:{
            num:{
                type:Number,
                default:5
            }
        }
        
    }
</script>

<style>

</style>
