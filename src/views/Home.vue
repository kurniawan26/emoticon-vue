<template>
  <div class="container">
    <section class="vote">
      <h3 class="give-your-vote">
        Silahkan Berikan Penilaian Anda Terhadap Layanan Kami
      </h3>
      <div class="emoticons">
        <vote :voteProp="vote"/>
      </div>
    </section>
    <section class="finish ">
      <transition name="fade">
      <h4 v-if="show">Terimakasih telah memberikan penilaian anda</h4>
      </transition>
    </section>
  </div>
</template>

<script>
// @ is an alias to /src
import Vote from '../components/Vote.vue';

export default {
  name: 'Home',
  data: function(){
    return{
      show: false
    }
  },
  components: {
    Vote
  },
  methods:{
    vote(){
      this.show = true;
    }
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

