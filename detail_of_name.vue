<template>
    
<section>
    
     <ul id="pr_dt" >
        <li id="dt1">{{detail_name}}</li>
            
            
            <li id="dt11">{{detail_count}}</li>
        
        
    </ul>
    </section>




</template>

<script>
    
    export default {
     props:['detail_name','detail_count'],
        data () {
            return {
            }
        },
        components: {
        }
    }
</script>

<style>
    
      #pr_dt{
        position: relative;
       
        width: 260%;
      margin-right: 35%;
        height: 30px;
        margin-top: 5%;
        background-color:gainsboro;
        color: black;
          direction: rtl;
          margin-left: -85%;
    }
  
    #dt1{
        position: relative;
        text-align: right;
        margin-right: 15%;
          margin-top: -.1%;
        
    }
    
  
    #dt11{
        position: relative;
         text-align: right;
       margin-right: 10%;
       margin-top: -.1%;
        
        
    }
    
    
    
    
    
    
    
    
</style>