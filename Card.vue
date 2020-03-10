<template>
  <div
  id="e3"
  style="max-width: 600px; margin: auto;"
  class="grey lighten-3"
  >
    <v-container
      fluid
      style="min-height: 0;"
      grid-list-lg
    >
      <v-layout row wrap>
        <v-flex xs12>
          <v-card target="_blank" :href="url" :color="color" class="white--text">
            <v-container fluid grid-list-lg>
              <v-layout row>
                <v-flex xs7>
                  <div>
                    <h1 class="headline">{{title}}</h1>
                    <h2>{{artistName}}</h2>
                  </div>
                </v-flex>
                <v-flex xs5>
                    <v-card-media
                      :src="image"
                      height="100px"
                      contain
                    ></v-card-media>
                </v-flex>
              </v-layout>
            </v-container>
          </v-card>
        </v-flex>
      </v-layout>
    </v-container>
  </div>

</template>
<script>
export default {
  props: ['title', 'image', 'artistName', 'url', 'color']

}
</script>
 <div class="product">
    <div :class="'product-inner ' + product.color">
      <div class="product-text-wrap">
        <h2 class="bg-text">{{ product.bgtext }}</h2>
      </div>
      <div class="product-image-wrap">
        <img :src="product.src" class="image" />
      </div>
      <div class="product-detail">
        <h2>{{ product.title }}</h2>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Incidunt eligendi sed cupiditate eius dolores consequatur explicabo dignissimos magnam amet eveniet!</p>
      </div>
    </div>
  </div>
