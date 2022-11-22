<template>
  <v-container>
    <v-list-item-group class="d-flex justify-space-between">
      <div class="v__item" v-for="teg in tegs" :key="teg.id" >
        <v-list-item-icon>
         <v-icon class="justify-start">{{ teg.icon }}</v-icon>   
        </v-list-item-icon>
        <v-list-item-content>
            <v-list-item-title >{{teg.text}}</v-list-item-title>
          </v-list-item-content>
        </div>
    </v-list-item-group>
  </v-container>
</template>

<script>
export default {
  name: "ListTegs",

  data: () => ({
    tegs: [
      {
        id: "0",
        icon: "mdi-star-outline",
        text: "5",
      },
      {
        id: "1",
        icon: "",
        text: "Обзорная",
      },
      {
        id: "2",
        icon: "mdi-bus",
        text: "На автобусе",
      },
      {
        id: "3",
        icon: "",
        text: "25 марта",
      },
      {
        id: "4",
        icon: "mdi-alarm",
        text: "6 часов",
      },
    ],
  }),
};
</script>

<style scoped>
.v__item{
    display: flex;
    flex-direction: row;
}
</style> 
