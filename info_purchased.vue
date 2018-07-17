<template>
  
<section>
    
    <div id="div_purch">
    
    <input type="text" id="brand_chur" value="نام برند"/>
         <input type="text" id="name_chur1" value="نام محصول"/>
         <input type="text" id="name_chur2" value="نام محصول"/>
         <input type="text" id="name_chur3" value="نام محصول"/>
       <input type="text" id="color_chur1" value="رنگ:"/>
         <input type="text" id="color_chur2" value="نام رنگ"/>
        <input type="text" id="size_chur1" value="سایز:"/>
        <input type="text" id="size_chur2"   value="عدد سایز"/>
       <input type="text" id="kod_chur1" value="کد:"/>
         <input type="text" id="kod_chur2"  value="کد کالا"/>
         
        
        
        
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
    #div_purch{
       
     color: black;
     position: relative;
        width: 50%;
        margin-left:16%;
        direction: rtl;
         
        height: 140px;
     
margin-top: -31%;
    }
    
    
    #brand_chur{
          position: relative;
        width: 85%;
              margin-left: 12%;
        border: 1px solid;
           border-color: white;
        font-size: 12px;
          
    }
    
    #name_chur1{
          position: relative;
      width: 28%;
        border: 1px solid;
           border-color: white;
         font-size: 12px;
    
       
      
    }
    #name_chur2{
        position: relative;
     width: 28%; 
        border: 1px solid;
           border-color: white;
     
         font-size: 12px;
       
    }
    #name_chur3{
          position: relative;
          border: 1px solid;
           border-color: white;
       
         font-size: 12px;
    margin-left: 15%;
      width: 28%;  
    }
    
    
    
    
    
    
    
     #color_chur1{
           position: relative;
      width: 12%;
       margin-left: 1%;
        border: 1px solid;
           border-color: white;
         font-size: 12px;
        
    
       
      
    }
    #color_chur2{
          position: relative;
     width: 85%;
         border: 1px solid;
      border-color: white;
      
          
         font-size: 12px;
       
    }
  
  #size_chur1{
        position: relative;
      width: 13%;
       margin-left: 1.5%;
        border: 1px solid;
           border-color: white;
         font-size: 12px;
    
       
      
    }
    #size_chur2{
          position: relative;
     width: 85%;
      border: 1px solid;   
      border-color: white;
       
         font-size: 12px;
       
    }
  
  
  
    
    #kod_chur1{
          position: relative;
      width: 13%;
       margin-left: 1%;
        border: 1px solid;
           border-color: white;
         font-size: 12px;
    
       
      
    }
    #kod_chur2{
          position: relative;
     width: 85%;
         border: 1px solid;
      border-color: white;
       
          
         font-size: 12px;
       
    }
  
  
    
    
    
    
    
    
    
    
    
    
    
    
    
</style>