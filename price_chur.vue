<template>
<section>
    <div id="price_div">
        <input id="price_ch1" value="قیمت واحد"/>
         <input type="text" id="price_ch11" value="9999 تومان"/>
        
    
        <input id="price_ch2" value="تخفیف" />
         <input type="text" id="price_ch22" value="9999 تومان"/>
    
    
    <div id="price_line"></div>
        <input id="price_ch3" value="قیمت نهایی"/>
         <input type="text" id="price_ch33" value="9999 تومان"/>
    </div>
    
    </section>




</template>

<script>
    export default {
        data () {
            return {
            }
        },
        components: {
        }
    }
</script>

<style>

    #price_div{
       position: relative;
        width: 80%;
        height: 130px;
        
     
       margin-left: 25%;
        
    direction: rtl;
    
    }
    
    
 
   
        #price_ch1{
           position: relative;
      width: 65%;
       margin-left: 1%;
        border: 1px solid;
           border-color: white;
         font-size: 15px;
        
    
       
      
    }
    #price_ch11{
          position: relative;
     width: 28%;
        margin-left: -15%;
         border: 1px solid;
      border-color: white;
      
         font-size: 15px;
       
    }
    
    
        #price_ch2{
           position: relative;
      width: 65%;
       margin-left: 1%;
        border: 1px solid;
           border-color: white;
         font-size: 15px;
        
    color: deeppink;
       
      
    }
    #price_ch22{
          position: relative;
     width: 28%;
        margin-left: -15%;
         border: 1px solid;
      border-color: white;
      color: deeppink;
         font-size: 15px;
       
    }
    
    
    
    
    
    
    
    
    
    
        #price_ch3{
           position: relative;
      width: 65%;
       margin-left: 1%;
        border: 1px solid;
           border-color: white;
         font-size: 15px;
        
    margin-top: 7%;
       
      
    }
    #price_ch33{
          position: relative;
     width: 28%;
        margin-left: -15%;
         border: 1px solid;
      border-color: white;
      
         font-size: 15px;
       
    }
    
    
    
    
    
    
    #price_line{
       
       position: relative;
        width: 110%;
        height:0%;
        border: 1px solid;
    margin-top: 5%;
        border-color: gainsboro;
     
        margin-right: 8%;
        
    }
    
    
    
    
    
    
    
    
    
    
</style>