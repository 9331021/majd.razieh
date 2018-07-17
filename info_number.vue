<template>
  
<section>
    
    <div id="sub_number"><b>{{sub}}</b></div>
    
    <input type="text" id="info_number" :placeholder="pla"    v-model="userinput"     @blur="check_input"/>
    
    
    
    </section>

</template>

<script>
    export default {
          props:['sub' , 'pla'],
        data () {
            return {
                 userinput: '',
            }
        },
        methods: {
             check_input: function () {
    
             if (isNaN(this.userinput)) {
        alert( "please wirte just digit");
              
    }
        }
    }
        
        
    }
</script>

<style>
    #form_info{
        border: 1px solid;
        width: 55%;
        height: 72px;
    }
    #sub_number{
         border: 1px solid;
       position: relative;
      width: 50%;
        text-align: right;
        margin-left: 45%;
        height: 30px;
        direction: rtl;
        font-size:12px;
        padding-top: 1.2%;
            color: blue;
    }
    
    #info_number
    {
        border: 1px solid;
        direction: rtl;
      width: 95%;
        margin-left:3%;
        margin-top: 0%;
        padding-right: 1%;
        background-color: gainsboro;
        color: ghostwhite;
        height: 40px;
        border-radius: 15px;;
    
       
    }
    
    
</style>