<template>
    <section>
        <ul id="input_order2">
            
   
         <li id="input_order21">
            <input id="input_21" type="number"  value="111"/> 
            </li>
            
          <li id="input_order22">
            <input id="input_22" type="number"  value="222"/> 
            </li>
            
            
             <li id="input_order23">
            <input id="input_23" type="text" value="333" /> 
            </li>
            
             <li id="input_order24">
            <input id="input_24" type="datetime-local"  value="444"/> 
            </li>
            
             <li id="input_order25">
            <input id="input_25" type="text"  value="تحویل داده شده"/> 
            </li>
             <li id="input_order26">
            <input id="input_26" type="text"  value="666"/> 
            </li>
            
             <li id="input_order27">
                 <button id="input_27" type="button"  v-on:click="seen=!seen">
                     <i v-if="seen" id="top_27" class="fa fa-angle-up"> </i>
    
                     <i v-else-if="!seen" id="top_27" class="fa fa-angle-down"></i>
                     
    
    </button>
            </li>
           
            

            
</ul>


        
        

 <purchased_products1  v-if="!seen"></purchased_products1>






    </section>
</template>

<script>
     import purchased_products1 from '~/components/purchased_products'
    export default {
        data () {
            return {
                seen:true,
            }
        },
        components: {
            purchased_products1
        }
    }
</script>

<style>
    
#input_order2{
    position: relative;
        color: black;
        background-color:lightgrey;
    border: 1px solid;
    width: 100%;
margin-left:  0%;
    height: 35px;
    text-align: center;
    margin-top: 2.8%;
   
    }
    
    #input_order21{
        width: 10%;
        position:absolute;
        margin-top:0%;
        margin-left: 86%;
       height: 30px;
        border: 1px solid;
         background-color: lightgrey;;
        border-color: lightgrey;

    }
    
    #input_21{
        width: 45%;
        height: 30px;
        font-size: 16px;
        position:absolute;
        text-align: center;
       margin-left: -33%;
       
        border: 1px solid;
         background-color: lightgrey;;
        border-color: lightgrey;

    }
    
    
    
    
    
    
    
    
    
    
    
    
    
    
     #input_order22   {
         width: 10%;
         height: 30px;
          position:absolute;
        margin-top:0%;
        margin-left: 73%;
         background-color: blue;
         border: 1px solid;
          background-color: lightgray;;
        border-color: lightgray;

    }
    
    #input_22   {
         width: 70%;
        height: 30px;
          position:absolute;
        margin-top:0%;
        margin-right: 10%;
        margin-left: -44%;
        font-size: 16px;
        text-align: center;
         background-color: blue;
         border: 1px solid;
          background-color: lightgray;;
        border-color: lightgray;

    }
    
    
    
    
    
    
    
    
    
    
         #input_order23   {
             width: 16%;
              position:absolute;
        margin-top:0%;
           color: black;
        margin-left: 34%;
            
         background-color: blue;
         border: 1px solid;
              background-color: lightgray;;
        border-color: lightgray;

    }

   #input_23{z-index: 1;
             width: 75%;
       margin-left: -10%;
       height: 30px;
       text-align: center;
              position:absolute;
        margin-top:.2%;
           color: black;
        font-size: 16px;
         background-color: blue;
         border: 1px solid;
              background-color: lightgray;;
        border-color: lightgray;

    }

    
    
    
    
    
    
    
    
         #input_order24   {
             width: 17%;
              position:absolute;
        margin-top:.2%;
             height: 25px;
        margin-left: 54.5%;
         background-color: blue;
         border: 1px solid;
              background-color: lightgray;;
        border-color: lightgray;

    }
    
         #input_24   {
             width: 100%;
              position:absolute;
        margin-top:.2%;
        margin-left: -43%;
         background-color: blue;
         border: 1px solid;
             font-size: 16px;
             text-align: center;
             direction: ltr;
              background-color: lightgray;;
        border-color: lightgray;

    }
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    

         #input_order25   {
             width: 14%;
              position:absolute;
        margin-top:.2%;
             height: 30px;
        margin-left: 20%;
         background-color: blue;
         border: 1px solid;
              background-color:lightgray;;
        border-color: lightgray;

    }
    
         #input_25   {
             width: 60%;
              position:absolute;
        margin-top:.2%;
        height: 25px;
             text-align: center;
             font-size: 14px;
         background-color: blue;
         border: 1px solid;
              background-color: lightgray;;;
        border-color: lightgray;
             color: blue;

    }
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
     #input_order26   {
         width: 15%;
         height:25px;
          position:absolute;
        margin-top:.2%;
        margin-left: 4%;
         background-color: blue;
         border: 1px solid;
          background-color: lightgrey;;
        border-color: lightgrey;

    }
    
    
     #input_26   {
         text-align: center;
         width: 72%;
         height:25px;
          position:absolute;
        margin-top:.2%;
        margin-left:0%;
         background-color: blue;
         border: 1px solid;
          background-color: blue;;
        border-color: blue;
         border-radius: 15px;
         color: white;

    }
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
     #input_order27   {
         width: 11%;
          position:absolute;
        margin-top:.2%;
        margin-left: -2%;
         background-color: blue;
         border: 1px solid;
          background-color: lightgrey;;
        border-color: lightgrey;

    }
    

    #input_27{
        border: 1px solid;
          background-color: lightgrey;
        border-color: lightgrey;
        
    }
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
</style>