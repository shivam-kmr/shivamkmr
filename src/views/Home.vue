<template>
  <div class="home">
    <Profile />
  </div>
</template>

<script>
// @ is an alias to /src
import Profile from "@/components/Profile.vue";

export default {
  name: "Home",
  title: "Shivam Kumar - Home",
  components: {
    Profile
  }
};
</script>
