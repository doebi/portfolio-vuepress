<template>
  <!--
  <h1 class="title">Wir reden nicht viel, wir machen einfach. Und das nicht irgendwie sondern <voi-guat /></h1>
  -->
  <h1 class="title">Unsere Arbeit beginnt wo andere aufhören. Wir sind nicht irgendwer sondern <voi-guat /></h1>
</template>

<script>
export default {
  props: {
  }
}
</script>

<style scoped>
  .title {
    text-align: center;
    font-size: calc(21px + (48 - 14) * ((100vw - 300px) / (1600 - 300)));
    font-weight: 300;
    line-height: 1.25;
    letter-spacing: 0.1rem;
    width: 800px;
    max-width: 100%;
    margin: 18vw auto 7vw auto;
  }

  @media screen and (min-width: 600px) {
    .title {
      margin: 12vw auto 7vw auto;
    }
  }

</style>
