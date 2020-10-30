<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p> 
      {{ msg2 }}
      {{ message }}
  <input v-model="message">


    </p>

    <button
      type="button"
      class="btn btn-warning btn-sm"
      @click="editBook(msg)">
      Update
    </button>
    
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data: function() {
    return {
      message: "Wagner", num2: ""
    }
  },   
  props: {
    msg: String,
    msg2: String,
    
  },
  methods: {
    getBooks() {
      const path = 'Hola has create';
      console.log(path);
        
    },
    addBook(payload) {
      const path = 'http://localhost:5001/books';
      console.log(path+payload);
    },
    editBook(cad) {
      console.log("edit "+cad+": "+this.message);
      
    },
  },
  created() {
    this.getBooks();
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.hello {
color: #1cca9f;
font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
}
</style>