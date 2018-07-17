<template>
  
<section>
    
    <div id="bdiv_purch">
    
   <input type="text" id="bbrand_chur" value="نام برند"/>
         <input type="text" id="bname_chur1" value="نام محصول"/>
         <input type="text" id="bname_chur2" value="نام محصول"/>
         <input type="text" id="bname_chur3" value="نام محصول"/>
       <input type="text" id="bcolor_chur1" value="رنگ:"/>
         <input type="text" id="bcolor_chur2" value="نام رنگ"/>
        <input type="text" id="bsize_chur1" value="سایز:"/>
        <input type="text" id="bsize_chur2"   value="عدد سایز"/>
       <input type="text" id="bkod_chur1" value="کد:"/>
         <input type="text" id="bkod_chur2"  value="کد کالا"/>
         
        
        
        
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
    #bdiv_purch{
       
     color: black;
     
        width: 50%;
        margin-left:22.4%;
        direction: rtl;
         
        height: 140px;
     
margin-top: -25%;
       
    }
    
     
    #bbrand_chur{
          position: relative;
        width: 85%;
              margin-left: 12%;
        border: 1px solid;
           border-color: white;
        font-size: 12px;
          
    }
    
    #bname_chur1{
          position: relative;
      width: 28%;
        border: 1px solid;
           border-color: white;
         font-size: 12px;
    
       
      
    }
    #bname_chur2{
        position: relative;
     width: 28%; 
        border: 1px solid;
           border-color: white;
     
         font-size: 12px;
       
    }
    #bname_chur3{
          position: relative;
          border: 1px solid;
           border-color: white;
       
         font-size: 12px;
    margin-left: 15%;
      width: 28%;  
    }
    
    
    
    
    
    
    
     #bcolor_chur1{
           position: relative;
      width: 12%;
       margin-left: 1%;
        border: 1px solid;
           border-color: white;
         font-size: 12px;
        
    
       
      
    }
    #bcolor_chur2{
          position: relative;
     width: 85%;
         border: 1px solid;
      border-color: white;
      
          
         font-size: 12px;
       
    }
  
  #bsize_chur1{
        position: relative;
      width: 13%;
       margin-left: 1.5%;
        border: 1px solid;
           border-color: white;
         font-size: 12px;
    
       
      
    }
    #bsize_chur2{
          position: relative;
     width: 85%;
      border: 1px solid;   
      border-color: white;
       
         font-size: 12px;
       
    }
  
  
  
    
    #bkod_chur1{
          position: relative;
      width: 13%;
       margin-left: 1%;
        border: 1px solid;
           border-color: white;
         font-size: 12px;
    
       
      
    }
    #bkod_chur2{
          position: relative;
     width: 85%;
         border: 1px solid;
      border-color: white;
       
          
         font-size: 12px;
       
    }
  
  
  
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
</style>