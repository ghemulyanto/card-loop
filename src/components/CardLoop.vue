<template>
  <v-container fluid grid-list-md>
    <v-layout row wrap>
      <v-flex v-for="item in items" :key="item.id" xs12 md6 lg3>
      <v-card width="90%">
        <v-card-title>{{item.itemName}}</v-card-title>
        <v-card-actions>
          <v-btn block rounded color="orange" class="body-1" @click="say('hello')">Button</v-btn>
        </v-card-actions>
      </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
  export default {
    name: 'card-loop',

    data: () => ({
       items: [
                    { id: 1, itemName: "Card Block 1" },
                    { id: 2, itemName: "Card Block 2" },
                    { id: 3, itemName: "Card Block 3" },
                    { id: 4, itemName: "Card Block 4" },
                    { id: 5, itemName: "Card Block 5" },
                    { id: 6, itemName: "Card Block 6" },
                    { id: 7, itemName: "Card Block 7" },
                    { id: 8, itemName: "Card Block 8" },
                    { id: 9, itemName: "Card Block 9" },
                ]
    }),

    methods:{
       say(message){
          alert(message);
        }
    }
  }
</script>
