<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <ContactList v-bind:tab="contactsList"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import ContactList from '@/components/ContactList.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld,
    ContactList
  },
  data(){
    return {
      contactsList: [
        {
          id: 1,
          name: "Imen",
          email: "imen@imen.com",
          phone: "11223344",
          adresse: 
          {
            street: "12345",
            city: "Tunis"
          }
        },
        {
          id: 2,
          name: "Ali",
          email: "ali@ali.com",
          phone: "11111111",
          adresse: 
          {
            street: "52365",
            city: "France"
          }
        },
        {
          id: 3,
          name: "Sarra",
          email: "sarra@sarra.com",
          phone: "222222222",
          adresse: 
          {
            street: "nllef",
            city: "Italy"
          }
        }
      ]
    }
  }
}
</script>
