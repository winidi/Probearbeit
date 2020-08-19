<template>
    <div class="content">
        <div class="menu">
<<<<<<< HEAD
            <br>
            <h1>Speisekarte</h1>
=======
>>>>>>> d07ca5799b0487bb587e398aeb70febd455610c0
            <div class="speisediv" v-for="(speise, index) in speisekarte" :key="index">
               <table>
                   <tr>
                        <th> {{ speise.gerichtname }} <br> {{speise.beschreibung}} </th>                        
                   </tr>
<<<<<<< HEAD
                    </table>
                      <button v-on:click="addMeal(index)">bestellen</button>
                    <hr>
                    </div>
                <div class="bestellung">
                <h1>Ihre Bestellung:</h1>
                <div v-for="order in orderList" :key="order.id">
            <h1>{{order.gericht}}</h1>
            </div>
        </div>
       
      
       </div>

=======
               </table>
               <button v-on:click="addMeal(index)">bestellen</button>
               <hr>
            </div>
        
        </div>
>>>>>>> d07ca5799b0487bb587e398aeb70febd455610c0
    </div>
</template>

<script>
export default {
    data(){
        return{
            id: '',
<<<<<<< HEAD
            count1: 0,
            count2: 0,
            count3: 0,
=======
>>>>>>> d07ca5799b0487bb587e398aeb70febd455610c0
            gerichtname: '',
            beschreibung: '',
            speisekarte: [
                {id: 1, gerichtname: 'Pilzsuppe' ,beschreibung: 'mit frischen Pilzen der Saison' },
                {id: 2, gerichtname: 'TomatenSuppe' ,beschreibung: 'mit frischen Tomaten ' },
                {id: 3, gerichtname: 'Kräutersuppe' ,beschreibung: 'mit frischen Pilzen' },
                {id: 4, gerichtname: 'Pilzsuppe' ,beschreibung: 'mit frischen Pilzen der Saison' },
                {id: 5, gerichtname: 'TomatenSuppe' ,beschreibung: 'mit frischen Tomaten ' },
                {id: 6, gerichtname: 'Kräutersuppe' ,beschreibung: 'mit frischen Pilzen' },
                {id: 7, gerichtname: 'Pilzsuppe' ,beschreibung: 'mit frischen Pilzen der Saison' },
                {id: 8, gerichtname: 'TomatenSuppe' ,beschreibung: 'mit frischen Tomaten ' },
            ],
<<<<<<< HEAD
            orderList: [ ]
=======
            orderList: []

>>>>>>> d07ca5799b0487bb587e398aeb70febd455610c0
        }
    },
    methods: {
        addMeal: function(index){
<<<<<<< HEAD
            //alert(index)
            //alert(this.speisekarte[index].gerichtname + ' zur Bestellung hinzugefügt')
            //alert(this.speisekarte.beschreibung)
            this.orderList.push({id: this.speisekarte[index].id , gericht: this.speisekarte[index].gerichtname})
            this.addBestellung(index)
            alert(this.speisekarte[index].gerichtname + ' zur Bestellung zugefügt')
          },

        addBestellung: function(array) {
            
         
=======
            alert(index)
            //alert(this.speisekarte.beschreibung)
            this.beschreibung = this.speisekarte[index].toString();
            this.orderList.push(this.speisekarte.id)

>>>>>>> d07ca5799b0487bb587e398aeb70febd455610c0
        }
    }
}
</script>

<style scoped>

<<<<<<< HEAD
.h1{
    font-family: 'Quicksand', 'Source Sans Pro', 'Segoe UI', 'Helvetica Neue', Arial, sans-serif;
   
}

.bestellung{
    background-color: tomato;
    width: 100%;
    height: 500px;
=======
th{
    
>>>>>>> d07ca5799b0487bb587e398aeb70febd455610c0
}

.speisediv{
    background-color: white;
    width: 50%;
    margin: 0 auto;
}
<<<<<<< HEAD
=======

>>>>>>> d07ca5799b0487bb587e398aeb70febd455610c0
.thclass {
    padding-left: 5em;
    padding-right: 5em;
    padding-top: 3em;
    
}
<<<<<<< HEAD
=======

>>>>>>> d07ca5799b0487bb587e398aeb70febd455610c0
.menu {
    color: black;
    background-color: tomato;
}
<<<<<<< HEAD
=======

>>>>>>> d07ca5799b0487bb587e398aeb70febd455610c0
.tableclass {
   margin-left:auto;
   margin-right:auto;
   padding: 8em;
}
<<<<<<< HEAD
=======


>>>>>>> d07ca5799b0487bb587e398aeb70febd455610c0
</style>