<template>
    <div id="colm_aside2">
      <h3 id="titlle2">{{titi}}</h3>
        
        
            
  <button id="img_sum2" type="button"  v-on:click="seen=!seen">
                     <i v-if="seen" id="top_p2" class="fa fa-plus"> </i>
    
                     <i v-else-if="!seen" id="top_m2" class="fa fa-minus"></i>
                         
    
    </button>      
 
        
        <div v-if="!seen" id="asid_daste2">
               
            <input type="text" id="search_brand" placeholder="جست و جو"/>           
          
            
            <p id="check_brand">
 <input type="checkbox" class="brands" value="نام برند" /> &nbspنام برند&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp brand<br />
            <div class="line_brand"></div>
	 <input type="checkbox" class="brands" value="نام برند" /> &nbspنام برند &nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp  brand<br />
             <div class="line_brand"></div>
	 <input type="checkbox" class="brands" value="نام برند" />&nbsp نام برند &nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp barnd<br />
             <div class="line_brand"></div>
	  <input type="checkbox" class="brands" value="نام برند" /> &nbspنام برند &nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp&nbsp brand
             <div class="line_brand"></div>
</p>
            
            
        
    </div>
       <div id="cx2"></div>  
        
    </div>
</template>

<script>
    export default {
    props:['titi'],
        methods:{
           
    },
        data() {
            return{
  seen: true,
                im2:'~assets/sum.png'
};
        }
        
        }
        
        
</script>

<style>
    #colm_aside2{

        height: 50px;
        width: 100%;
        margin-top: 5%;
        border-radius: 5%;
        background-color:gainsboro;
            background-color: gainsboro;
    }
    
    
   #titlle2{
margin-left: 50%;
       direction: rtl;
        margin-top: -10%;
        background-color: gainsboro;
        z-index: 1;
text-align: right;
       font-size: 17px;
       width: 45%;
       height: 42px;
   
    }
  
    
    #asid_daste2{
       position: relative;
     direction: rtl;
        width: 100%;
        margin-top: 2%;
        height: 300px;
        border-radius: 5%;
        background-color:gainsboro;
         overflow-y: scroll;    
        padding-left: 2%;
    }

    #search_brand{
        border: 1px solid;
        background-color: white;
        width: 90%;
        height: 50px;
        padding-right: 4%;
        font-size: 20px;
        margin-top: 5%;
    margin-right: 0%;
        margin-left: 5%;
        padding-bottom: 1.8%;
    border-radius: 12px;}
            
    
    #check_brand{
        direction: rtl;
    }
    
    .brands {
        margin-top: 8%;
        font-size: 15px;
         transform: scale(2) !important;
     padding-left: 2%;
        margin-left: 2%;
        
        
    }
    .line_brand{
        width: 90%;
        margin-left: 4%;
        margin-right: 4%;
        margin-top: 4%;
        border: 1px solid;
        border-color: aliceblue;
    }
     #cx2{
        
        width: 20%;
    
        height: 5px;
        
    }
    
    
    .fa-plus{
        
    
    
    
      
        font-size: 10px;

        
    } 
    
    #pl{
        z-index: 1;
         position: relative;
        margin-left: 10%; 
         margin-top: -14%;
    }
    
    #mi{position: relative;
        margin-right: 80%;
    }
    #img_sum2:focus{
        border: 1px solid;
        border-color: gainsboro;
        outline-style: none;
    }
    #top_m2:focus{
        border: 1px solid;
        border-color: gainsboro;
        outline-style: none;
       
    }
     .fa-minus{
        
       position: relative;
        margin-right: -10%;
        z-index: 1;
       margin-top: -15%;
        font-size: 10px;
       
        
    }  
    
      #img_sum2{
          position: absolute;
        height: 20px;
        width: 10%; 
        z-index: 1;
    margin-top: -13%;
        margin-left: 7%;
          border: 1px solid;
          border-color: gainsboro;
          background-color: gainsboro;
         
          padding-right: 5%;
       
    }
    
    
     #top_p2{
     margin-left: -3%;
        
        margin-top: -25%;
    }
    
    
    #top_m2{
     margin-left: -3%;
        margin-top: -25%;
    }
     
    
</style>