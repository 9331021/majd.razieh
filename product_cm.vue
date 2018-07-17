<template>
  

<section>
    <figure >
        
        <div id="product_div"> 
      <!-- <div id="product_text">product image</div> -->
              <img id="img_down" :src="url_down"/>
       
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
         props:['url_down'],
      
    }
</script>

<style>
    figure{
       
        width: 80%;
         
        
    }
    #product_div{
        position: relative;
        margin-top: 8%;
        width: 90%;
        height:120px;
        border: 1px solid;
        border-color:black;
       
        
       
    }
    #img_down{
        width: 100%;
        height:120px;
      
  border: 1px solid;
    }
  
    
    #N{
       
        position: absolute;
        text-align: center;
        margin-top: -10%;
        margin-left:20%;
       padding-top: .5%;
        font-size: 10px;
        background-color: deeppink;
        width: 2%;
        height: 30px;
        border: 1px solid;
        border-radius: 50%;
        text-align: center;
    }
    
    #product_text{
      font-size: 12px;
        margin-top: 45%;
        margin-left: 2%;
        text-align: center;
       z-index: -1;
    }
    
    
    
       #name_brand
    {
       text-align: center;
        font-size: 14px;
       
      
    }
    #name_product{
       
        text-align: center;
        color: gray;
        font-size: 10px;
        
    }
    
    
    
    
    
    #price{
     
        font-size: 6.5px;
    }
    
     #price_reduction1{
        text-align: right;
         margin-top: 2%;
        
         text-decoration:line-through;
      
    }
    #price_reduction2{
        position: relative;
        text-align: left;
        margin-top: -24%;
        margin-left: 0%;
        margin-right: 1%;
        color: red;
        
    }
   
    
    #toman{
        text-align: center;
        color: red;
    font-size: 10px;
        margin-top: -2%;
       
    }
    
    
</style>