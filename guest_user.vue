<template>
<section>
    <Wheader>
   
        
        
 </Wheader>       
        
    
    
<!-- big letter -->    
    <div id="big_letter">
     <img id="big_letter2" src='~assets/big_letter.png' />   
        <div id="content">محتوای سایت </div>
  
    </div>
        
        
        
        
        
<!--footer-->
 
     <footer1>
    </footer1>
        
      <!-- end footer -->

    </section>
</template>


<script>    
    import Wheader from '~/components/header'
         import footer1 from '~/components/footer'
    export default {
        components: {
         Wheader,
            footer1
            
        }
    };
</script>






<style>
    
   

    
    
    
    
    
    
    #big_letter{
        border: 1px solid;
        border-color: black;
        width: 53%;
      height: 394px;
        margin-left: 24%;
        margin-top: 4%;
       
        z-index: -1;
        
    }
    
    #big_letter2{
     z-index: -1;
        margin-left: 2.3%;
        margin-top: 2.5%;
        
        
    }
    #content{
        position: absolute;
        margin-top: -15%;
        border: 1px solid;
        border-color: black;
        text-align: center;
        width: 20%;
        height: 40px;
        background-color: white;
        margin-left: 16%;
       
    }
    

   
 
    </style>