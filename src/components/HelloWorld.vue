<template>
  <div>
    <input class='input-form' v-model='newTask' v-on:keyup.enter="addItem" placeholder='Enter task here'>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    newTask: '',
    tasks: ['one', 'two', 'three'],
  },
  data: function () {
    return { mutableList: JSON.parse(this.tasks)};
  },
  methods:{
    addItem: function(){
      this.tasks.push(this.newTask);
      this.newTask = '';
      console.log(tasks);
    }
  }

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
</style>
