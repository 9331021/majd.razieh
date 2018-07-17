<template>
    <section>
     <ul id="daste1">
  <li id="first">
       <button id="img_left11" type="button"  v-on:click="seen=!seen">
                     <i v-if="seen" id="left_l11" class="fa fa-angle-left"> </i>
    
                     <i v-else-if="!seen" id="down_d11" class="fa fa-angle-down"></i>
                         
    </button>
      
&nbsp{{  name_of_group   }}
      
      
        <div v-if="!seen" id="last_list1">
  
            <Aasidegray111 name_of_group="نایک 2"></Aasidegray111>
            
  </div>
      
      
      
      
    </li>
         
 
         
         
    </ul>  

    </section>

</template>

<script>
     import Aasidegray111 from '~/components/asidegray111'
    export default {
        props:['name_of_group'],
        data () {
            return {
                seen:true
            }
        },
        components: {
            Aasidegray111
        }
    }
</script>

<style>
   
    
    
    
    #daste1{
 
    float: right;
    margin-right: -25%;
 background-color: gainsboro;;  
       
     
     
    }
    #img_left11:focus{
      border: 1px solid;
        border-color: gainsboro;
        outline-style: none;
        
    }
    
    #name_of_group{
        margin-right: 15%;
    }
    
   #img_left11{
       position: relative;
     border: 1px solid;
        border-color: gainsboro;
       background-color: gainsboro;
       margin-right: 0%;
       margin-top: 5%;
        width:5%;;
        height:15px;;
        
    } 
    
    #left_l11{
    position: relative;
    margin-top: -20%;
        font-size: 20px;
        z-index: 1;
color: black}
    
    #down_d11{
    position: relative;
      margin-top: -50%;
        margin-left: 40%;
        margin-right: -90%;
        font-size: 20px;
       
        color: black;
        z-index: 1;
    }
    #down_d11:focus{
  
        border-color: gainsboro;
        
    } 
      
   
    
    
    
    
    
</style>