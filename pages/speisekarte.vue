<template>
    <div class="content">
        <div class="menu">
            <div class="speisediv" v-for="(speise, index) in speisekarte" :key="index">
               <table>
                   <tr>
                        <th> {{ speise.gerichtname }} <br> {{speise.beschreibung}} </th>                        
                   </tr>
               </table>
               <button v-on:click="addMeal(index)">bestellen</button>
               <hr>
            </div>
        
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            id: '',
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
            orderList: []

        }
    },
    methods: {
        addMeal: function(index){
            alert(index)
            //alert(this.speisekarte.beschreibung)
            this.beschreibung = this.speisekarte[index].toString();
            this.orderList.push(this.speisekarte.id)

        }
    }
}
</script>

<style scoped>

th{
    
}

.speisediv{
    background-color: white;
    width: 50%;
    margin: 0 auto;
}

.thclass {
    padding-left: 5em;
    padding-right: 5em;
    padding-top: 3em;
    
}

.menu {
    color: black;
    background-color: tomato;
}

.tableclass {
   margin-left:auto;
   margin-right:auto;
   padding: 8em;
}


</style>