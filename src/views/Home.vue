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
  margin-top: 20%;
  display: inline-block;
  height: 100vh;
  align-items: center;
  flex-wrap: wrap;
}

.give-your-vote{
  font-size: 21px;
}

.section{
  width: 100%;
}

.emoticons{
  display: flex;
  justify-content: center;
}

.finish{
  position: absolute;
  bottom: 20px;
  left: 35%;
}

</style>

