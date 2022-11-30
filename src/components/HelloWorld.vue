<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <EasyPlayer id="EasyPlayer" videoUrl="http://192.168.100.53:8080/live/ch04_1.flv" fluent>
    </EasyPlayer>
  </div>
</template>

<script>
import EasyPlayer from '@easydarwin/easyplayer'
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      
    }
  },
  components: {
    EasyPlayer
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello{
  display: align;
  background-color: blue;
}

#EasyPlayer {
  width: 750px;
  height: 500px;
  margin: 0 auto;
}

</style>
