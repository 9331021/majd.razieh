<template>
<section>
    <Dheader_1 :counter_of_shoping="counter"></Dheader_1>
    <search_nav3></search_nav3>
    
    <div id="part3">
        <div id="name1_big"><b>نام برند</b></div>
        <div id="name2_big"><b>نام محصول</b></div>
          <div id="name22_big"><b>نام محصول </b></div>
        <div id="name222_big"><b>نام محصول</b></div>
         <div id="price1_big">قیمت قبل خرید</div>
         <div id="price2_big">قیمت بعد خرید</div>
          
        <div id="color1_big"> : رنگ </div>
         <input type="text" id="color2_big"  placeholder="نام رنگ" value=""/>
        
        <product_sm id="product_sm1" :url_="imags[current_counter]"></product_sm>
        <product_sm id="product_sm2" :url_="imags[current_counter+1]"></product_sm>
        <product_sm id="product_sm3" :url_="imags[current_counter+2]"></product_sm>
       
        <select id="select_" placeholder="انتخاب کنید">
             <option id="selected"  > انتخاب کنید </option>
  <option id="20">20</option>
  <option id="50">50</option>
  <option id="60"> 60</option>
           
    </select>
        <p  id="guide" >راهنمای سایز</p>
        <button id="add_basket" value="افزودن به سبد خرید" v-model="counter" @click="inputClass">افزودن به سبد خرید</button>
        <button id="like"> <i class="fa fa-heart-o"> </i></button>
        <div id="zamanat1"><img id="z1" src="~assets/zamanat.png">ضمانت هفت روز بازگشت کالا</div>
        <div id="deliveri"><img id="z2" src="~assets/car.png">تحویل رایگان</div>
        <div id="zamanat2"><img id="z3" src="~assets/zamanat2.png">ضمانت اصل بودن کالا</div>
        
        <div id="property">
            <h6 id="pr1">ویژگی ها</h6>
 <ul id="pr">
     <li id="pr2">تیشرت مردانه نخی  برای استفاده روزمره </li>
     <li id="pr3"> دارای یقه گرد و اسیتن کوتاه</li>
     <li id="pr4">پارچه تیشرت  طرحدار است</li>
     <li id="pr5">فرم تیشرت معمولی است</li>
     <li v-if="seen_more" id="pr5">تهیه شده از 100%الیاف نخی</li>
     <li v-if="seen_more" id="pr6">قابل شستشو در درمای30درجه سانتی گراد</li>
     
     
    </ul>
   
        <p id="more_p" >نمایش بیشتر
     <button id="more_b" v-on:click="seen_more=!seen_more" >
        <i  v-if="!seen_more" id="more_i" class="fa fa-angle-down"></i>
          <i  v-else-if="seen_more" id="more_i" class="fa fa-angle-up"></i>
        
    </button>
            </p>
        </div>  
    </div>
    
    <div id="part4" >
         <img id="select_image" :src="require('~/assets/4.jpg')" />
          <p id="text_big">product image</p>
        
        <div id="N_big" >N%</div>
    </div>
    
    
    <div id="part5" >
         
         <button id="slide_show_prv" v-model="current_counter"  @click="show_prv">
                   <i id="slide_show_up" class="fa fa-angle-up"></i>
    </button>
        
    
        
 <button class="product_select" v-model="sel_counter" @click="select0">  
     <product_sm  class="product_smm"  :url_="imags[current_counter]" ></product_sm>
    </button>
<button class="product_select" v-model="sel_counter" @click="select1" > 
    <product_sm  class="product_smm"  :url_="imags[current_counter+1]"  ></product_sm></button>
<button class="product_select" v-model="sel_counter" @click="select2">
    <product_sm  class="product_smm"  :url_="imags[current_counter+2]"  ></product_sm></button>
<button class="product_select" v-model="sel_counter" @click="select3">
    <product_sm  class="product_smm"  :url_="imags[current_counter+3]"  ></product_sm></button>
       
    
   
        <button id="slide_show_next" v-model="current_counter" @click="show_next">
                   <i id="slide_show_down" class="fa fa-angle-down"></i>
    </button>
        
        
    
    </div>
    
      
    <detail_of_product1></detail_of_product1>
    
      
    <div id="part7">
     
        <h4 id="text_pro">محصولات مرتبط</h4> 
        
           <button id="but_angle" @click="show_prv_down">
        <i id="p-angel" class="fa fa-angle-right" ></i>
    </button>
        <product_cm  id="duc1" :url_down="imags_down[current_counter_down]"></product_cm>
        <product_cm id="duc2" :url_down="imags_down[current_counter_down+1]"></product_cm>
        <product_cm id="duc3" :url_down="imags_down[current_counter_down+2]"></product_cm>
        <product_cm id="duc4" :url_down="imags_down[current_counter_down+3]"></product_cm>
        <product_cm id="duc5" :url_down="imags_down[current_counter_down+4]"></product_cm>
        <product_cm id="duc6" :url_down="imags_down[current_counter_down+5]"></product_cm>
    <button id="but_angle1" @click="show_next_down">   
        <i id="p-angel2" class="fa fa-angle-left" ></i>
    </button>      
        
         
    </div>
    
    <div id="part8"><footer3></footer3> </div>
    
    
    
    
    
 </section>    







</template>

<script>
     import Dheader_1 from '~/components/header_1'
          import search_nav3 from '~/components/search_nav'
    import product_sm from '~/components/prouduct_sm'
         import product_cm from '~/components/product_cm'
               import footer3 from '~/components/footer'
             import detail_of_product1 from '~/components/detail_of_product'
                   
                   
    export default {
        data () {
            return {
                seen:true,
                seen1:true,
                seen_more:false,
                imags:[require('~/assets/1.jpg'),require('~/assets/2.jpg'),require('~/assets/3.jpg'),require('~/assets/4.jpg'),require('~/assets/5.jpg'),require('~/assets/6.jpg')],
                 imags_down:[require('~/assets/1.jpg'),require('~/assets/2.jpg'),require('~/assets/3.jpg'),require('~/assets/4.jpg'),require('~/assets/5.jpg'),require('~/assets/6.jpg'),require('~/assets/1.jpg'),require('~/assets/2.jpg'),require('~/assets/3.jpg')],
               sel_counter:1,
                counter:0,
                current_counter:1,
                current_counter_down:1,
                
            };
        },
        components: {
            product_sm,
            product_cm,
            footer3,
            detail_of_product1,
            search_nav3,
            Dheader_1
              
            
            
        },
        
         methods: {
    inputClass: function () {
      var x1=document.getElementById("select_").value;
          var x2=document.getElementById("color2_big").value;
          if (x2==="") {
        alert( "please wirte one color");
    }
      else if(isNaN(x1)) {
        alert( "please select one size");
    } 
        
        else {
      this.counter++;
    }
    },
              show_prv_down: function () {
             this.current_counter_down -= 1;
                  
              }
             ,
             show_next_down: function () {
             this.current_counter_down += 1;
              },
             
             
             
             
             
             
             
             show_prv: function () {
             this.current_counter -= 1;
                  
              }
             ,
             show_next: function () {
             this.current_counter += 1;
              },
               select0: function () {
             this.sel_counter=this.current_counter;
                  
                   document.getElementById("select_image").src=this.imags[this.sel_counter];
             },
             
              select1: function () {
             this.sel_counter=this.current_counter+1;
            
                  document.getElementById("select_image").src=this.imags[this.sel_counter];
               
            },
              select2: function () {
             this.sel_counter=this.current_counter+2;
                  
                    document.getElementById("select_image").src=this.imags[this.sel_counter];
                   
         },
              select3: function () {
             this.sel_counter=this.current_counter+3;
                
                  document.getElementById("select_image").src=this.imags[this.sel_counter];
                  
              }
   }
  
        
        
        
        
    }
</script>

<style>
    
         @import '../assets/font/font-awesome-4.7.0/css/font-awesome.css';
    
    #select_image{
         position: relative;
       
        width: 100%;
        height: 420px;
        z-index: -1;
        
    }
    
    
    #part3{
        position: relative;
       width: 35%;
        margin-top: 12%;
        height: 700px;
        margin-left: 10%;
       
        
    }    
    
     #part4{
          position: relative;
       width: 30%;
         margin-left: 46%;
        height: 420px;
         margin-top: -51%;
       border: 1px solid;
        
    }    
    
     #part5{
        
          position: relative;
       width: 12%;
         margin-top: -38%;
          margin-left: 76%;
        height: 620px;
        
        
         padding-top: 2.7%;
        
    }    
    
     
     #part7{
        position: relative;
       width: 100%;
        height: 250px;
         margin-top: 1%;
       
        
    }
    
    .product_smm{
        margin-left: 12%;      
    }
    
    .product_select{
        width: auto;
        background-color: white;
        border: 1px solid;
        border-color: white;
        outline-style: none;
        outline-color: white;
    }
    
    .product_select:focus{
    outline-style: none;
    }
    
    
    
    #slide_show_up{
      
        z-index: 1;
    margin-top: -13%;
        font-size: 50px;
        margin-left: 5%;
        
    }
    #slide_show_prv:focus{
      border: 1px solid;
          border-color: white;
          background-color: white;
        outline-style: none;
       
    }
    
    
    
    
      #slide_show_prv{
          position: relative;
        height: auto;
        width: auto;
          border: 1px solid;
          border-color: white;
          background-color: white;
       
    margin-top: -5%;
        margin-left: 22%;
       
    
    }
    
    

    
    
    
    
    
     #slide_show_down{
      
        z-index: 1;
    margin-top: -7%;
        font-size: 50px;
        margin-left: 3%;
         background-color: white;
        
    }
    #slide_show_next:focus{
      border: 1px solid;
          border-color: white;
          background-color: white;
        outline-style: none;
       
    }
    
    
    
    
    
    
      #slide_show_next{
          position: relative;
        height: auto;
        width: auto;
          border: 1px solid;
         border-color: white;
          background-color: white;
       
    margin-top: 3%;
        margin-left: 22%;
       
    
    }
    
    
   
    
    
    
    
    
    #text_big{
        font-size: 50px;
        
        margin-top: -70%;
        margin-left: 12%;
        display: none;
        
    }
    
    #N_big{
        width: 15%;
        height: 59px;
        text-align: center;
        padding-top: 2.5%;
        font-size: 22px;
        border-radius: 50%;
        margin-left: -.2%;
        margin-top: -108%;
        background-color:deeppink;
        border: 1px solid;
        z-index: 1;
    }
    
    #name1_big{
          position: relative;
        width: 20%;
        height: 40px;
        
        margin-left: 80%;
        direction: rtl;
    font-size: 23px;
    }
    
    
     #name2_big{
           position: relative;
        width: 20%;
        height: 40px;
       
          margin-left: 80%;
           direction: rtl;
    }
     #name22_big{
           position: relative;
        width:20%;
        height: 40px;
          margin-left: 60%;
         margin-top: -8.4%;
       
           direction: rtl;
    }
     #name222_big{
         position: relative;
        width: 20%;
        height: 40px;
         margin-top: -8.5%;
          margin-left: 40%;
           direction: rtl;
       
    }
    
    #price1_big{
        position: relative;
        margin-left: 76%;
        text-decoration: line-through;
        color: red;
    }
      #price2_big{
          position: relative;
        margin-left: 48%;
       margin-top: -5%;
    }
    
    
    #color1_big{
   
        width: 10%;
        height: 25px;
        margin-left: 88%;
    }
    
     #color2_big{
     position: absolute;
        width: 15%;
         direction: rtl;
        height: 25px;
         margin-left: 72%;
border: 1px solid;
         border-color: white;
         margin-top: -26px;
    }
   #product_sm1{
         position: relative;
       width: 30%;
       margin-left: 82%;
    }
    
    
    
    
   #product_sm2{
         width: 30%;
       margin-left: 65%;
       margin-top: -23.5%;
    }
    
   #product_sm3{
        width: 30%;
       margin-left: 48%;
       margin-top: -23.5%;
    }
    
    
    #select_{
        position: relative;
        width: 40%;
        height: 30px;
        direction: rtl;
        font-size: 16px;
        margin-left: 58%;
        margin-top: 3%;
        
    
    }
    #guide{
        width: 20%;
        direction: rtl;
          position: relative;
        font-size: 14px;
        margin-left: 40%;
        margin-top: -25px;
        
    }
    
    
    #add_basket{
        position: relative;
    width: 40%;
        margin-left: 57%;
        margin-top: -1%;
        height: 30px;
        padding-right: 5%;
        background-color: deeppink;
        border-color: deeppink;
        color: white;
        font-size: 15px;
    } 
    #like{
        position: relative;
        position: relative;
      width: auto;
        height: auto;
        font-size: 25px;
        margin-left: -50%;
        margin-top: 3.5%;
             border: 1px solid;
       border-color: white;
       background-color: white;
    }
    
    
    
    .fa-heart-o{
     color: red;
        font-size: 40px;
    }
    
    
    
    
    
    #deliveri
    {position: relative;
         direction: rtl;
        width: 50%;
        height: 20px;
        margin-top: -4%;
        font-size: 10px;
        margin-left: 48%;
        
    }
     #z2{
         position: relative;
        margin-top: 0%;
     width: 10%;
        margin-left: 2%;
        height: 20px;
    }
   #z1{
        position: relative;
        margin-top: 1%;
     width: 10%;
        margin-left: .5%;
        height: 20px;
    }
    
    
    #zamanat1{
         position: relative;
        direction: rtl;
        width: 50%;
        height: 20px;
        margin-top: 4%;
        font-size: 10px;
        margin-left: 70%;
    }
    
     #z3{
          position: relative;
        margin-top: -1%;
     width: 10%;
        margin-left: 2%;
        height: 20px;
    }
    #zamanat2{
         position: relative;
        direction: rtl;
        width: 50%;
        height: 20px;
        margin-top: -4%;
        font-size: 10px;
        margin-left: 18%;
    }
    
    
    #pr1{
        margin-left: 85%;
        margin-top: 1%;
        font-size: 15px;
    }
    
    #pr{
        list-style-type:disc;
        margin-top: 2%;
       margin-left: 0%;
        z-index: 1;
        width: 100%;
          
       height: 260px;
        direction: rtl;
        text-align: right;
    }
     #property{
      
         height: 300px; 
        margin-top: 10%;
        z-index: 1;
    }
    
    #pr2{
       
        height: 20px;
        color: black;
        width: 100%;
        text-align: right;
        font-size: 13px;
        
    }
      #pr3{
       
        height: 20px;
        color: black;
        width: 100%;
        text-align: right;
        font-size: 13px;
        
    }
      #pr4{
    
        height: 20px;
        color: black;
        width: 100%;
        text-align: right;
        font-size: 13px;
        
    }
      #pr5{
       
        height: 20px;
        color: black;
        width: 100%;
        text-align: right;
        font-size: 13px;
        
    }
    
    
      #pr6{
       
        height: 20px;
        color: black;
        width: 100%;
        text-align: right;
        font-size: 13px;
        
    }
    
    
    
    #more_p{
      
       position: relative;
            width: 18%;
        font-size:14px; 
        height: 20px;
        color: black;
        margin-left: 5%;
        margin-top: -15%;


    }
   #more_i{
       position: relative;
        margin-top: -43%;
        margin-left: 0%;
       font-size: 20px;
    }
    
    #more_b{
      position: relative;
        width: auto;
        height: auto;
        margin-top: -60%;
        color: black;
        margin-left: 12%;
         border: 1px solid;
        background-color: white;
        border-color: white;
        padding-bottom: 1%;
        
    }
    #more_b:focus{
      outline-color: white;
       outline-style: none;
         outline-color: white;
         
    }
     
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
      
    #part7{
         position: relative;
        direction: rtl;
        background-color: ghostwhite;
        padding-right: 6%;
    }
#text_pro{
     position: relative;
    float: right;
    margin-top: 1%;
    font-size: 18px;
    margin-right: 7%;
       
        
    }
    
 
    #p-angel{
       position: relative;
       font-size: 60px;
      
       
        margin-top: 4%;
    
     
    
    }
   
    
    
    #p-angel2{
    
        position: relative;
    
       font-size: 60px;
       
  
    }
   
    
    
   #but_angle1{
       position: relative;
         width: auto;
        height: auto;
        border: 1px solid;
        margin-left: 15%;
         border: 1px solid;
        margin-top: -1%;
       border-color: ghostwhite;
       background-color: ghostwhite;
      
    } 
    
  
   #but_angle{
       position: relative;
         width: auto;
        height: auto;
        border: 1px solid;
        margin-left: 85%;
        margin-top: 2%;
       border: 1px solid;
       border-color: ghostwhite;
       background-color: ghostwhite;
       
    }
     #but_angle:focus{
    outline-style: none;
    }
     #but_angle1:focus{
    outline-style: none;
    }
    
    
     
    
    #duc1{
        width: 10%;
        height: 40px;
        margin-right: 20%;
        margin-top: -7%;
    }
    
     #duc2{
        width: 10%;
        height: 40px;
        margin-right: 30%;
        margin-top: -3.8%;
    }
     #duc3{
        width: 10%;
        height: 40px;
        margin-right: 40%;
        margin-top: -3.8%;
    }
     #duc4{
        width: 10%;
        height: 40px;
        margin-right: 50%;
        margin-top: -3.8%;
    }
     #duc5{
        width: 10%;
        height: 40px;
        margin-right: 60%;
        margin-top: -3.8%;
    }
     #duc6{
        width: 10%;
        height: 40px;
        margin-right: 70%;
        margin-top: -3.8%;
    }
    
    
    
    
    #part8{
      padding-top: .2%;
        width: 100%;
        height: 200px;
        background-color:gainsboro;;
        margin-top: 2.5%;
    }
    
    
    
    
    
    
    
    
    
    
    
    
    
</style>