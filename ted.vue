<template>
    <section>
        <h1>sldfhiowhf</h1>
    
        <input type="button" @click="next">
    </section>
</template>

<script>
    
    export default {
        
        data: {
 images: ['~/assets/1.jpg','~/assets/2.jpg','~/assets/3.jpg','~/assets/4.jpg'],
 currentNumber: 0,

 },

 mounted: function () {
 this.startRotation();
 },

 methods: {
 

 

 next: function() {
 this.currentNumber += 1
 }
 }
}
        
        
        
</script>

<style>
    
</style>