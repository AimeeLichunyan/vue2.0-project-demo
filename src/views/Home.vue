<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <el-radio
      v-model="value"
      @click.native.prevent="changeIsRelative()"
      :label="true"
      >选我
    </el-radio>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
  data() {
    return {
      value: false,
    };
  },
  methods: {
    changeIsRelative() {
      this.value = !this.value;
    },
  },

  components: {
    HelloWorld,
  },
};
</script>
