<template>
    <div class="hero" :style="`background-image: url(${bgImage})`">

    </div>
</template>

<script>
export default {
    name: "Hero",
    props: ["bgImage"]
}
</script>

<style>
    .hero{
        height: 400px;
  }
</style>