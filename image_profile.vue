<template>
  

<section>
    <figure >
        
      
       <div id="name_profile">نام کاربر</div>        
        
        
          <div id="c_profile">
    
     <div v-if="!image">
  
    <input type="file" @change="onFileChange">
  </div>
  <div v-else>
    <img id="imgg" :src="image" />
   
  </div>
 

    
    </div>
        
        <figcaption id="male_profile">جنسیت</figcaption>
       
        <figcaption id="input_male">
    
            <input  type="button" id="women" value="زن"/>
            <div id="div_women">
            <i id="women_fa" class="fa fa-external-link fa-rotate-90"></i>
    </div>
            
            <input  type="button" id="men" value="مرد"/>
             <div id="div_men">
            <i id="men_fa" class="fa fa-external-link"></i>
    </div>
    
        </figcaption>
      
        </figure>
    
    
    </section>


</template>

<script>
    
    
    export default {
        
        data: {
        
   image:false,
 },
  methods: {
    onFileChange(e) {
      var files = e.target.files || e.dataTransfer.files;
      if (!files.length)
        return;
      this.createImage(files[0]);
    },
    createImage(file) {
      var image = new Image();
      var reader = new FileReader();
      var vm = this;

      reader.onload = (e) => {
        vm.image = e.target.result;
      };
      reader.readAsDataURL(file);
    },
   
        
        
  }
      
    }
</script>

<style>
    
  
    #imgg {
  width: 50%;
 
  display: block;
    border: 1px solid;
       width: 100%;
    margin-top: 0%;
        margin-left:1%;
        border-radius: 80px;
        height: 160px;
        z-index: 1;
}
    
    
    figure{
       border: 1px solid;
        width: 100%;
        height: 270px;
         
        
    }
   
    #name_profile{
        border: 1px solid;
        text-align: center;
        height: 30px;
        
    }
    #c_profile{
      border: 1px solid;
       width: 50%;
    margin-top: 2%;
        margin-left:25%;
        border-radius: 90px;
        height: 160px;  
        border-color: ghostwhite;
    }
    
   #male_profile{
       text-align: center;
         margin-left: 1%;
        margin-top: 2%;
    }
   
    #men{
    position: absolute;
        margin-top: 5%;
       border-bottom-right-radius: 15px;
        border-top-right-radius: 15px;
        width: 20%;
        height: 30px;
        margin-left: 49%;
         border-bottom-right-radius: 15px;
        border-top-right-radius: 15px;
        text-align: right;
          background-color: white;
    }
    
    #women{
        position: absolute;
         margin-top: 5%;
        margin-left: 31%;
        width: 21%;
         border-bottom-left-radius: 15px;
        border-top-left-radius: 15px;
        height: 30px;
        text-align: left;
        background-color: white;
    }
    
   
    
    
    #div_women{
        position: absolute;
        width: 8%;
        height: 25px;;
        margin-left: 41%;
margin-top: 5.5%;
        border: 1px solid;
        background-color: red;
        text-align: center;
        padding-left: 4%;
        padding-bottom: 5%;
    }
    
     #div_men{
        padding-right: 4%;
        position: absolute;
        width: 9%;
         margin-left: 50%;
margin-top: 5.5%;
         background-color: blue;
        height: 25px;;
        border: 1px solid;
         border-color: red;
         text-align: center;
    }
    
    
    #women_fa{
        
        width: 5%;
        height: 10px;
        z-index: 1;
        background-color: red;
        font-size: 20px;
        color: white;
        
    }
   #men_fa{
         width: 5%;
        height: 10px;
        z-index: 1;;
       color: white;
        background-color: red;
        font-size: 18px;
    }
   
    
    
</style>