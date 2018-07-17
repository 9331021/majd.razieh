<template>
    <section>
        <ul id="input_order1">
            
   
         <li id="input_order11">
            <input id="input_11" type="number"  value="111"/> 
            </li>
            
          <li id="input_order12">
            <input id="input_12" type="number"  value="222"/> 
            </li>
            
            
             <li id="input_order13">
            <input id="input_13" type="text" value="333" /> 
            </li>
            
             <li id="input_order14">
            <input id="input_14" type="datetime-local"  value="444"/> 
            </li>
            
             <li id="input_order15">
            <input id="input_15" type="text"  value="تحویل داده شده"/> 
            </li>
             <li id="input_order16">
            <input id="input_16" type="text"  value="666"/> 
            </li>
            
             <li id="input_order17">
                 <button id="input_17" type="button"  v-on:click="seen=!seen">
                     <i v-if="seen" id="top_17" class="fa fa-angle-up"> </i>
    
                     <i v-else-if="!seen" id="top_17" class="fa fa-angle-down"></i>
                         
    
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
    
#input_order1{
    position: relative;
        color: black;
        background-color:lightgrey;
    border: 1px solid;
    width: 100%;
margin-left:  0%;
    height: 35px;
    text-align: center;
    margin-top: .8%;
   
    }
    
    #input_order11{
        width: 10%;
        position:absolute;
        margin-top:.2%;
        margin-left: 86%;
       height: 28px;
        border: 1px solid;
         background-color: lightgrey;;
        border-color: lightgrey;

    }
    
    #input_11{
        width: 45%;
        height: 28px;
        font-size: 16px;
        position:absolute;
        text-align: center;
       margin-left: -33%;
       
        border: 1px solid;
         background-color: lightgrey;;
        border-color: lightgrey;

    }
    
    
    
    
    
    
    
    
    
    
    
    
    
    
     #input_order12   {
         width: 10%;
         height: 28px;
          position:absolute;
        margin-top:.2%;
        margin-left: 73%;
         background-color: blue;
         border: 1px solid;
          background-color: lightgray;;
        border-color: lightgray;

    }
    
    #input_12   {
         width: 70%;
        height: 28px;
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
    
    
    
    
    
    
    
    
    
    
         #input_order13   {
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

   #input_13{
       z-index: 1;
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

    
    
    
    
    
    
    
    
         #input_order14   {
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
    
         #input_14   {
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
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    

         #input_order15   {
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
    
         #input_15   {
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
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
     #input_order16   {
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
    
    
     #input_16   {
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
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
     #input_order17   {
         width: 11%;
          position:absolute;
        margin-top:.2%;
        margin-left: -2%;
         background-color: blue;
         border: 1px solid;
          background-color: lightgrey;;
        border-color: lightgrey;

    }
    

    #input_17{
        border: 1px solid;
          background-color: lightgrey;
        border-color: lightgrey;
        
    }
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
</style>