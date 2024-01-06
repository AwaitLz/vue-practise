<template>
  <div>
    <p>姓名:{{ name }}</p>
    <p>年龄:{{ age }}</p>
    <p @click="sayHello(10)">说话</p>
  </div>
</template>

<script>
export default {
  name: "App",
  setup() { //为一个函数
     //定义变量 
    let name = "张三";
    let age = 20;
     // 定义方法
    function sayHello(m) {
      alert(`${name}--${age}--${m}`);
    }
    return { //setup函数返回值为一个对象
      name,
      age,
      sayHello,
    };
  },
};
</script>










<!-- <template>
  <div class="person">
    {{ name }}
    <button @click="onclickHandle">点击</button>
  </div>
</template>


<script>
  export default {
    name: "PersonCom",
    data() {
      return {
        name: 'vue'
      }
    },
    methods: {
      onclickHandle () {
        this.name = 'react'
      }
    }
  }

</script>

<style scoped>
.person {
  width: 300px;
  margin: 10px;
  padding: 20px;
  background: rebeccapurple
}
</style> -->
