<template>
  
  <v-flex xs10 offset-xs1 class="scale-up-hor-center">
    <v-alert info value="true" id="rotate-scale-up" class="text-xs-center">
      Pemenang
    </v-alert>
    
  <h1 class="text-center">{{winner}}</h1>
    
  <div class="text-xs-center">
    <v-btn primary dark v-if="winner != ''" @click="resetRace()" type="button" name="button">Restart</v-btn>
  </div>
      <!-- <button v-if="winner != ''" @click="resetRace()" type="button" name="button">Restart</button> -->
  </v-flex>
</template>

<script>
  export default {
  }
</script>

<style>
.scale-up-hor-center {
	-webkit-animation: scale-up-hor-center 0.4s cubic-bezier(0.390, 0.575, 0.565, 1.000) both;
	        animation: scale-up-hor-center 0.4s cubic-bezier(0.390, 0.575, 0.565, 1.000) both;
}

@-webkit-keyframes scale-up-hor-center {
  0% {
    -webkit-transform: scaleX(0.4);
            transform: scaleX(0.4);
  }
  100% {
    -webkit-transform: scaleX(1);
            transform: scaleX(1);
  }
}
@keyframes scale-up-hor-center {
  0% {
    -webkit-transform: scaleX(0.4);
            transform: scaleX(0.4);
  }
  100% {
    -webkit-transform: scaleX(1);
            transform: scaleX(1);
  }
}

</style>