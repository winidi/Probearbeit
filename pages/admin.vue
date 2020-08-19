<template>
     <div class="content">
         <br>
         <h1>Admin Bereich</h1>

          <div class="eintraege">
                <ul v-for="(gast, index) in gastbuch" :key="index">
                    <hr>
                <p class="pgast">{{gast.name}}</p>
                {{gast.text}}
                 {{index}}

                <button class="adminbutton" v-on:click="deleteGasteintrag(index)">Eintrag löschen</button>
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
            gastbuch: [],
            
        }
    },
   mounted() {
        this.gastbuch = JSON.parse(localStorage.getItem('STORAGE_KEY'))
    },

    methods: {
        deleteGasteintrag: function(index) {
            alert(index)
            this.gastbuch.splice(index, 1);
            localStorage.setItem('STORAGE_KEY', JSON.stringify(this.gastbuch));
            this.gastbuch = JSON.parse(localStorage.getItem('STORAGE_KEY'))
        }
        
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