<template>
    <div id="colm_aside3">
        <h3 id="titlle3">{{titi}}</h3>
        
            
  <button id="img_sum3" type="button"  v-on:click="seen=!seen">
                     <i v-if="seen" id="top_p3" class="fa fa-plus"> </i>
    
                     <i v-else-if="!seen" id="top_m3" class="fa fa-minus"></i>
                         
    
    </button>      
        
     
        
        
        
        
        
        
        <div v-if="!seen" id="asid_daste3">
                  
            <table id="table_color">
    <tr>
        <td><input type="text" id="color11"></td>
         <td> <input type="text" id="color12"></td>
         <td> <input type="text" id="color13"></td>
         <td> <input type="text" id="color14"></td>
        <td> <input type="text" id="color15"></td>
    </tr>
                
                <tr>
        <td> <input type="text" id="color21"></td>
         <td> <input type="text" id="color22"></td>
         <td> <input type="text" id="color23"></td>
         <td> <input type="text" id="color24"></td>
                     <td> <input type="text" id="color25"></td>
    </tr>
                <tr>
        <td> <input type="text" id="color31"></td>
         <td> <input type="text" id="color32"></td>
         <td> <input type="text" id="color33"></td>
         <td> <input type="text" id="color34"></td>
                     <td> <input type="text" id="color35"></td>
    </tr>
                <tr>
        <td> <input type="text" id="color41"></td>
         <td> <input type="text" id="color42"></td>
         <td> <input type="text" id="color43"></td>
         <td> <input type="text" id="color44"></td>
                     <td> <input type="text" id="color45"></td>
    </tr>
                
                       <tr>
        <td> <input type="text" id="color51"></td>
         <td> <input type="text" id="color52"></td>
         <td> <input type="text" id="color53"></td>
         <td> <input type="text" id="color54"></td>
                            <td> <input type="text" id="color55"></td>
    </tr>
                       <tr>
        <td> <input type="text" id="color61"></td>
         <td> <input type="text" id="color62"></td>
         <td> <input type="text" id="color63"></td>
         <td> <input type="text" id="color64"></td>
                            <td> <input type="text" id="color65"></td>
    </tr>
                
                
                
    
    
    </table>
          
            
           
            
            
        
    </div>
       <div id="cx3"></div>  
        
    </div>
</template>

<script>
    export default {
    props:['titi'],
        methods:{
           
    },
        data() {
            return{
  seen: true
}
        }
        
        }
        
        
</script>

<style>
    #colm_aside3{

        height: 50px;
        width: 100%;
        margin-top: 5%;
        padding-left: 2%;
        border-radius: 5%;
        background-color:gainsboro;
            background-color: gainsboro;
    }
    
    
   #titlle3{
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
   
    
    #asid_daste3{
     direction: rtl;
        width: 100%;
        margin-top: 2%;
        height: 300px;
        border-radius: 5%;
        padding-left:5%;
        background-color:gainsboro;
        
    }

    #color11{
       margin-right: 10%;
        margin-top: 5%;
        height: 30px;
        width: 70%;
        border: 1px solid;
        
         background-color: ghostwhite;
    }
    #color12{
        margin-right: 10%;
        height: 30px;
        width: 70%;
        border: 1px solid;
         background-color: gainsboro;
        
        
    }
    #color13{
        margin-right: 10%;
       height: 30px;
        width: 70%;
        border: 1px solid;
        background-color: darkgray;
    }
    #color14{
        margin-right: 10%;
       height: 30px;
        width: 70%;
        border: 1px solid;   
        background-color:gray;
        
  
       
    }
    #color15{
        margin-right: 10%;
       height: 30px;
        width: 70%;
        border: 1px solid;
              
        background-color: black;
       
    }
    
    
    
    
    
    #color21{
       margin-right: 10%;
        margin-top: 5%;
        height: 30px;
        width: 70%;
        border: 1px solid;
       background-color:white;
    
    }
    #color22{
        margin-right: 10%;
        height: 30px;
        width: 70%;
        border: 1px solid;
        background-color:burlywood;
        
    }
    #color23{
        margin-right: 10%;
       height: 30px;
        width: 70%;
        border: 1px solid;
        background-color:blanchedalmond;
    }
    #color24{
        margin-right: 10%;
       height: 30px;
        width: 70%;
        background-color:green;
        border: 1px solid;
    }
    #color25{
        margin-right: 10%;
       height: 30px;
        width: 70%;
        border: 1px solid;
        background-color:brown;
    }
    
   #color31{
       margin-right: 10%;
        margin-top: 5%;
        height: 30px;
        width: 70%;
        border: 1px solid;
       background-color:red;
    }
    #color32{
        background-color:deeppink;
        margin-right: 10%;
        height: 30px;
        width: 70%;
        border: 1px solid;
    }
    #color33{
        margin-right: 10%;
       height: 30px;
        background-color:darkmagenta;
        width: 70%;
        border: 1px solid;
    }
    #color34{
        margin-right: 10%;
       height: 30px;
        width: 70%;
        border: 1px solid;
        background-color:aqua;
    }
    #color35{
        margin-right: 10%;
       height: 30px;
        width: 70%;
        border: 1px solid;
        background-color:blue;
    }
    
    
    
    #color41{
       margin-right: 10%;
        margin-top: 5%;
        height: 30px;
        width: 70%;
        border: 1px solid;
        background-color:darkblue;
    }
    #color42{
        margin-right: 10%;
        height: 30px;
        width: 70%;
        border: 1px solid;
        background-color:yellow;
        
    }
    #color43{
        margin-right: 10%;
       height: 30px;
        width: 70%;
        border: 1px solid;
        background-color:pink;
    }
    #color44{
        margin-right: 10%;
       height: 30px;
        width: 70%;
        border: 1px solid;
        background-color:firebrick;
    }
    #color45{
        margin-right: 10%;
       height: 30px;
        width: 70%;
        border: 1px solid;
        background-color:orange;
    }
    
    
    
    #color51{
       margin-right: 10%;
        margin-top: 5%;
        height: 30px;
        width: 70%;
        border: 1px solid;
        background-color:darkolivegreen;
    }
    #color52{
        margin-right: 10%;
        height: 30px;
        width: 70%;
        border: 1px solid;
        background-color:cadetblue;
    }
    #color53{
        margin-right: 10%;
       height: 30px;
        width: 70%;
        border: 1px solid;
        background-color:darkkhaki;
    }
    #color54{
        margin-right: 10%;
       height: 30px;
        width: 70%;
        background-color:darkgoldenrod;
        border: 1px solid;
    }
    #color55{
        margin-right: 10%;
       height: 30px;
        background-color:palevioletred;
        width: 70%;
        border: 1px solid;
    }
    
    #color61{
       margin-right: 10%;
        margin-top: 5%;
        height: 30px;
        width: 70%;
        border: 1px solid;
        background-color:gainsboro;
    }
    #color62{
        margin-right: 10%;
        height: 30px;
        width: 70%;
        background-color:gainsboro;
        border: 1px solid;
        border-color: gainsboro;
    }
    #color63{
        margin-right: 10%;
       height: 30px;
        width: 70%;
         border: 1px solid;
   border-color: gainsboro;
        
        background-color:gainsboro;
    }
    #color64{
        margin-right: 10%;
         border: 1px solid;
       height: 30px;
        width: 70%;
    border-color: gainsboro;
        background-color:gainsboro;
    }
    #color65{
        margin-right: 10%;
       height: 30px;
         border: 1px solid;
        width: 70%;
     border-color: gainsboro;
        background-color:gainsboro;
    }
    
        #cx3{
        
        width: 20%;
    
        height: 5px;
        
    }
    
    
    .fa-plus{
    font-size: 10px;

        
    } 
    
    #pl2{
        z-index: 1;
         position: relative;
        margin-left: 10%; 
         margin-top: -14%;
    }
    
    #mi2{position: relative;
        margin-right: -15%;
    }
    
    
     .fa-minus{
        
       position: relative;
        margin-right: -10%;
        z-index: 1;
       margin-top: -15%;
        font-size: 10px;
       
        
    }
    
     #img_sum3{
         position: absolute;
        height: 20px;
        width: 10%; 
        z-index: 1;
    margin-top: -13%;
        margin-left: 7%;
          border: 1px solid;
        background-color: gainsboro;
        border-color: gainsboro;
        
       padding-right: 5%;
       
    }
    
      #top_p3{
     margin-left: -5%;
        margin-top: -28%;
    }
    
    
    #top_m3{
     margin-left: -5%;
        margin-top: -35%;
         outline: none;
    }
    
     #top_m3:focus{
     outline: none;
        
    }
    
      #img_sum3:focus{
        border: 1px solid;
        border-color: gainsboro;
        outline-style: none;
    }
    
</style>