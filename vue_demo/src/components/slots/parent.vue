<template>
  <div class="parent">
    父组件
    <br/><br/><br/><br/><br/>
    <Child>
        <div slot="s1">
            <p class="ptest" slot="s1">我是插槽1</p>
            <p class="ptest" slot="s2">我是插槽2</p>
        </div>
       
        <p class="ptest" slot="s2" slot-scope="key">{{key.text}}</p>
        
   </Child>
  </div>
</template>

<script>
    
import Child from './child'

    export default{
        name:"parent",
        data(){
            return{

            }
        },
        components:{
            Child
        }
        
    }
</script>

<style>
.ptest{
    color: brown
}
</style>

