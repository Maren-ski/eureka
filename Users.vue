<template>
  <div>
    <p> {{ user.userName }} </p>

  </div>

</template>

<script>

  export default {
    name: "Users",
    props: ["user"]
  }
</script>
