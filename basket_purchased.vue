<template>
    <section>
        <Aheader_1 v-model="counter_of_shoping"></Aheader_1>
 
   <div id="example1">
       <div id="line_aqua"></div>
<div id="example2">
<i id="truck" class="fa fa-truck"></i>

    <p id="send_info">اطلاعات ارسال </p>
</div>
       
       
       <div id="example3">
<i id="arrow" class="fa fa-cart-arrow-down"></i>
<p id="send_basket">سبد ارسال  </p>

</div>
       
       
       
        
       <div id="example4">
<i id="file" class="fa fa-file-o"></i>
           <p id="detail_info"> جزییات پرداخت </p>


</div>
       
</div>
    
        <div id="part10">
    
        
            <basket_send_purchased1></basket_send_purchased1>
            
            <table_purchased1></table_purchased1>
        
     </div>   
        
        
        <button id="save_next" value="ثبت و مرجله بعد">
            <b> <a id="save_next2" href="#"> ثبت و مرحله بعد </a></b>    
    </button>
        
        <footer6></footer6>
    
    </section>




</template>

<script>
    
      import footer6 from '~/components/footer'
           import basket_send_purchased1 from '~/components/basket_send_purchased'
               import table_purchased1 from '~/components/table_purchased'
                    import Aheader_1 from '~/components/header_1'
        
    export default {
        data () {
            return {
            }
        },
        components: {
            basket_send_purchased1,
            footer6,
            table_purchased1,
            Aheader_1
        }
    }
</script>

<style>
    
      @import '../assets/font/font-awesome-4.7.0/css/font-awesome.css';
    
    
        
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
#example1 {
    border: 2px solid ;
    border-color: gainsboro;
  margin-top: 10%;
  
    height:0px;
    direction: rtl;
    
}
    ul{
        margin-top: -.1%;
    }

    #line_aqua{
        position: absolute;
         border: 2px solid ;
    border-color: aqua;
  
  width: 25%;
        margin-top: -.1%;
    height:0px;
    direction: rtl;
    }  
    
    
    
#example2{

width:8%;
 border: 2px solid gainsboro;
 height:45px;
 border-top-color:white;
 
 border-bottom-left-radius: 40px;
 border-bottom-right-radius: 40px;
 padding-left:2%;
    margin-right: 45%;
   direction: rtl;
    margin-top: -.2%;
     background-color: white;
    
}




#truck{
    position: relative;
        color: black;
    z-index: 1;
font-size:40px;
    
    margin-right: 3%;
 direction: rtl;
    margin-top: -1%;
    }

    
    
    
    #example3{

width:8%;
 border: 2px solid gainsboro;
 height:40px;
 border-top-color:white;
           border-right-color: aqua;
         border-bottom-color: aqua;
        border-left-color: aqua;
 border-bottom-left-radius: 40px;
 border-bottom-right-radius: 40px;
 padding-left:2%;
    margin-right: 25%;
        margin-top: -3.3%;
   direction: rtl;
         background-color: white;
        padding-bottom: 3%;
}




#arrow{
   
     position: relative;
   margin-right: 3%;
     margin-top: -2%;
    
font-size:40px;
 direction: rtl;
        color: black;
    }

    
    
        #example4{

width:8%;
 border: 2px solid gainsboro;
 height:43px;
 border-top-color:white;;
 border-bottom-left-radius: 40px;
 border-bottom-right-radius: 40px;
 padding-left:2%;
    margin-right: 65%;
        margin-top: -3.3%;
            background-color: white;
   direction: rtl;
            margin-bottom: 3%;
}
    




#file{
      position: relative;
    margin-left: 15%;
    color: black;
font-size:30px;
 direction: rtl;
    margin-top: 2%;
    margin-bottom: 3%;
   
    }

    
    
    
    
    
    
    

    footer6{
    
        margin-top: 40%;
         margin-bottom: -80%;
        
    }
    
    
    #detail_info{
        position: relative;
        font-size: 12px;
        margin-top: 2.5%;
       
        margin-right: 1%;
        padding-top: 4%;
    }
    #send_info{
         position: relative;
        font-size: 12px;
        margin-top: 3%;
        margin-right: 1%; 
        
    }
    
    #send_basket{
          position: relative;
        font-size: 13px;
        margin-top: 3%;
        margin-right: 1%;
        
    }
    
    #part10{
        margin-top: 10%;
        height: auto;
       
    }

    
    #save_next{
        margin-top: 5%;
        width: 18%;
        height: 40px;
        font-size: 17px;
        background-color: blue;
        
        border: 1px solid;
        border-color: blue;
        border-radius: 20px;
    margin-left: 10%;
        color: white;
    
    }
    
    #save_next2{
        color: white;
         font-size: 17px;
    }
    
    
    
</style>