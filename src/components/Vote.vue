<template>
  <div class="buttons">
    <button
      v-for="(emoticon, index) in emoticons"
      :key="index"
      :id="emoticon"
      :value="emoticon"
      class="btn-emoticon"
      @click="vote"
    ></button>
  </div>
</template>

<script>
// @ is an alias to /src
import moment from "moment";

export default {
  name: "Home",
  components: {},
  data: function () {
    return {
      emoticons: ["very-bad", "bad", "ok", "good", "very-good"],
    }
  },
  methods:{
    vote(e){
      var voted = e.target.value;

      var waktu = moment().format('MMMM Do YYYY, h:mm:ss a');

      localStorage.setItem('vote', voted)
    }
  }
};
</script>

.<style>
.buttons{
  display: flex;
}

.btn-emoticon{
  background: url('../assets/emoticon.png');
  width: 101px;
  height: 100px;
  border: none;
  margin: 0px 10px;
}

#very-bad{
  background-position: 0px 0px;
}

#very-bad:hover{
  background-position: 0px -100px;
}

#very-bad:hover:active{
  background-position: 0px -200px;
}

#bad{
  background-position: -101px 0px;
}

#bad:hover{
  background-position: -101px -100px;
}

#bad:hover:active{
  background-position: -101px -200px;
}

#ok{
  background-position: -202px 0px;
}

#ok:hover{
  background-position: -202px -100px;
}

#ok:hover:active{
  background-position: -202px -200px;
}

#good{
  background-position: -303px 0px;
}

#good:hover{
  background-position: -303px -100px;
}

#good:hover:active{
  background-position: -303px -200px;
}

#very-good{
  background-position: -404px 0px;
}

#very-good:hover{
  background-position: -404px -100px;
}

#very-good:hover:active{
  background-position: -404px -200px;
}
</style>