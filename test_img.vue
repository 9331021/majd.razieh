<template>
    <section>
        
        <ted1>
 <img :src="images[currentNumber]" />
</ted1>
        
    </section>
</template>

<script>
     import ted1 from '~/components/ted';
    export default {
        data () {
            return {
               currentNumber:0 
            }
        },
        components: {
           ted1,
        }
    }
</script>

<style>
    
</style>