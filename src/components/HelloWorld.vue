<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <div>
      <h1> Some Rad CheeseHeads </h1>
      <ul>
        <li v-for="person in sampleLoop">
          {{person.firstName}} {{person.lastName}}
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Hello',
  data () {
    return {
      msg: 'HelloWorld',
      sampleLoop: [ { firstName: 'Aaron', lastName: 'Rodgers' }, { firstName: 'Brett', lastName: 'Favre'}, { firstName: 'Justin', lastName: 'Gehr' }]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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
