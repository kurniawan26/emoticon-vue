<template>
  <div class="container">
    <section class="vote">
      <h3 class="give-your-vote">
        Silahkan Berikan Penilaian Anda Terhadap Layanan Kami
      </h3>
      <div class="emoticons">
        <vote/>
      </div>
    </section>
    <section class="finish">
      <h4>Terimakasih telah memberikan penilaian anda</h4>
    </section>
  </div>
</template>

<script>
// @ is an alias to /src
import Vote from '../components/Vote.vue';

export default {
  name: 'Home',
  components: {
    Vote
  }
};
</script>

.<style>
.container{
  display: flex;
  height: 100vh;
  align-items: center;
  flex-wrap: wrap;
}

.emoticons{
  display: flex;
}
section{
  width: 100%;
}
</style>

