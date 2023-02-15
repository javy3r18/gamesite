<template>
  <b-container fluid class="m-0 p-0">
    <div class="vh-100" :class="mainHeight">
      <div class="position-absolute logo">
        <h1>Here is the logo</h1>
      </div>
      <b-row class="w-100 m-0 p-0">
        <b-col :class="columnsHeight" class="columns bg-aqua"></b-col>
      </b-row>
      <b-row class="w-100 m-0 p-0">
        <b-col :class="columnsHeight" class="columns bg-aqua"></b-col>
      </b-row>
      <b-row class="w-100 m-0 p-0">
        <b-col :class="columnsHeight" class="columns bg-aqua"></b-col>
      </b-row>
      <b-row class="w-100 m-0 p-0">
        <b-col :class="columnsHeight" class="columns bg-blue"></b-col>
      </b-row>
      <b-row class="w-100 m-0 p-0">
        <b-col :class="columnsHeight" class="columns bg-blue"></b-col>
      </b-row>
      <b-row class="w-100 m-0 p-0">
        <b-col :class="columnsHeight" class="columns bg-blue"></b-col>
      </b-row>
      <b-row class="w-100 m-0 p-0">
        <b-col :class="columnsHeight" class="columns bg-green"></b-col>
      </b-row>
      <b-row class="w-100 m-0 p-0">
        <b-col :class="columnsHeight" class="columns bg-green"></b-col>
      </b-row>
      <b-row class="w-100 m-0 p-0">
        <b-col :class="columnsHeight" class="columns bg-green"></b-col>
      </b-row>
      <b-row class="w-100 m-0 p-0">
        <b-col :class="columnsHeight" class="columns bg-purple"></b-col>
      </b-row>
      <b-row class="w-100 m-0 p-0">
        <b-col :class="columnsHeight" class="columns bg-purple"></b-col>
      </b-row>
      <b-row class="w-100 m-0 p-0">
        <b-col :class="columnsHeight" class="columns bg-purple"></b-col>
      </b-row>
      <b-row class="w-100 m-0 p-0">
        <b-col :class="columnsHeight" class="columns bg-red"></b-col>
      </b-row>
      <b-row class="w-100 m-0 p-0">
        <b-col :class="columnsHeight" class="columns bg-red"></b-col>
      </b-row>
      <b-row class="w-100 m-0 p-0">
        <b-col :class="columnsHeight" class="columns bg-red"></b-col>
      </b-row>
      <b-row class="w-100 m-0 p-0">
        <b-col :class="columnsHeight" class="columns bg-yellow"></b-col>
      </b-row>
      <b-row class="w-100 m-0 p-0">
        <b-col :class="columnsHeight" class="columns bg-yellow"></b-col>
      </b-row>
      <b-row class="w-100 m-0 p-0">
        <b-col :class="columnsHeight" class="columns bg-yellow"></b-col>
      </b-row>
    </div>
    <main>hola</main>
  </b-container>
</template>

<script>
export default {
  data() {
    return {
      mainHeight: "",
      columnsHeight: "",
    };
  },

  mounted() {
    this.changeMainHeight();
  },

  methods: {
    changeMainHeight() {
      setTimeout(() => {
        this.mainHeight = "mainHeight";
        this.columnsHeight = "columns-resized";
      }, "6000");
    },
  },
};
</script>

<style>
.mainHeight {
  height: calc(100vh - ((100vh / 18) * 2)) !important;
}

.columns {
  background-color: black;
  height: calc(100vh / 18);
  margin: 0;
  padding: 0;
  transition: all ease-in-out 3s;
}

.columns-resized {
  height: calc((100vh - ((100vh / 18) * 2)) / 18) !important;
}

.logo {
  right: 50%;
  top: 50%;
}

main {
  background-color: rgba(0, 0, 0, 0.932);
  height: 500px;
}

.bg-blue:hover {
  background-color: #002861dc;
  transition: all ease-in-out 0.4s;
}

.bg-red:hover {
  background-color: #6b0000dc;
  transition: all ease-in-out 0.4s;
}

.bg-yellow:hover {
  background-color: #787006dc;
  transition: all ease-in-out 0.4s;
}

.bg-green:hover {
  background-color: #003b08dc;
  transition: all ease-in-out 0.4s;
}

.bg-aqua:hover {
  background-color: #006c6edc;
  transition: all ease-in-out 0.4s;
}

.bg-purple:hover {
  background-color: #72017adc;
  transition: all ease-in-out 0.4s;
}
</style>
