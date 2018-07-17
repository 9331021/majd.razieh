<template>
  
<section>
   
    <div id="sub_pass"><b>{{sub}}</b></div>
    
    <input type="password" id="info_pass" :placeholder="pla" v-model="passinput"   @blur="check_input1"/>
    

    
    </section>

</template>

<script>
    export default {
          props:['sub' , 'pla'],
        data () {
            return {
             passinput:''   
            }
        },
        components: {
        },
        
         methods: {
    check_input1(event) {
        
      this.$emit('blur', this.passinput)
    }
  }
        
        
    }
</script>

<style>
  
    #sub_pass{
         border: 1px solid;
       position: relative;
      width: 55%;
        margin-left: 40%;
        height: 30px;
        direction: rtl;
        font-size:12px;
        padding-top: 1.2%;
            color: blue;
        direction: rtl;
        text-align: right;
    }
    
    #info_pass
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