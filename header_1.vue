<template>
    
<section>
   <div id="top" >
<div id="top2">

    <select id="login">
  <option id="Edit">تغیرات</option>
  <option id="Exit">خروج</option>
  <option id="user" selected>راضیه معینی</option>
    </select>
   <a id="basket" href='basket_purchased.vue' v-model="counter_of_shoping">سبد خرید </a>
  
    <i  id="basket2" class="fa fa-shopping-cart"><div id="ci_basket" >{{counter_of_shoping}}</div></i>
    <a id="order" href="join.html">پیگیری سفارشات </a>
    <img id="order2" src='~assets/order2.png' />
    </div>          
<div class="titr"> Clothser</div>

<ul id="ul_nav">
  <li id="nav_man"><a href="#">مردانه  </a> </li>
  <li  id="nav_woman"><a href="#">زنانه </a></li>
  <li id="nav_child"><a href="#">بچگانه </a></li>
  <li id="nav_sport"><a href="#">ورزشی</a></li>
  <li id="nav_price"><a href="#">تخفیف </a></li>
  <li id="nav_brand"><a href="#">برندها </a></li> 
</ul>

        
        
<div id="line"> </div>   

    
    </div>
    
    
    </section>
</template>

<script>
    export default {
        props:['counter_of_shoping'],
        data () {   
            return {
                counter_of_shoping:0,
            }
        },
        components: {
        }
    }
</script>

<style>

    
 
        #top{
	width:100%;
            height: 150px;
            margin-left: 0%;
	margin-top:2%;
  
    }
 
    #login{
	float:right;
	direction: rtl;
        font-size: 14px;
        border: 1px solid;
        
	text-align:center;
	height:90%;
	width:26%;
	color:#270000;
	border-color: white;
   margin-top: 1%;
	margin-right:-1.5%;
        
	text-decoration:none;
 padding-top: .7%;
 
}
 
    
#basket{
    
    
		float:right;
	direction:rtl;
   
	text-align:center;
	height:90%;
    padding-top: .7%;
	width:15.%;
	color:black;
     background-color:white;
	margin-right: 5%;
    margin-top: 3.3%;
font-size: 14px;
	
	text-decoration:none;
	
}
    #top2{
 position: relative;
        width: 32%;;
    direction: rtl;
        height: 50px;
        margin-left:63%;
margin-top: .5%;
       
       
    }
 


#login:hover {
    background: white;
    color: blue;
}
#basket2
    {width: 6%;
        
       
       font-size: 17px;
        height: 50%;
        margin-top: 5%;
        margin-left: 51%;    
        
    }
    
    
    #ci_basket{
        position: relative;
        border: 1px solid;
        width: 100%;
        height: 25px;
        background-color: deeppink;
        margin-right: 23%;
        border-radius: 35px;
      color: white;
        margin-top: -10%;
        text-align: center;
        
    }
    
    
#order{
		float:right;
	direction:rtl;
   
	text-align:center;
	height:90%;
	width:28%;
    padding-top: 1%;
	color:black;
     background-color:white;
margin-top:-10%;
	margin-right:50%;
    font-size: 14px;
	text-decoration:none;
	
}
   
    #order2{
         z-index: 1;
      
        margin-top: -14%;
margin-right: 0%;
        margin-left: 17%;
      
           
    }
    
    
    .titr{
    width: 15%;
   font-size: 25px;
    text-align: center;
    font-family:sans-serif;
    color: black;
      
    margin-left:40%;
        margin-top: -3%;
     text-shadow : 3px 3px 3px gray ; 
}
   
    
   

    

   ul li {
	float:right;
	position:relative;
	text-align:center;
	width:120px;
       list-style-type:none;
       margin-left: 1%;
       text-decoration: none;
       border-bottom-color: white;
       margin-top: 4%;
       margin-left: 1%;
      
  
}
    
    ul li a{
         text-decoration: none;
        color: black;
     
    }
    
    #nav_man{
        margin-left: 1%;
       
        
    }
    
    #nav_woman{
        margin-left: 1%;
         
    }
    #nav_child{
        margin-left: 1%;
        
    }
    #nav_spot{
        margin-left: 1%;
    }
    
    #nav_price{
        margin-left: 1%;
    }
    #nav_brand{
       
        margin-left: 1%;
    }
    
    #ul_nav{
        position: relative;
      
       
        width: 70%;
        height: 70px;
        margin-left: 15%;
        margin-top: 2%;
        padding-right: 5%;
        text-align: right;
    }
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    #line{
        
        width: 90%;
       border: solid 1px;
    border-color: white;
border-bottom-color: black;
        margin-top: 1.5%;
        margin-left: 5%;
        
    }
    
    
      
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
</style>