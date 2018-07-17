<template>
    <section>
     <ul id="daste">
  <li id="first">
       <button id="img_left1" type="button"  v-on:click="seen=!seen">
                     <i v-if="seen" id="left_l1" class="fa fa-angle-left"> </i>
    
                     <i v-else-if="!seen" id="down_d1" class="fa fa-angle-down"></i>
                         
    </button>
      
&nbsp{{  name_of_group   }}
      
      
        <div v-if="!seen" id="last_list">
  
            <Aasidegray11 name_of_group="نایک"></Aasidegray11>
            
  </div>
      
      
      
      
    </li>
         
 
         
         
    </ul>  

    </section>

</template>

<script>
     import Aasidegray11 from '~/components/asidegray11'
    export default {
        props:['name_of_group'],
        data () {
            return {
                seen:true
            }
        },
        components: {
            Aasidegray11
        }
    }
</script>

<style>
   
    
    
    
    #daste{
 
    float: right;
    margin-right: -25%;
 background-color: gainsboro;;  
       
     
     
    }
    #img_left1:focus{
      border: 1px solid;
        border-color: gainsboro;
        outline-style: none;
        
    }
    
    #name_of_group{
        margin-right: 20%;
    }
    
   #img_left1{
       position: relative;
     border: 1px solid;
        border-color: gainsboro;
       background-color: gainsboro;
       margin-right: 0%;
       margin-top: 5%;
        width:5%;;
        height:15px;;
        
    } 
    
    #left_l1{
    position: relative;
    margin-top: -20%;
        font-size: 20px;
        z-index: 1;
color: black}
    
    #down_d1{
   position: relative;
      margin-top: -50%;
        margin-left: 40%;
        margin-right: -90%;
        font-size: 20px;
       
        color: black;
        z-index: 1;
    }
    #down_d1:focus{
  
        border-color: gainsboro;
        
    } 
      
   
    
    
    
    
    
</style>