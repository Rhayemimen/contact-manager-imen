<template>
 <ul v-for="person in tab" v-bind:key="person.id">
     <li fa-icon icon="user">{{person.id}}</li>
     <li>{{person.name}}</li>
     <li>{{person.email}}</li>
     <li>{{person.phone}}</li>
     <li>{{person.adresse.street}} {{person.adresse.city}}</li>
 </ul>
 
</template>

<script>
export default {
    name:'ContactsList',
    props: {
        tab: Array
    }
}
</script>

<style>

</style>