<template>
<section>
    <div id="bprice_div">
        <input id="bprice_ch1" value="قیمت واحد"/>
         <input type="text" id="bprice_ch11" value="9999 تومان"/>
        
    
       <input id="bprice_ch2" value="تخفیف "/>
         <input type="text" id="bprice_ch22" value="9999 تومان"/>
    
    <div id="bprice_line"></div>
       <input id="bprice_ch3" value="قیمت نهایی"/>
         <input type="text" id="bprice_ch33" value="9999 تومان"/>
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

    #bprice_div{
       position: relative;
        width: 70%;
        height: 130px;
        
      
    border: 1px solid;
        margin-left: 12%;
    direction: rtl;
    
    }
    
    
    
     #bprice_ch1{
         position: relative;
           margin-top: 2%;
     border: 1px solid;
        font-size: 14px;
           margin-right: 5%;
           border: 1px solid;
           border-color: white;
      
        width: 45%;
    }
       #bprice_ch11{
   position: relative;
           direction: ltr;
      margin-top: -1.5%;
           margin-right: -4%;
           border: 1px solid;
             border-color: white;
          font-size: 14px;
           height: 25px;
     width: 37%;
           
           color: black;
    }
    
   
    
    
    
 #bprice_ch2{
         position: relative;
           margin-top: 2%;
     border: 1px solid;
        font-size: 14px;
           margin-right: 5%;
           border: 1px solid;
           border-color: white;
      color: deeppink;
        width: 45%;
    }
       #bprice_ch22{
   position: relative;
           direction: ltr;
      margin-top: -1.5%;
           margin-right: -4%;
           border: 1px solid;
             border-color: white;
          font-size: 14px;
           height: 25px;
     width: 37%;
           
           color: deeppink;;
    }
    
     #bprice_ch3{
         position: relative;
           margin-top: 2%;
     border: 1px solid;
        font-size: 14px;
           margin-right: 5%;
           border: 1px solid;
           border-color: white;
      
        width: 45%;
    }
       #bprice_ch33{
   position: relative;
           direction: ltr;
      margin-top: -1.5%;
           margin-right: -4%;
           border: 1px solid;
             border-color: white;
          font-size: 14px;
           height: 25px;
     width: 37%;
           
           color: black;
    }
    
    
    #bprice_line{
        position: relative;
        width: 85%;
        height:0%;
        border: 1px solid;
    margin-top: 2%;
      margin-right: 6%;
        border-color: gainsboro;
     
      
        
    }
    
    
    
    
    
    
    
    
    
    
</style>