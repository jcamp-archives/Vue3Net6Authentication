<template>
  <div>
    <blockquote>
      &#8220;{{ props.quote }}&#8221;
      <footer>
        <small>
          <em>&mdash;<span v-html="props.author"></span></em>
        </small>
      </footer>
    </blockquote>
  </div>
</template>

<script setup lang="ts">

const props = defineProps({
  quote: String,
  author: String
})
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
