<template>
<section>
       <div id="product_div2"> 
             <img id="a_img" :src="url_"/>
         
        </div>   
    
    </section>




</template>

<script>
    export default {
   props:['url_'],
        data () {
            return {
          
            }
        },
        components: {
        }
    }
</script>

<style>
    
     #product_div2{
        margin-top: 8%;
        width: 52%;
        height:100px;
        border: 1px solid;
        border-color:black;
        
       
    }
   #a_img{
        width: 100%;
        height:98px;
 
    }
    
    
    
    
    
    
    
     #product_text2{
      font-size: 10px;
        margin-top: 40%;
        margin-left: 5%;
       z-index: -1;
    }
    
    
    
    
</style>