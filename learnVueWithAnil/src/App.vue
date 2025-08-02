<template>
  <!-- <h1 v-if="headingHide === true">Home Component</h1>

  <button v-on:click="showHeading">click here</button>
  <button v-on:dblclick="getData('Button double clicked')">click here</button>
  <br />
  <br />
  <button @click="counter">counter {{ count }}</button> -->

  <!-- <h1>Email is: {{ email }}</h1>
  <h1>Number is: {{ number }}</h1>
  <h1>Name is: {{ name }}</h1> -->

  <!-- <VModel />	 -->
  <!-- <TwoWayBinding /> -->
  <!-- <ConditionalRendering /> -->
  <!-- <ConditionalRendering /> -->
  <!-- <ForLoopAndList /> -->
  <!-- <Child heading="Child Components" name="Polok Banik" :age=23 :usersDetails="users" :getData="getData" /> -->
  <!-- <Parent /> -->
  <!-- <HTMLBinding /> -->
  <!-- <ClassBinding /> -->
  <!-- <ChildToParentProps :passData="passData" /> -->
  <!-- <Ref /> -->
  <SimpleForm />
</template>

<script>
import CheckBoxAndRadioValue from "./components/CheckBoxAndRadioValue.vue";
import ConditionalRendering from "./components/ConditionalRendering.vue";
import TwoWayBinding from "./components/twoWayBinding.vue";
import VModel from "./components/VModel.vue";
import ForLoopAndList from "./components/ForLoopAndList.vue";
import HTMLBinding from "./components/HTMLBinding.vue";
import Child from "./components/Child.vue";
import Parent from "./components/reuseComponents/Parent.vue";
import ClassBinding from "./components/ClassBinding.vue";
import ChildToParentProps from "./components/ChildToParentProps.vue";
import SimpleForm from "./components/SimpleForm.vue";
import Ref from "./components/Ref.vue";
export default {
  components: {
    VModel,
    TwoWayBinding,
    CheckBoxAndRadioValue,
    ConditionalRendering,
    ForLoopAndList,
    Child,
    Parent,
    HTMLBinding,
    ClassBinding,
    Ref,
    ChildToParentProps,
    SimpleForm,
  },

  data() {
    return {
      users: [
        { name: "Polok", age: 23 },
        { name: "Nishan", age: 24 },
        { name: "Kopil", age: 25 },
        { name: "Showrov", age: 26 },
      ],
    };
  },

  methods: {
    getData() {
      alert("function is called");
    },

    passData(getName) {
      alert(getName);
    },
  },

  //   data() {
  //     return {
  //       //   name: "Polok Banik",
  //       //   email: "abc@gmail.com",
  //       //   number: 12345,
  //       headingHide: false,
  //       count: 0,
  //     };
  //   },
  //   methods: {
  //     getData(getValue) {
  //       alert(getValue);
  //     },
  //     getConsole() {
  //       console.warn("mouse down the heading");
  //     },
  //     showHeading() {
  //       this.headingHide = !this.headingHide;
  //     },
  //     counter() {
  //       this.count++;
  //     },
  //   },
};
</script>

<style scoped></style>
