<template>
  

<section>
    <figure >
        
        <div id="product_div"> 
       <div id="product_text">product image</div>        
        </div>   
        
          <div id="N">N%</div>
        
        <figcaption id="name_brand"><b>نام برند</b></figcaption>
        <figcaption id="name_product">نام محصول</figcaption>
        <figcaption id="price">
            <p id="price_reduction1">قیمت قبل تخفیف</p>
            <p id="price_reduction2">قیمت بعد تخفیف</p></figcaption>
        <figcaption id="toman"> تومان</figcaption>
        </figure>
    
    
    </section>


</template>

<script>
    export default {
      
    }
</script>

<style>
    figure{
       
        width: 80%;
         
        
    }
    #product_div{
        position: relative;
       
        width: 100%;
        height:240px;
        border: 1px solid;
        border-color:black;
        
       
    }
    
  
    
    #N{
       
        position: relative;
        text-align: center;
        margin-top: -130%;
        margin-left:0%;
        
       padding-top: .5%;
        font-size: 20px;
        background-color: deeppink;
        width: 25%;
        padding-top:2%;
        height: 50px;
        border: 1px solid;
        border-radius: 50%;
    }
    
    #product_text{
      font-size: 20px;
        margin-top: 40%;
        margin-left: 15%;
       z-index: -1;
    }
    
    
    
       #name_brand
    
    {position: relative;
        margin-top: 110%;
       text-align: center;
        font-size: 14px;
       
      
    }
    #name_product{
       
        text-align: center;
        color: gray;
        font-size: 14px;
        
    }
    
    
    
    
    
    #price{
     
        font-size: 10.5px;
    }
    
     #price_reduction1{
        text-align: right;
         margin-top: 2%;
        
         text-decoration:line-through;
      
    }
    #price_reduction2{
position: relative;
        text-align: left;
        margin-top: -15%;
        color: red;
        
    }
   
    
    #toman{
        position: relative;
        text-align: center;
        color: red;
margin-top: -4%;
        font-size: 14px;
       
    }
    
    
</style>