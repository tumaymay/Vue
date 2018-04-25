<template>
  <div>
    父组件
    <br/><br/><br/><br/><br/>
    <Child @sendmsg="getMsg" :num="num"/>
    {{ info }}
  </div>
</template>

<script>
    
import Child from './child'

    export default{
        name:"parent",
        data(){
            return{
                info:"",
                num:10,
            }
        },
        components:{
            Child,
        },
        methods:{
            getMsg(data){
                this.info=data;
            }
        }
    }
</script>

<style>

</style>

