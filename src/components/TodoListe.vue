<template>
<input type="text" size="50" v-model ="zielEingabe">
<button @click="neuZiel">Neu</button>
<h2>{{ msg }}</h2>
<p v-for="ziel in zielListe" :key="ziel.key">
<input type="radio" name="zielSelect" v-bind:value="ziel.id" v-model=zielSelect> 
</p>
<button @click="deleteZiel">Delete</button>
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
        {id:1, inhalt: 'CSS Animationen lernen'}
        {id:2, inhalt: 'Vue lernen'}
    ],
    let neuId = this.zielListe[thiszielListe.length-1].id+1
}
</script>
