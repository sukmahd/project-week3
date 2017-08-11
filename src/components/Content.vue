<template>
  <v-flex offset-xs3 xs12>
    <div class="row">
      <div class="col-md-8">
        <p v-for="dice in dices">{{dice.dice}}
          <v-btn fab dark large class="orange" @click="randomDadu(dice)" type="button" name="button">
            <v-icon dark>gamepad</v-icon>
          </v-btn>
        </p>
        <p>{{hasil}}</p>  
        <div>
          <v-list-tile>
            <template v-for="todo in todos">
              <v-list-tile-title>test</v-list-tile-title>
              <v-list-tile-score>score</v-list-tile-score>
            </template>
          </v-list-tile>          
        </div>
      </div>
    </div>
  </v-flex>
</template>

<script>
export default {
  data () {
    return {
      dices: [
        { dice: 'test dice' }
      ],
      todos: [
        { todo: 'test todo' }
      ]
    }
  }
}
</script>

<style lang="css">
</style>
