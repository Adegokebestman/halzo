<template>
  <div>
      <form @submit="addTodo">
          <input type="text" v-model="title" name="todo" placeholder="Add Todo">
          <input type="submit" class="btn" value="add">
      </form>
      </div>  
</template>


<script>
// import uuid from 'uuid';
// import { v4 as uuidv4 } from 'uuid';
export default {
 name: "addTodo", 
 data() {
    return {
        title: ''
    } 
},
methods: {
    addTodo(e){
        e.preventDefault();
        const newTodo = {
            // id: uuidv4(),
            title: this.title,
            completed: false
        }
    // send data to parent
    this.$emit('add-todo', newTodo); 
    this.title = '';
    }
}

}
</script>



<style scoped>
form{
    display: flex;
}
input[type="text"]{
    flex: 10;
    padding: 5px;
}
input[type="submit"]{
    flex: 2;
}
</style>