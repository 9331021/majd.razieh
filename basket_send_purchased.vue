<template>
    <section>
        <div id="intro_purch">
            <p id="pur_1"><b>مشخصات اصلی</b></p> 
              <p id="pur_2"><b>تعداد</b></p> 
              <p id="pur_3"><b>قیمت</b></p> 
            
           
           
       
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
    
    #intro_purch{
        
       
     position: relative;
        width: 100%;
        height:40px;;
        text-align: center;
         background-color: ghostwhite;
        
    }
    
    #pur_1{
        position: relative;
        width: 32%;
        height: 40px;
        border: 1px solid;
        margin-left: 59%;
         background-color: ghostwhite;
        border-color: gainsboro;
    }
    
    #pur_2{
         width: 20%;
         height: 40px;
        border: 1px solid;
        margin-top:-4.1%;
        margin-left: 39%;
        background-color: ghostwhite;
        border-color: gainsboro;
    }
    
    #pur_3{
        position: relative;
         width: 29%;
          height: 40px;
        margin-left: 10%;
        border: 1px solid;
        margin-top:-4.2%;
        background-color: ghostwhite;
        border-color: gainsboro;
    }
    
    
    
</style>