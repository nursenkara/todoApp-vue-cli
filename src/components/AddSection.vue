<template>
<div>
<label for="todoText"></label>
<input  v-model ="todoText" @keydown.enter = "addNewTodo(todoText)" type="text" id = "todoText" placeholder="Bir şeyler yazınız...">

</div>
</template>

<script>
export default {
    props: {
        addNewTodo: () => {
        }
    },
    data(){
        return{
            todoText:null
        };
    },
    methods:{
       // addNewToDo(){
       //    this.$emit("add-todo",this.todoText);
        //   this.todoText = null;
      //  }
    }
};
</script>