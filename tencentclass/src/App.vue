<template>
  <div id="app">
    <div class="top-box">
      <!-- <search /> -->
    </div>
    <div class="center-box">
      <banner />
    </div>
  </div>
</template>

<script>
import banner from "./components/banner";

export default {
  name: "App",
  data: function () {
    return {
      msg: "hello ，大家好！",
      Loading: false,
    };
  },
  components: {
    // search,
    banner,
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
}

ul {
  list-style: none;
}

.top-box {
  position: fixed;
  left: 0;
  top: 0;
  z-index: 100;
  width: 100%;
}

.center-box {
  margin-top: 45px;
  margin-bottom: 45px;
}

.bottom-box {
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;
}

.Loading {
  z-index: 1000;
}
</style>
