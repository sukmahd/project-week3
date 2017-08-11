<template>
  <v-flex offset-xs3 xs12>
    <div class="col-md-4">

      <!-- <ul>
        <div v-for="todo in todos">
          <div class="row">
            <a :href="'#'+todo.text" class="btn btn-info" data-toggle="collapse">{{todo.text}}</a>
            <hr>
            <div :id="todo.text" class="collapse">
              <input :value="todo.text"  @input="updateTodoText(todo, $event.target.value)">
              <input :value="todo.number" @input="updateTodoNumber(todo, $event.target.value)">
            </div>
            <hr>
          </div>
        </div>
      </ul> -->

      <ul>
        <div>
          <div class="row">

            <div class="text-xs-center">
            <v-card>
              <v-toolbar class="indigo" dark>
                <v-toolbar-title>Player 1</v-toolbar-title>
              </v-toolbar>
            </v-card>
          </div>

            <div class="text-xs-center">
              <v-btn round white>Player 1</v-btn>
            </div>

            <div class="text-xs-center">
              <v-menu offset-y>
                <v-btn primary dark slot="activator">Set Your Bet!!</v-btn>
                <v-list>
                  <v-list-tile v-for="todo in todos" :key="todo.number">
                    <v-list-tile-title>{{ todo.number }}</v-list-tile-title>
                  </v-list-tile>
                </v-list>
              </v-menu>
            </div>

            <div class="text-xs-center">
              <v-menu transition="scale-transition">
                <v-btn dark primary slot="activator">Set Your Bet!!</v-btn>
                <v-list>
                  <v-list-tile v-for="n in 6" :key="n">
                    <v-list-tile-title v-text="'Dice: ' + n"></v-list-tile-title>
                  </v-list-tile>
                </v-list>
              </v-menu>
            </div>

            <!-- <div class="text-xs-center">
              <v-menu transition="scale-transition">
                <v-btn dark primary slot="activator">Set Your Bet!!</v-btn>
                <v-list>
                  <v-list-tile v-for="n in 5" :key="n">
                    <v-list-tile-title v-text="'Dice: ' + n"></v-list-tile-title>
                  </v-list-tile>
                </v-list>
              </v-menu>
            </div> -->

          </div>
        </div>
      </ul>
    </div>
  </v-flex>
</template>

<script>
export default {
}
</script>

<style lang="css">
</style>
