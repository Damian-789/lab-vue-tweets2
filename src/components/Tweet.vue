<template>
  <div className="tweet">
    <img
      src="https://i.imgur.com/9yw1Fyw.jpg"
      className="profile"
      alt="profile"
    />

    <div className="body">
      <div className="top">
        <span className="user">
          <span className="name">{{tweet.user.name}}</span>
          <span className="handle">@{{tweet.user.handle}}</span>
        </span>

        <span className="timestamp">Nov 30, 2020</span>
      </div>

      <p className="message">
        {{ tweet.message }}
      </p>

      <div className="actions">
        <!-- Font Awesome icons -->
        <i class="far fa-comment"></i>
        <i class="fas fa-retweet"></i>
        <i class="far fa-heart"></i>
        <i class="fas fa-share"></i>
      </div>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>



<script setup>
const props = defineProps(["tweet"]);

</script>





<style scoped>
a {
  color: #42b983;
}
</style>
