<template>
  
<section>

    <div id="sub_info"><b>{{sub}}</b></div>
    
    <input type="text" id="info_info" :placeholder="pla"/>

    
    </section>

</template>

<script>
    export default {
          props:['sub' , 'pla'],
        data () {
            return {
            }
        },
        components: {
        }
    }
</script>

<style>
  
    #sub_info{
         border: 1px solid;
       position: relative;
      width: 55%;
        text-align: right;
        margin-left: 40%;
        height: 30px;
        direction: rtl;
        font-size:12px;
        padding-top: 1.2%;
            color: blue;
    }
    
    #info_info
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