<template>
  
<section>

<div class="search">
<button type="submit" class="searchButton"> <i class="fa fa-search"></i></button>
<input type="text" class="searchTerm" ></div>
    </section>



</template>

<script>
    export default {
        data () {
            return {
            }
        },
        components: {
        }
    }
</script>

<style>
        
    .search {
  float:left;
  width: 18%;
  margin-left:8%;
  margin-top:-25px;
}
.searchButton {
  position: absolute;  
  right: 90%;
    top:4.5%;
  width: 20px;
  height: 20px;
 margin-top: 1.8%;
  text-align: center;
  color: black;
  cursor:pointer;
  font-size: 12px;
  border:solid 0px;
    
     border-radius:5px;
  border-color:#172593;
    background-color: white;
}

.searchTerm {
  direction:rtl;
  float: right;
  width: 100%;
  height: 22px;
  background-color:white;
  border:thin;
    border: solid 1px;
    border-color: black;
  border-radius:11px;
  color: black;
    margin-top: -40%;
}
    
    .searchTerm:hover{
    color: rgb(59,85,230);;
}
.searchButton:hover{
color: rgb(59,85,230);    
}
    
   
    .searchTerm:hover {
   border-color: rgb(59,85,230);;
}    
    
</style>