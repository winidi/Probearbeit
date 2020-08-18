<template>
     <div class="content">
         <br>
         <h1>Admin Bereich</h1>

          <div class="eintraege">
                <ul v-for="gast in gastbuch" :key="gast.id">
                    <hr>
                <p class="pgast">{{gast.name}}</p>
                {{gast.text}}

                </ul>
                              
                
    	    </div>

        

     </div>
</template>


<script>
export default {
    data(){
        return{
            test: ''
        }
    }
}
</script>


<style >
.content{  
    margin: 0;
    width: 100%;
    min-height: 100vh;
    background-image: linear-gradient(
        #f8bcb8,	
        rgb(212, 179, 179),    
        #B5D5D8);
}
</style>