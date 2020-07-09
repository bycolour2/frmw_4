<template>
  <div>
    <span>{{ base }}</span
    ><sup>{{ exp }}</sup> = {{ base ** exp }}
  </div>
</template>

<script>
export default {
  name: "Deg",
  props: {
    base: {
      type: Number
    },
    exp: {
      type: Number
    }
  }
};
</script>

<style></style>
