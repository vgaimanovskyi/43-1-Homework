<template>
  <div class="mainer">
    <input type="text" v-model.lazy="num" />
    <button v-on:click="num--">-</button>
    <p>{{num}}</p>
    <button v-on:click="num++">+</button>
  </div>
</template>

<script>
export default {
  props: ["num"],
  data() {
    return {};
  }
};
</script>
<style lang="scss">
.mainer {
  width: 200px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  border: 1px solid #000;
  background-color: #ccc;
  padding: 15px;
  text-align: center;
}
input {
  width: 100%;
  padding: 5px;
  margin: 0 0 10px 0;
  text-align: center;
}
p {
  display: inline-block;
  width: 100px;
}
</style>