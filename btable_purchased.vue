<template>
    <section>
          <table id="btable_purchase">        
            
           <tr id="btr_purchase"> 
               
               

               
               
        <td id="btd_purchase1">
            <bprice_chur1></bprice_chur1>
    </td>
          <td id="btd_purchase2">
              
                   <input type="text" id="bcounter_chur"  value="1"/>  
    
         
    
    </td>
          
               <td id="btd_purchase3">
                   
                   <bproduct_chur1></bproduct_chur1>    
                   <binfo_purchased1></binfo_purchased1>
                           
    </td>
            
            
            
    </tr> 
    </table> 
        
        
    </section>
</template>

<script>
    import bproduct_chur1 from '~/components/bproduct_chur'
        import binfo_purchased1 from '~/components/binfo_purchased'
             import bprice_chur1 from '~/components/bprice_chur'
        
    export default {
        data () {
            return {
            }
        },
        components: {
        bproduct_chur1,
            binfo_purchased1,
              bprice_chur1
        
        }
        
    }
</script>

<style>
    
    
    #btable_purchase{
        margin-top: -1.5%;
     position: relative;
        width: 100%;
        height: 160px;
         background-color: white;
    }
    
    #btd_purchase3{
         position: relative;
        width: 45%;
        height: 65px;
       border: 1px solid;
         border-color: black;
         border-right-color: black;
         border-left-color: black;
        
    }
      #btd_purchase2{
           position: relative;
        width: 20%;
        height: 65px;
         border: 1px solid;
          border-color: black;
          border-right-color: black;
           border-left-color: black;
             
    }
      #btd_purchase1{
           position: relative;
        width: 35%;
        height: 65px;
      
        border: 1px solid;
           border-color: black;
           border-right-color: black;
           border-left-color: black;
          
    }
    
    
   
 

    
    #bcounter_chur{
        
        direction: rtl;
        width: 15%;
        border: 1px solid;
        border-color: white;
        margin-left: -2%;
    }
    
    
    
    
    
</style>