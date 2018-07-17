<template>
    <section>
        <div id="intro_purch">
            <p id="pur_1"><b>مشخصات اصلی</b></p> 
              <p id="pur_2"><b>تعداد</b></p> 
              <p id="pur_3"><b>قیمت</b></p> 
            
            <btable_purchased1></btable_purchased1>
            <btable_purchased1></btable_purchased1>
               <btable_purchased1></btable_purchased1>
             <btable_purchased1></btable_purchased1>
             <p id="pur_4">ارسال به آدرس شماره یک -شهر شماره یک -خیابان شماره یک-در تاریخ 23/2/97 ساعت 00:00</p> 
       
    </div>
        
        
    </section>
</template>

<script>
     import btable_purchased1 from '~/components/btable_purchased'
    export default {
        data () {
            return {
            }
        },
        components: {
            btable_purchased1
        }
    }
</script>

<style>
    
    #intro_purch{
        position: relative;
        position: relative;
        border: 1px solid;
        width: 100%;
        height:auto;
        text-align: center;
        
    }
    
    #pur_1{
         position: relative;
        width: 45%;
        height: 40px;
        border: 1px solid;
        margin-left: 55%;
        
    }
    
    #pur_2{
         position: relative;
         width: 20%;
         height: 40px;
        border: 1px solid;
        margin-top:-4.7%;
        margin-left: 35%;
        background-color: ghostwhite;
    }
    
    #pur_3{
         position: relative;
         width: 35%;
          height: 40px;
        margin-left: 0%;
        border: 1px solid;
        margin-top:-4.6%;
        background-color: ghostwhite;
    }
    
       #pur_4{
            position: relative;
         width: 90%;
         height: 20px;

        margin-top:.2%;
       margin-left: 3%;
           font-size: 12px;
        background-color: ghostwhite;
    }
    
    
    
</style>