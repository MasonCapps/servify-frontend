<script>
import axios from "axios";

export default {
  created: function () {
    delete axios.defaults.headers.common["Authorization"];
    localStorage.removeItem("jwt");
    this.$router.push("/sites/1");
  },
};
</script>

<template>
  <div class="logout"></div>
</template>
