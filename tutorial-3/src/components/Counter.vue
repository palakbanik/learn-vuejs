<template>
  <div class="main-container">
    <h1>Counter</h1>
    <div>
      <button @click="increment">Increase</button>
      <h3 class="static" :class="{ active: isActive, 'text-danger': hasError }">
        {{ count }}
      </h3>
      <button @click="decrement">Decrement</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      count: 0,
      isActive: false,
      hasError: false,
    };
  },
  methods: {
    increment() {
      this.count++;
      if (this.count > 0) {
        this.isActive = true;
        this.hasError = false;
      }
    },
    decrement() {
      this.count--;
      if (this.count <= 0) {
        this.isActive = false;
        this.hasError = true;
      }
    },
  },
};
</script>

<style scoped>
.main-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

div {
  display: flex;
  gap: 10px;
}

h3 {
  font-size: 50px;
}

button {
  background: gray;
  color: white;
  font-size: 20px;
  padding: 10px 15px;
  border: none;
  border-radius: 20px;
  cursor: pointer;
}

.active {
  color: red;
}
.text-danger {
  background-color: gray;
}
</style>
