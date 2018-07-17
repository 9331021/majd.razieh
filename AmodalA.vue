<template>
  <transition name="modal-fade">
    <div id="modal-backdrop">
      <div id="modal">
       
            <header>
          <slot name="header">
           <button
                   type="button" id="bun-close" @click="close" aria-label="Close modal"><i class="fa fa-close"></i></button><p id="in">{{sub_tii}} </p>
         </slot>
        </header>
    
          
          <section  class="modal-body" id="modalDescription">
          <slot name="body">
          
               <info1  id="tel" sub="شماره تلفن یا ایمیل" pla="برای مثال majd.razieh" ></info1>
              
              
        <info_pass1  id="pass" sub="رمزعبور " pla="" ></info_pass1>
              
              
             <p id="forget_pass">رمز عبور خود را فراموش کرده اید؟</p>
             <a id="forget_click" href="#">کلیک کنید</a>
              <button type="button" id="bun-enter" @click="closes"><a  id="pass_right"href="home_page.vue"> {{but_tii}}</a></button>

           
          </slot>
        </section>
       
         
          
         
        
      </div>
    </div>
  </transition>
</template>



<script>
    import info_pass1 from '~/components/info_pass'
          import info1 from '~/components/info'
   
    export default {
        props:['sub_tii','but_tii'],
         name: 'modal',
    methods: {
      close() {
        this.$emit('close');
      },
        
        closes() {
            this.$emit('close');
   
      },
    },
      
        data () {
            return {
              
            }
        },
        components: {
            info1,
       info_pass1
        }
    }
</script>










<style>
#forget_click{
float:right;
 color: rgb(59,85,230);
  text-decoration: none;
font-weight:800;
font-size:12px;
margin-top:12px;
margin-right:3px;
}


#forget_pass{
float:right;
margin-right:20px;
font-size:12px;
margin-top:10px;
}

#password{
float:right;
  margin-top:12px;
  width:233px;
  height:30px;
  border-radius:15px;
  border:1px rgb(240,240,247);
  padding-left:15px;
  margin-right:28px;
  background-color:rgb(240,240,247);
}

#pass{
 float:right;
  color: rgb(59,85,230);
  font-size:14px;
  width: 85%;
  margin-right:20px;
  margin-top:15px;
}

  #modal-backdrop {
    position: fixed;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
      
    background-color: rgba(0, 0, 0, 0.3);
    display: flex;
    justify-content: center;
    align-items: center;
      z-index: 1;
  }

  #tel{
  float:right;
  color: rgb(59,85,230);
  font-size:14px;
  width: 85%;
  margin-right:15px;

  }

  #in{
  float:right;
  color:black;
  font-size:20px;
  foint-weight:300;
 margin-right:130px;
 margin-top:10px;
  }
  #modal {
  float:right;
    background: #FFFFFF;
    width:28%;;
    height:350px;
    box-shadow: 2px 2px 20px 1px;
    overflow-x: auto;
    display: flex;
    flex-direction: column;
  }

  

    #pass_right{
        color: black;
    }
    
    #pass_right:focus{
        color: blue;
    }

  

  .modal-body {
    position: relative;
    padding: 20px 10px;
  }

  #bun-close {
  float:right;
    border: none;
    font-size: 20px;
   
    cursor: pointer;
    font-weight: bold;
    color: black;
    float:right;
  margin-right:7px;
    margin-top:2px;
    background: transparent;
  }

  #bun-enter {
  float:right;
 color:white;
 background-color:rgb(102,102,102);
 margin-top:20px;
 margin-right:130px;
 border-radius:15px;
 font-size:16p;
 width:100px;
 height:35px;

  }
</style>
