    <template>
  <section>
<div id="top" >

<button  id="login"  v-model="sub_ti"  @click="showModalA">عضویت</button>
<button id="join" v-model="but_ti" @click="showModalB">ورود</button>
<modal1 v-if="isModalVisibleA" :but_tii="but_ti"   :sub_tii="sub_ti" @close="closeModalA" />

 

<div class="titr"> Clothser</div>
 
    
<ul>
  <li><a href="#">مردانه  </a> </li>
  <li><a href="#">زنانه </a></li>
  <li><a href="#">بچگانه </a></li>
    
  <li><a href="#">ورزشی</a></li>
  <li><a href="#">تخفیف </a></li>
  <li><a href="#">برندها </a></li> 
</ul>

<div id="line"> </div>
    
   
</div>
 <search_nav5></search_nav5>
    </section>
</template>
<script>
     
     import search_nav5 from '~/components/search_nav';
 import modal1 from '~/components/AmodalA';
   
    export default{
          name: 'app',
       components: {
       search_nav5,
        
            modal1
            
        },
          data () {
      return {
        isModalVisibleA: false,
         
      };
    },
    methods: {
      showModalA(){
        this.isModalVisibleA = true;
           this.sub_ti = "ثبت نام";
          this.but_ti = "ثبت نام";
          
           
      },
        showModalB() {
        this.isModalVisibleA = true;
             this.sub_ti = "ورود ";
             this.but_ti = "ورود ";
            
      },
       
      closeModalA() {
        this.isModalVisibleA = false;
      },
       
    },
              
  };
</script>



<style>







        #top{
	width:90%;
	margin-top:2%;}
    


    #login{
	float:right;
	
	text-align:center;
	height:23px;
	width:7%;
	color:#270000;
	border:solid 1px;
	border-color:black;
    background-color: white;
	margin-right:1%;
	text-decoration:none;
	border-radius:50px;
 
}
 
    
#join{
		float:right;
	direction:rtl;
   
	text-align:center;
	height:23px;
	width:7%;
	color:white;
     background-color:grey;
	border:solid 1px;
	border-color:black;

	margin-right:0.4%;
	text-decoration:none;
	border-radius:50px;
}

    

#join:hover {
    background:blue;
    color: white;
}

#login:hover {
    background: white;
    color: blue;
}
















    
    
    
    .titr{
    
   font-size: 25px;
    text-align: center;
    font-family:sans-serif;
    color: black;
    margin-left:25%;
     text-shadow : 3px 3px 3px gray ; 
}
   
    
 ul {
	list-style-type:none;
	color:white;
	width:70%;
	height:0%;
	background-color:white;
     margin-left:16%;
     margin-top: 3%;
    
}
   ul li {
	float:right;
	position:relative;
	text-align:center;
	width:120px;
       margin-left: 1%;
      
  
} 
   
      ul li a{
        text-decoration: none;
        color: black;
    
    }
    
    
    #line{
        
        width: 90%;
       border: solid 1px;
    border-color: white;
border-bottom-color: black;
        margin-top: 6%;
        margin-left: 9%;
        
    }
    
    </style>