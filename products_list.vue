<template>
<section>
    <Bheader_1></Bheader_1>
    <search_nav1></search_nav1>
    
    <div id="head_product1">
        نام دسته
         </div>
        <div id="head_product2">
            <p id="ppp">  مرتب سازی</p>
        <select id="select_order">
  
  <option >تنوع رنگ</option>
  <option >ارازان ترین</option>
  <option selected>محبوب ترین</option>
    </select>  
            <input type="button" value="صفحه قبلی" id="prv_page"><i class="fa fa-angle-right" ></i>
           <input type="text" id="count_page" value="صفحه 1 تا 2" />
            <input type="button" value="صفحه بعدی" id="next_page"><i class="fa fa-angle-left"></i>
           
        
        
    </div>
   
    
    <section id="part1">
        <table id="table_product">
<tr id="tr_product1">
    <td id="td_product1">
         <product id="product1"></product>
    </td>
     <td id="td_product2">
           <product id="product2"></product>
    </td>
     <td id="td_product3">
           <product id="product3"></product>
    </td>
     <td id="td_product4">
           <product id="product4"></product>
    </td>
    </tr>
            <tr id="tr_product2">
    <td id="td_product21">
     <product id="product21"></product>
    
    </td>
     <td id="td_product22">
          <product id="product22"></product>
    </td>
     <td id="td_product23">
          <product id="product23"></product>
    </td>
     <td id="td_product24">
          <product id="product24"></product>
    </td>
    </tr>
            
 
            
            
          
            
            
            
    </table>
        
        
    </section>
    
    
    
    <aside id="part2">
        <aside_gray id="gray1"
    titi="دسته بندی ها "
    >
    
    </aside_gray>
        
      <aside_gray2 id="gray2"
    titi="براساس برند ها "
    >
    
    </aside_gray2> 
        
        
        
        
        <aside_gray3 id="gray3" titi="رنگ">
    
    </aside_gray3> 
        
        
        
        

    </aside> 
    
    
    
    
    <footer2></footer2> 
    
    
    
    
    </section>
</template>

<script>    
    import product from '~/components/product'
           import aside_gray from '~/components/aside_gray'
                import aside_gray2 from '~/components/aside_gray2'
                    import aside_gray3 from '~/components/aside_gray3'
                      import footer2 from '~/components/footer'
        import Bheader_1 from '~/components/header_1'
             import search_nav1 from '~/components/search_nav'
        
    export default {
        components: {
        
            product,
            aside_gray2,
            aside_gray,
            aside_gray3,
            footer2,
            Bheader_1,
            search_nav1
          
            
        }
    };
</script>

<style>
     
  
    
    
    
    
    
    
    #head_product1{
     
        margin-left: 10%;
       padding-top: 2%;
        font-size: 24px;
        width: 65%;
        margin-top: 2%;
       text-align: right;
        height: 40px;
        direction:rtl;
        
    }
     #head_product2{
       
        width: 65%;
         margin-top: 2%;
        margin-left: 10%;
        height: 70px;   
         direction: rtl;
         text-align: right;
    }
   
    ul{
        margin-top: -.5%;
    }
    #select_order{
     position: absolute;
        margin-right:12%;
      height: 28px;
        margin-top: 1%;
        margin-bottom: 0%;
        font-size: 18px;
        width: 12%;
        
    }
    
    #ppp{
        position: absolute;
        font-size: 20px;
        margin-top: 1%;
    }
    
    #prv_page{
        position: absolute;
       
        margin-top: .7%;
        margin-right: 40%;
        border: 1px solid;
        width: 7.5%;
        height: 38px;
      padding-right: 1%;
        font-size: 16px;
        background-color: white;
    }
    .fa-angle-right{
        position: absolute;
        margin-right: 40.5%;
        font-size: 20px;
        margin-top: 1.5%;
    }
    .fa-angle-left{
     position: absolute;
       margin-top: 1.5%;
       margin-left: 19%;
        margin-right: -1%;
        z-index: 1;
        font-size: 20px;
        color: black;
     
    }
    #next_page{
        margin-top: 1%;
        float: right;
        margin-right:86%;
        border: 1px solid;
        width: 11.5%;
        height: 38px;
         padding-left: 1.2%;
        font-size: 16px;
        background-color: white;
    }
    #count_page{
        position: absolute;
        width: 6%;
    margin-top: 1.2%; !important
        z-index: 1;
       margin-right: 49%;
        border: 1px solid;
        border-color: white;
        font-size: 14px;
        color: black;
        direction: rtl;
        height: auto;
    }
   
    #count_page:focus {
 
    border:1px solid;
    border-color:white;;
}
    
    
    
    
    #part1{
      
        margin-left: 1%;
        width: 75%;
        height:950px;
        float: left;
        margin-top: 1%;
           
    }   
    
    
    #part2{
       float: right;
          margin-top: -8.5%;
        margin-right: 1%;
        position: relative;
        width: 20%;
        height: 800px;
        
    }   
    
    
    #table_product{
       
        width: 100%;
        height: 750px;
        
    }
    
    #td_product1{
     
         width: 20%;
        height: 280px;
        
        
    }
     #td_product2{
     
         width: 20%;
        height: 270px;   
        
    }
    
     #td_product3{
     
         width: 20%;
        height: 270px;
        
        
    }
     #td_product4{
    
         width: 20%;
        height: 270px;
        
        
    }
    
    
    
    
     #td_product21{
     
         width: 20%;
        height: 280px;
        
        
    }
     #td_product22{
     
         width: 20%;
        height: 270px;   
        
    }
    
     #td_product23{
     
         width: 20%;
        height: 270px;
        
        
    }
     #td_product24{
    
         width: 20%;
        height: 270px;
        
        
    }
    

    #gray1{
       border-radius: 5%;
background-color: gainsboro; 
        
        
    }
    
    #gray2{
background-color: gainsboro; 
         border-radius: 5%;
        margin-top: 15%;
        
    }
    
     #gray3{
background-color: gainsboro; 
         border-radius: 5%;
        margin-top: 15%;
        
    }
    
    
    
     footer2{
         position: relative;
         z-index: 1;
         margin-bottom: 70%;
        margin-top: -50%;
         margin-top: -100px;
    }     
     
    
    
    
</style>