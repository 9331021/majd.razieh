<template>
    <section>
        
         <div id="part6">
         <ul id="line_">
                <li id="line_1">
              <button id="detail_but1"   v-on:click="seen=!seen ; seen1=!seen1">مشخصات محصول </button>
       <span v-if="!seen && seen1">
   <detail_of_name1 detail_name="razieh" detail_count="20"></detail_of_name1>
    </span>
    </li>
             <li id="line_2" >
              <button id="detail_but2"   v-on:click="seen1=!seen1; seen=!seen"> نظرات کاربران</button>
                 <span v-if="!seen1 && seen">
      <textarea id="comment" ></textarea>
    </span>
    </li>
    </ul>
        
    </div>
    </section>
</template>

<script>
     import detail_of_name1 from '~/components/detail_of_name'
    export default {
       
        data () {
            return {
                seen:false,
                 seen1:true,
                
                
            }
        },
        components: {
            detail_of_name1
        }
    }
</script>

<style>
   #detail_but1{
       position: relative;
    width: 65%;
       height: 40px;;
       margin-right: -50%;
       margin-top: -50%;
font-size: 16px;
       background-color: gainsboro;
       border: 1px solid;
       border-color: gainsboro;
    }
    
    #detail_but2{
        position: relative;
    width: 60%;
       height: 40px;;
       margin-right: 0%;
       margin-top: -50%;
        margin-left: 50%;
font-size: 16px;
       background-color: gainsboro;
       border: 1px solid;
       border-color: gainsboro;
    }
    
    
    #detail_but2{
     outline-style: none;   
    }
    
    
     #detail_but1{
     outline-style: none;   
    }
    
    
    
    
    
    #part6{
        position: relative;
       width: 100%;
        height:250px;
      
         margin-top:25%;
        
         
    }
    
    
    
    
    #line_{
        position: relative;
     width: 116%;
        margin-top: -1%;
        height: 45px;
        color: black;
       
       float: left;
        margin-left: -16%;
        text-align: center;
        background-color: gainsboro;
        padding-right: 35%;
    }
    
    
    #line_1{
       position: relative;
        width: 30%;
margin-top: 1%;  
        
    }
    
    #line_2{
       position: relative;
         width: 30%;
        margin-top: 1%;
        margin-left: 10%;
        
        
    }
    
  
 
    
    #comment{
        position: relative;
        width: 260%;
        margin-top: 3%;
        height: 200px;
        direction: rtl;
        background-color: ghostwhite;;
        
    }
    
  
    
    
    
    
    
    
</style>