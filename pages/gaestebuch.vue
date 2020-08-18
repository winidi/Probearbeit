<template>
    <div class="content">
        <div class="cincont">
            <div class="guestbookbox">
        <br>
        <h1>Tragen Sie sich ein</h1>
        <label>Name:</label><br>
        <input class="center-block" type="text" v-model="fname"><br> 
        <label>Ihre Nachricht:</label><br>
        <textarea class="center-block" type="text" id="msg" v-model="guesttext"></textarea><br> 
        <button @click="addGuestPost" class="gaestebuchbtn">Abschicken</button>

            </div>

            <div class="eintraege">
                
                <ul v-for="gast in gastbuch" :key="gast.id">
                    <hr>
                <p class="pgast">{{gast.name}}</p>
                {{gast.text}}
                
                </ul>
                              
                
    	    </div>

            
        </div>
    </div>

</template>


<script>
export default {
    data(){
        return {          
            
            fname: ' ',
            guesttext: '',
            id: 0,

            gastbuch: [
              {id: 1, name: 'Leo', text: 'Der erste Eintrag'},
           
            ]
        }
    },
    methods: {
        addGuestPost: function () {
            this.id++;
            this.gastbuch.id = this.gastbuch.id + 1
            this.gastbuch.push ({id: this.id, name: this.fname, text: this.guesttext});
            
            
            
        }

       
    
    }
    
}
</script>

<style scoped>

.eintraege {
    border: solid black;
}

.center-block {

  margin: auto;
  
}

.cincont{

 width: 50%;
 margin: 0 auto;
}

.guestbookbox {
    padding-left: 1em;
    width: 33em;
    margin: auto;
    border: 2px solid #ccc;
}



#msg{
  width: 33em;
  height: 16em;
}

</style>

