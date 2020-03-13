<template>
    <div class="tweet-container">
        <div class="tweet-author"><h3>{{ author }}</h3></div>
        <div class="tweet-content"><p>{{ content }}</p></div>
        <div class="tweet-date"><i>{{ date }}</i></div>
    </div>
</template>
<script>
export default {
  name: 'Tweet',
  props: {
    author: String,
    content: String,
    date: String
  }
}
</script>

<style scoped>
    .tweet-container {
        width : 20vw;
        height : 25vh;
        border : 1px solid black;        
    }
</style>
