<template>
<section>
    
    
        <Cheader_1 counter_of_shoping="1"></Cheader_1>
            <search_nav2></search_nav2>
    <div id="part11"> 
    <info1  id="last_name" sub="نام و نام خانوادگی" pla="برای مثال راضیه معینی مجد" ></info1>
         <info_number1  id="phone_" sub="شماره تلفن همراه" pla="09135011305" ></info_number1>
         <date1  id="birth_day" sub="تاریخ تولد " pla="date piker is here" ></date1>
         <info_pass1  id="curr_pass" sub="رمزعبور فعلی" pla="" ></info_pass1>
        <div id="img_profile"> <image_profile1></image_profile1></div>
       
         <info_pass1  id="new_pass" sub="رمزعبور جدید" pla="" v-model="passinput1" @blur="check_password1"  ></info_pass1>
         <info_number1  id="phone_sabet" sub="شماره تلفن ثابت" pla="2742114" ></info_number1>
    <info_number1  id="card_16" sub="شماره کارت 16 رقمی " pla="اختیاری" ></info_number1>
        <info1  id="city" sub="شهر" pla="برای مثال کرمان" ></info1>
         <info_pass1  id="repaet_pass" sub="تکرار رمزعبور فعلی" pla="" v-model="passinput2"  @blur="check_password2" ></info_pass1>
    <input id="save_1" type="button" placeholder="ثبت تغیرات" value="ثبت تغیرات "  @click="check_password"  />
    
    
    </div>

    
    
    <div id="part22">
    
   <p id="but" >
       <button  id="but_address"   v-on:click="seen=!seen" ><b>آدرس ها</b></button>
    </p>
        <span id="close_address" v-if="seen"> <i id="img_left" class="fa fa-angle-left"></i></span>
         
        <div v-else-if="!seen" id="open_address"><i  id="img_down" class="fa fa-angle-down"></i>
    
     <div id="addres_part">
         <table_address1></table_address1>
           <table_address1></table_address1>
           <table_address1></table_address1>
           <input id="save_2" type="button" placeholder="ثبت ادرس جدید" value="ثبت آدرس جدید"/>
    </div>
    
    </div>
            

    </div>
     
    <div id="part33">
        
        <p id="but1" >
       <button  id="but_order"  v-on:click="seen1=!seen1" ><b> سفارشات</b></button>
            
    </p>
        
        
        
        <span v-if="seen1"> <i id="img_left1" class="fa fa-angle-left"></i></span>
         
        <div v-else-if="!seen1" id="open_address1"><i  id="img_down1" class="fa fa-angle-down"></i>
     <table_order1 id="table_order111"></table_order1>
     <div id="order_part">
        <save_order_example1></save_order_example1>
         <save_order1></save_order1>
         <save_order1></save_order1>
         
         
         
    </div>
    
    </div>

    
    </div>
    <footer5></footer5>

    </section>

</template>

<script>
    import info_pass1 from '~/components/info_pass'
          import info1 from '~/components/info'
               import date1 from '~/components/date'
        import info_number1 from '~/components/info_number'
             import image_profile1 from '~/components/image_profile'
                  import table_address1 from '~/components/table_address'
                        import footer5 from '~/components/footer'
                      import table_order1 from '~/components/table_order'
                          import save_order1 from '~/components/save_order'
                              
                              
                              
                               import search_nav2 from '~/components/search_nav'
                          import Cheader_1 from '~/components/header_1'
                              
                              
                               import save_order_example1 from '~/components/save_order_example'
    export default {
        data () {
            return {
                 seen: true,
                seen1:true,
                passinput1:'',
                passinput2:''
            }
        },
        components: {
            info1,
            date1,
            info_pass1,
            info_number1,
            image_profile1,
            table_address1,
            table_order1,
            save_order1,
            save_order_example1,
            footer5,
            Cheader_1,
            search_nav2
        },
            methods: {
        check_password1 (value) {
  this.passinput1=value;
          
    } ,
      
                    check_password2(value) {
  this.passinput2=value;
            
    },
                
                
                     check_password() {
      
                         if(this.passinput2!==this.passinput1){
            alert("invalid pasword please tyr it");
    }       
            
                     }
                
                
    }
    }
  
        
        

</script>

<style>
    @import '../assets/font/font-awesome-4.7.0/css/font-awesome.css';

    
    
    
    
    
    
    
    #part11{
        margin-top: 2%;
border: 1px solid;
        width: 91.5%;
        margin-left: 5%;
        height: 500px;
    }
    

    
    #last_name{
         position: absolute;
        margin-top: 1%;
      margin-left: 64%;
        width: 25%;
          border: 1px solid;
    }
    
    #phone_{
         position: absolute;
         margin-top: 7%;
      margin-left: 64%;
        width: 25%;
          border: 1px solid;
    }
    
    
    #birth_day{
         position: absolute;
         margin-top: 13%;
      margin-left: 64%;
        width: 25%;
          border: 1px solid;
    }
    #curr_pass{
         position: absolute;
         margin-top: 25%;
      margin-left: 64%;
        width: 25%;
        border: 1px solid;
    }
    #new_pass{
         position: absolute;
         margin-top: 25%;
      margin-left: 33%;
        width: 25%;
          border: 1px solid;
    }
    #city{
         position: absolute;
        margin-top: 1%;
        margin-left: 2%;
        width: 25%;
        text-align: right;
        direction: rtl;
          border: 1px solid;
    }
    
    
    
    #img_profile{
        position: absolute;
        width: 25%;
        height: 280px;
margin-left: 33%;
        border: 1px solid;
        background-color:ghostwhite;
          border: 1px solid;
    }
    
    
      #card_16{
         position: absolute;
        margin-top: 13%;
        margin-left: 2%;
        width: 25%;
        text-align: right;
        direction: rtl;
          border: 1px solid;
    }
    
  
    
    #phone_sabet{
         position: absolute;
        margin-top: 7%;
        margin-left: 2%;
        width: 25%;
        text-align: right;
        direction: rtl;
          border: 1px solid;
    }
    
    
    
    
    #repaet_pass{
         position: absolute;
        margin-top: 25%;
        margin-left: 2%;
        width: 25%;
        text-align: right;
        direction: rtl;
          border: 1px solid;
        
    }
    
    #save_1{
        width: 25%;
        height: 45px;
        border-radius: 25px;
        background-color: blue;
        color: white;
        text-align: center;
        font-size: 20px;
    margin-left: 38%;
        margin-top: 38%;
    }
      #save_2{
        width: 14%;
        height: 35px;
        border-radius: 25px;
        background-color: blue;
        color: white;
        text-align: center;
        font-size: 15px;
    margin-left: 0%;
        margin-top: 10%;
    }
    
    
    
    
    
    
    
    
    
    
    
    
     #part22{
        border: 1px solid;
        width: 100%;
        height: auto;
    }
    
        #addres_part{
        border: 1px solid;
            border-color: white;
        width: 90%;
        height:auto;
            margin-left: 5%;
            margin-top: 4.5%;
              
    }
    
    
    #part33{
        border: 1px solid;
        width: 100%;
        height: auto;
    }
    
    
    
    
    #order_part{
        
        border: 1px solid;
        width: 90%;
        margin-top: -1%;
        margin-left: 5%;
        border-color: blue;
        height:auto;
        background-color: ghostwhite;
    }   
    
     
    #but_address{outline-style: none;}
     #but_order{outline-style: none;}
    
    
    
    
    #but_address{
        position: relative;
        width: 60%;
        height: 30px;
        background-color: white;
        border: 1px solid;
        border-color: white;
color: black;
        font-size: 20px;
        margin-top: 25%;
        margin-right: -5%;
        
    }
    #but{
        padding-top: .5%;
        width: 12%;
        direction: rtl;
        height: 40px;
       
        margin-left: 85%;
       
            
    }
    
  
      #img_left{
          
      
          position: relative;
           z-index: 1;
          margin-top: -1.5%;
          
     margin-left: 84.5%;
        font-size: 15px;
    }
    
      #img_down{
          position: relative;
           z-index: 1;
        
          margin-top: -4.9%;
          margin-left: 84.5%;
          
        font-size: 15px;
    }
    
    
    #but_order{
        width: 60%;
        height: 30px;
        background-color: white;
        border: 1px solid;
        border-color: white;
color: black;
        font-size: 20px;
        margin-top: 26%;
        margin-left: 15%;
    }
    #but1{
        padding-top: .2%;
        width: 12%;
        direction: rtl;
        height: 40px;
    
        margin-left: 83.5%;
       
            
    }
    
  
      #img_left1{
          
      
          position: relative;
           z-index: 1;
          margin-top: -1%;
          
     margin-left: 84.5%;
        font-size: 15px;
    }
    
      #img_down1{
          position: relative;
           z-index: 1;
        
          margin-top: -4%;
          margin-left: 84.5%;
          
        font-size: 15px;
    }
    
    #table_order111{
    
        margin-top: -6%;
        margin-left: 5%;
    }
    
    
    
    
    #part44{
        width: auto;
        
        height: auto;
       
    }
  
    
    
    
    
    
    
</style>