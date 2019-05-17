<template>
  <div>
    <el-select v-model="value" placeholder="Select">
      <el-option
              v-for="item in options"
              :key="item.value"
              :label="item.label"
              :value="item.value"
              :disabled="item.disabled">
      </el-option>
    </el-select>
  </div>
</template>

<script>

export default {
    name: 'mainClock',
    data() {
      return {
        selected: 'Japan',
        options: [
          { value: -9, label: 'Japan', disabled: false },
          { value: 0, label: 'UK', disabled: false },
          { value: 4, label: 'USA', disabled: false }
        ]
      }
    },
    methods: {
        addCountry() {
            let gmt = (new Date()).toGMTString()
            this.word = gmt
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
