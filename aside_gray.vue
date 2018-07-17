<template>

    <div id="colm_aside">
        
        
      <h3 id="titlle">{{titi}}</h3>
      
  <button id="img_sum" type="button"  v-on:click="seen=!seen">
                     <i v-if="seen" id="top_p" class="fa fa-plus"> </i>
    
                     <i v-else-if="!seen" id="top_m" class="fa fa-minus"></i>
                         
    
    </button>      
        
        
            
        <div v-if="!seen" id="asid_daste">
  
            <Aasidegray1 name_of_group="ادیداس"></Aasidegray1>
            
  </div>
        <div id="cx"></div>
            
    </div>
   
</template>

<script>
    
     import Aasidegray1 from '~/components/asidegray1'
    export default {
    props:['titi'],
    components:{
          Aasidegray1 
    },
        data() {
            return{
  seen: true,
                im:'sum'
};
     
        }
        
        }
        
        
</script>

<style>
    #colm_aside{
padding-top: 2%;
        height: auto;
        width: 100%;
        background-color:gainsboro;
            background-color: gainsboro;
        border-radius: 5%;
        padding-right: 2%;
        border: 1px solid;
    }
    #cx{
        
        width: 20%;
       
        height: 25px;
        
    }
    
   #titlle{
       position: absolute;
margin-left: 45%;
       direction: rtl;
       text-align: right;
        margin-top: 2%;
        background-color: gainsboro;
        z-index: 1;
       direction: rtl;
      
          
       width: 50%;
       height: 40px;
       font-size: 17px;
   
    }
    #img_sum{
       
        height: 20px;
        width: 10%; 
        z-index: 1;
        border: 1px solid;
        background-color: gainsboro;
        border-color: gainsboro;
    margin-top: 3%;
        margin-left: 6%;
       text-align: center;
        padding-bottom: 2%;
          
    
    
    }

    
    
    #cx{
        
        width: 20%;
       
        height: 25px;
        
    }
    
    
    .fa-plus{
        
     position: absolute;
        margin-left: -6%;
    
       margin-top: 3%;
        font-size: 10px;

        
    }   
     .fa-minus{
        
       position: absolute;
        margin-right: -10%;
        z-index: 1;
       margin-top: -15%;
        font-size: 10px;
       
        
    }  
    
    
    
    #asid_daste{
        margin-top: 8%;
      direction: rtl;
        width: 100%;
        height: 220px;
         border-radius: 5%;
        background-color:gainsboro;
        overflow-y: scroll;
        overflow-x: hidden;
        
        
    }

    #top_p{
     margin-left: -1.2%;
        margin-top: -2%;
    }
    
    
    #top_m{
     margin-left: -1.2%;
        margin-top: -2%;
    }
    
      #img_sum:focus{
        border: 1px solid;
        border-color: gainsboro;
        outline-style: none;
    }
    
    
</style>