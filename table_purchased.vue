<template>
    <section>
          <table id="table_purchase">        
            
           <tr id="tr_purchase"> 
               
               

               
               
        <td id="td_purchase1">
            <price_chur1></price_chur1>
    </td>
          <td id="td_purchase2">
              
                   <button id="boot_m" @click="decrementValue"><i id="id_m" class="fa fa-minus"  ></i></button>
             <input type="text" id="counter_chur" v-model="counter_shoaping" value="1"/>  
    
  <button id="boot_p" @click="incrementValue"><i id="id_p" class="fa fa-plus" ></i></button>
    
    </td>
          
               <td id="td_purchase3">
                   
                   <product_chur1></product_chur1>    
                   <info_purchased1></info_purchased1>
                           
    </td>
            
            
            
    </tr> 
    </table> 
        
                   <button id="boot_close">
                   <i id="id_close" class="fa fa-close"></i>
    </button>
        
    </section>
</template>

<script>
    import product_chur1 from '~/components/product_chur'
        import info_purchased1 from '~/components/info_purchased'
             import price_chur1 from '~/components/price_chur'
        
    export default {
        data () {
            return {
                counter_shoaping:0,
            }
        },
        components: {
        product_chur1,
            info_purchased1,
              price_chur1
        
        },
        
         methods: {
   
    incrementValue() {
      this.counter_shoaping++;
    },
    decrementValue() {
      this.counter_shoaping--;
    }
  
  }   
        
    }
</script>

<style>
    
    
    #table_purchase{
        position: relative;
     margin-left: 10%;
        width: 81%;;
        height: 150px;
        border: 1px solid;
    
    }
    
    #td_purchase3{
        position: relative;
        width: 30%;
        height: 50px;
       border: 1px solid;
         border-color: white;
    }
      #td_purchase2{
          position: relative;
        width: 19%;
        height: 50px;
            border: 1px solid;
     padding-left: 7%;
       
            border-color: white;
          border-left-color: gainsboro;
         border-right-color: gainsboro;
    }
      #td_purchase1{
          position: relative;
        width: 27.4%;
        height: 50px;
         border: 1px solid;
           border-color: white;
            border-right-color: gainsboro;
         
    }
    
    
   
    #boot_close{
     
        position: absolute; 
        width: 2%;
        height: 160px;
        margin-top: -11.5%;
        margin-left: 10%;
    }
    
    #boot_m{
        position: relative;
        

        border-radius: 20px;
        color: white;
        background-color: gray;
    }
      #boot_p{
           position: relative;
        margin-left: 10%;
           border-radius: 20px;
          color: white;
          background-color: gray;
    }
    
    
    #counter_chur{
        position: relative;
        direction: rtl;
        width: 15%;
        border: 1px solid;
        border-color: white;
        margin-left: 8%;
    }
    
  
    
    
    
</style>