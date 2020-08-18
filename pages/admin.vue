<template>
     <div class="content">
         <br>
         <h1>Admin Bereich</h1>

          <div class="eintraege">
                <ul v-for="gast in gastbuch" :key="gast.id">
                    <hr>
                <p class="pgast">{{gast.name}}</p>
                {{gast.text}}

                <button class="adminbutton" @click="deleteGasteintrag">Eintrag löschen</button>
                </ul>
                              
                
    	</div> 

       
        

     </div>
</template>


<script>
export default {
    data(){
        return{
            test: '',
            name: '',
            gastbuch: []
        }
    },
   mounted() {
        this.gastbuch = JSON.parse(localStorage.getItem('STORAGE_KEY'))
    },
    watch: {
        name(newName) {
            localStorage.name = newName;
        }
    },
    methods: {
        
    }
}
</script>


<style >
.adminbutton {
    
    margin-left: 2em;
}

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