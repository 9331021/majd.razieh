<template>
  
<section>
  
    <div id="sub_date"><b>{{sub}}</b></div>
    
    <input type="date" id="info_date" :placeholder="pla" value="2018-01-11"
               min="1970-01-01" max="2018-02-31"/>
    

    
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
  
    #sub_date{
         border: 1px solid;
       position: relative;
      width: 55%;
        margin-left: 40%;
        height: 30px;
        text-align: right;
        font-size:12px;
        padding-top: 1.2%;
            color: blue;
    }
    
    #info_date
    {
        border: 1px solid;
     
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