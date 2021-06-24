<template>
<input type="text" size="50" v-model ="zielEingabe">
<button @click="neuZiel">Neu</button>
<h2>{{ msg }}</h2>
<p v-for="ziel in zielListe" :key="ziel.key">
<input type="radio" name="zielSelect" v-bind:value="ziel.id" v-model=zielSelect> 
<button @click="deleteZiel">Delete</button>
</p>
</template>
<script>
export default {
name: 'ToDo',
props: { 
    msg: String 
    },
data: function() {
return { 
    zielListe: [
        {id:1, inhalte: 'CSS Animationen lernen'}
    ]
}
},
methods: {
neuZiel() { },
deleteZiel () { }
}
}
</script>'},