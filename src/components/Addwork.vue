<template>
  <v-container>
    <h1>Homework / Assignment</h1>
    <v-select :items="items" v-model="select"></v-select>
    <v-btn @click="addTodo">click</v-btn>
    <v-container>
      <v-list v-for="(item, i) in additem" :key="i">
     
      </v-list>
    </v-container>
  </v-container>
</template>

<script>
export default {
  name: "Addwork.",
  data() {
    return {
      select: "",
      items: ["Web", "SA", "ML", "etc"],
      additem: [],
    };
  },
  methods: {
    addTodo() {
      this.additem.push({ this.select });
    },
  },
};
</script>

<style></style>
