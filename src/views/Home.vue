<template>
  <div class="container">
    <section class="vote">
      <h3 class="give-your-vote">
        Silahkan Berikan Penilaian Anda Terhadap Layanan Kami
      </h3>
      <div class="emoticons">
        ini akan menjadi komponen vote
      </div>
    </section>
    <section class="finish">
      <h4>Terimakasih telah memberikan penilaian anda</h4>
    </section>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  components: {
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
section{
  width: 100%;
}
</style>

