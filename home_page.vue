 <template>
<section>
    
    
      <Eheader_1></Eheader_1>
    <search_nav4></search_nav4>
     
     <div id="line2"> </div>
    <div id="slidshow"> 
     
        <img id="array_img"  :src="images[currentNumber]" />
          
         <button id="back_left" @click="back"><i id="back" class="fa fa-angle-left" v-model="currentNumber" ></i></button>
        <p>Image slider</p>
        
        <button id="next_right" @click="next"> <i id="next"  class="fa fa-angle-right" v-model="currentNumber" ></i></button>
     
        <div id="ci1" v-model="civalue">
    </div>
     <div id="ci2">
    </div>
     <div id="ci3">
    </div>
    <div id="ci4">  
    </div>
    </div>
 
    
      <div id="line3"> </div>
    
    
    <div id="image_table">
            <div id="col1_image"><div id="bla1">image</div></div>
            <div id="col2_image"><div id="bla2">image</div></div>
            <div id="col3_image"><div id="bla3">image</div></div>
    
            <div id="col11_image">پچگانه</div>
            <div id="col22_image">زنانه</div>
            <div id="col33_image">مردانه</div>
    </div>
    
  
    <p id="best"><b>بهترین را از ما خرید کنید</b></p>
   <table id="table4">  
        <tr id="row_3">
            <td id="box_blue">
                <div id="box1">
 <img  id="letter2" src='~assets/Captureletter2.png'>  </div>
            <div id="text4">
                در خبرنامه ما 
                </div>
                <div id="text5">
                عضو شوید !
                </div>
       <div class="ev3">
                <input type="text" class="text66"   placeholder="آدرس ایمیل خود را وارد کنید." >
                 <div class="ev">
                    <i id="env" class="fa fa-envelope" ></i>
                </div>
                </div>
        <button id="text7" type="button">عضو شوید</button>    
            </td>
        <td id="box_white">
                <div id="box2">
                <div id="box22">
تمام برندهای معتبر را با ما تجربه کنید.
                </div>
                    </div>
    </td>
    </tr>
        
        
    </table>
    <div id="part_footer">
    <footer10></footer10>
    </div>
    </section>
</template>  
 


<script>    

         import footer10 from '~/components/footer'
             import Eheader_1 from '~/components/header_1'
          import search_nav4 from '~/components/search_nav'
    export default {
            data() {
                 return {
 images: [require('~/assets/1.jpg'),require('~/assets/2.jpg'),require('~/assets/3.jpg'),require('~/assets/4.jpg')],
currentNumber:0, 
                    cc:'red',
                     civalue:'sssssss'
         
                 }
 },
        components: {
        
            footer10,
            Eheader_1,
            search_nav4
            
        },
        
         methods: {
  next: function() {
 this.currentNumber += 1;
   if( this.currentNumber === 0){
 document.getElementById("ci1").style.background="#778899";
   document.getElementById("ci2").style.background="#FFFFFF";
         document.getElementById("ci3").style.background="#FFFFFF";
         document.getElementById("ci4").style.background="#FFFFFF"
   }
      
            else if( this.currentNumber === 2){
                 document.getElementById("ci3").style.background="#778899";
   document.getElementById("ci1").style.background="#FFFFFF";
         document.getElementById("ci2").style.background="#FFFFFF";
         document.getElementById("ci4").style.background="#FFFFFF"
            }
            else if( this.currentNumber === 3){
                 document.getElementById("ci4").style.background="#778899";
   document.getElementById("ci1").style.background="#FFFFFF";
         document.getElementById("ci3").style.background="#FFFFFF";
         document.getElementById("ci2").style.background="#FFFFFF"
            }
       else if( this.currentNumber === 1){
                 document.getElementById("ci2").style.background="#778899";
   document.getElementById("ci4").style.background="#FFFFFF";
         document.getElementById("ci3").style.background="#FFFFFF";
         document.getElementById("ci1").style.background="#FFFFFF"
            }
      
      
 },
             
             
             back: function() {
 this.currentNumber -= 1;
                  if( this.currentNumber === 1){
   document.getElementById("ci2").style.background="#778899";
   document.getElementById("ci1").style.background="#FFFFFF";
         document.getElementById("ci3").style.background="#FFFFFF";
         document.getElementById("ci4").style.background="#FFFFFF"
   }
      
            else if( this.currentNumber === 2){
                 document.getElementById("ci3").style.background="#778899";
   document.getElementById("ci1").style.background="#FFFFFF";
         document.getElementById("ci2").style.background="#FFFFFF";
         document.getElementById("ci4").style.background="#FFFFFF"
            }
            else if( this.currentNumber === 3){
                 document.getElementById("ci4").style.background="#778899";
   document.getElementById("ci1").style.background="#FFFFFF";
         document.getElementById("ci3").style.background="#FFFFFF";
         document.getElementById("ci2").style.background="#FFFFFF"
            }
       else if( this.currentNumber === 0){
                 document.getElementById("ci1").style.background="#778899";
   document.getElementById("ci4").style.background="#FFFFFF";
         document.getElementById("ci3").style.background="#FFFFFF";
         document.getElementById("ci2").style.background="#FFFFFF"
            }                
                 
                 
                 
                 
                 
                 
                 
 }
             
 }
        
        
        
        
        
    };
</script>







<style>
    
     @import '../assets/font/font-awesome-4.7.0/css/font-awesome.css';
    
    
    
    
    
    
    
  
    
    
     #line2{
        
        width: 100%;
       border: solid 1px;
    border-color: white;
border-bottom-color: black;
        margin-top: 1%;
      
        
    }
    
    #array_img{
   
        width: 90%;
       position: relative;
        margin-top:0%;
        margin-left: 5%;
      border: 1px solod;
        border-color: white;
        height: 200px;
     
    }
    #slidshow{
        margin-left: 4%;
        width: 90%;
       
      
        height: 220px;
        border: 1px solid;
        margin-top: 2%;
    }
    
    
    #back{
        margin-left: 2%;
        margin-top: 5%; 
        font-size: 80px;
         color: gainsboro;
    }
    
    
    #next{
        margin-left: 20%;
        margin-top: -5%;
        font-size: 80px;
        color: gainsboro;
    }
    
    #back_left{
        position: absolute;
        margin-top: 4%;
        margin-left: -85%;
        background-color: white;
          border: 1px solid;
        border-color: white;
    }
    
    
    
    #next_right{
        border: 1px solid;
        border-color: white;
        background-color: white;
        position: absolute;
        margin-left: 86%;
        margin-top: -5%;
       
    }
    
  
    
    
    
    #slidshow p{
    margin-top: -10%;    
        margin-left: 47%;
    }
    
    #ci1{
        position: relative;
        height: 5%;
        width: .8%;
        border-radius:50px;
        border: 1px solid;
        margin-left: 48.8%;
        margin-top: 8.2%;
        background-color: "#778899"
    }
     #ci2{
           position: relative;
        height: 5%;
        width: .8%;
        border-radius:80px;
        border: 1px solid;
        margin-left: 49.8%;
        margin-top: -.9%;
    }
     #ci3{
           position: relative;
        height: 5%;
        width: .8%;
        border-radius:80px;
        border: 1px solid;
        margin-left: 50.8%;
        margin-top: -.9%;
    }
     #ci4{
           position: relative;
        height: 5%;
        width: .8%;
        border-radius:80px;
        border: 1px solid;
        margin-left: 51.8%;
        margin-top: -.9%;
    }
    
    
    
    #line3{
        width: 100%;
       border: solid 1px;
    border-color: white;
border-bottom-color: black;
        margin-top: 1%;
           
    }
    
    
    #image_table{
        margin-left: 4%;
        width: 90%;
        margin-top: 1.2%;
        height:200px;
        
       
    }
  
    #col1_image{
        
        width: 33.3%;
        height: 130px;
        background-image: url('~assets/letter_image.png');
        
    }
     #col2_image{
        height: 130px;
       margin-left: 33.1%;
           width: 33.3%;
         margin-top: -10.7%;
         
 background-image: url('~assets/letter_image.png');
        
    }
     #col3_image{
         margin-left: 66.3%;
           width: 33.3%;
         margin-top: -10.8%;
         height: 130px;
         
        background-image: url('~assets/letter_image.png');
      
    }
   
  
      
     #col11_image{
    
    height: 30%;
        width: 33.3%;
        margin-top: -.3%;
         background-color: gainsboro;
         border: 1px solid;
         border-color: gainsboro;
          border-right-color: black;
         text-align: center;
         padding-top: 1%;
         font-size: 20px;
    }
    
    #col22_image{
    height: 30%;
        width: 33.3%;
        background-color: gainsboro;
    margin-left: 33.3%;
        margin-top: -4.9%;
        border: 1px solid;
         border-color: gainsboro;
          border-right-color: black;
          border-right-color: black;
        text-align: center;
         padding-top: 1%;
         font-size: 20px;
    }
    #col33_image{
    height: 30%;
        margin-left: 66.6%;;
        margin-top: -5%;
        background-color: gainsboro;
        width: 33.3%;
        text-align: center;
         padding-top: 1%;
         font-size: 20px;
      
   
        
    }
    
    
    
    
    
    
    
    
    
    
    
    #bla1{
         border: 1px solid;
        width: 9%;
        margin-left: 11%;
        text-align: center;
      position: absolute;
        height: 6%;
         margin-top: 3.2%;
        background-color: white;
         padding-top: .5%;
    }
     #bla2{
         border: 1px solid;
        width: 9%;
        margin-left: 11%;
        text-align: center;
      position: absolute;
        height: 6%;
         margin-top: 3.2%;
        background-color: white;
         padding-top: .5%;
        
    }
     #bla3{
        border: 1px solid;
        width: 9%;
        margin-left: 11%;
        text-align: center;
      position: absolute;
        height: 6%;
         margin-top: 3.2%;
        background-color: white;
         padding-top: .5%;
    }
    
    
    
    
    #best{
        margin-left: 40%;
    font-size: 25px;
        
    }
        
        
        
        
        
        
    
#table4{
    
   width:80.5%;
      height: 250px; 
    position:relative;
    top: 150px;
     margin-top: -120px;
    margin-left: 230px;
    padding-bottom: 12%;
    
}

    
#box_blue{
    position: relative;
    float: left;
    margin-left: -15%;
border: solid 1px;
    border-color: gainsboro;
    width:29%;
      height: 250px; 
   margin-top: 0px;
    background-color:rgb(59,85,230);
    box-shadow:  10px 10px 10px #999;
    
    
}
#box_white{
    position: relative;
    float: right;
   margin-left: -5%;
    margin-right: 5%;
    border: 1px solid;
    width:78%;
      height: 250px;
    background-image: url(~assets/Capturebrand.png);
    
}
#box2{
    
    width:48%;
      height: 27px;
    text-align: center;
    direction: rtl;
    border: solid 1px;
    border-color: #2773CF;
    border-radius: 14px;
    background-color: rgb(59,85,230);
   
    margin-left: 240px;
    margin-top: 110px;
    padding-bottom: 4%;
}

#box22{
    width:100%;
      height: 27px;
    text-align: center;
    direction: rtl;
   color: white;
    margin-left: 25%;
    z-index: 1;
   
    margin-top: 5px; 
    
    
}



#letter2{
    margin-left: 130px;
    margin-top: 40px;
    
}
#text4{
    margin-left: 0px;
    margin-top: 2px;
    text-align: center;
    color: white;
    font-size: 15px;
}

#text5{
    margin-left: 0px;
    margin-top: 5px;
    text-align: center;
    color: white;
    font-size: 15px;
    
}

.text66{

    direction: rtl;
  width: 202px;
    height: 30px;
   margin-left:15%;
    margin-top:15px;
    top:-150%;
    padding-right: 15%;
    border-radius: 15px;
    font-size: 12px;
}

.ev{
    height: 30px;
    width: 20px;
   margin-left:15%;
    margin-top: -35px;
   border-radius: 15px; 
   
    
}


.ev > .fa-envelope{
  font-size:22px;
    color:rgb(59,85,230);
    margin-left: 200px;
    margin-top: 5px;
}  


.ev3*:hover{
   color: black;
    
}


.ev > .fa-envelope:hover{
    color: black;
    
}  
.text66:hover{
    color: black;
}
.ev3:hover .ev > .fa-envelope{
    color: black;
    
}





#text7{
     width:28%;
      height: 30px;
    border: solid 1px;
    border-color: white;
     margin-left: 111px;
    margin-top: 18px;
     border-radius: 20px;
    background-color: black;
    color: white;font-size: 14px;
  
    
}
#text7:hover{
    background-color: rgb(34,38,64)
    
}    
        
    #part_footer{
        margin-top: 13%;
    } 
        
        
        
    #env{
        color: black;
       position: relative;
        
       
        margin-left: 810%;
        margin-top: 45%;
        z-index: 1;
        font-size: 20px;
    }
        
        
    #env:hover{
        color: blue;
    }   
    
    
</style>