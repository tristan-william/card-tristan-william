<template>
  <div class="home">
      <ul>
        <li v-for="(list,index) in lists" :key="index">{{list.name}}</li>
        <About></About>
      </ul>
  </div>
</template>

<script>
// @ is an alias to /src
import About from './About'
export default {
  name: 'home',
  components: {
    About,
  },
  data(){
    return {
      lists:[
        { name:'彭于晏', age:'18', hobby:'read'},
        { name:'吴彦祖', age:'18', hobby:'read'},
        { name:'霍建华', age:'18', hobby:'read'},
      ],
    }
  },
};
</script>
