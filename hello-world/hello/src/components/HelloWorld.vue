<template>
  <div class="hello">
    <!-- <h1>{{ msg }}</h1> -->
  <p @click="aa">aaaaaaaaaa</p>
  
 
    <el-date-picker
      v-model="monthVal"
      type="month"
      @change="monthChange"
      value-format="yyyy-MM"
      placeholder="选择月">
    </el-date-picker>
 



  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data(){
    return{
        monthVal: '',
      
    }
  },
  created(){
  },
  mounted(){
    this.init()
  },
  methods:{
    init(){
    },
    aa(){
      console.log(1111)
    },
    monthChange(){
      console.log(this.monthVal)
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
