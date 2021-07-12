<template>
  <div class="home">
    <div class="row"
    >
    <div id="col">
    <v-card
    max-width="550"
    id="card"
    class="hidden-sm-and-down"
    >
    <v-list-item>
      <v-list-item-content class="text-left">
   
        <v-list-item-title class="font-weight-bold become">
           BECOME A DIGITAL FARMER
        </v-list-item-title>
        <v-list-item-subtitle class= "blue--text join" style="font-size: 38px;">Join the fastest growing </v-list-item-subtitle>
        <v-list-item-subtitle class= "blue--text join" style="font-size: 38px;">digital farming platform</v-list-item-subtitle>
        <v-card-text class="text-left" id="why">
          Why struggle to <strong>access information, markets, finance</strong> or <strong> record keeping </strong>in your farm? With <strong>zalisha</strong> we give you the platform you need to enable your growth
        </v-card-text>
      </v-list-item-content>

  
    </v-list-item>

    <v-card-actions>
      <v-btn
        color="#4CAF50"
        dark
      >
        JOIN NOW
      </v-btn>
    </v-card-actions>

    </v-card>
  </div>  

<div id="col">
  <v-carousel 
     cycle
     hide-delimiters
     show-arrows-on-hover
     class="hidden-sm-and-down"
     style="max-width: 300px; justify-content: center; margin-left: 0px;">
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      max-width="280"
    ></v-carousel-item>
  </v-carousel>
</div>  

</div>
<v-carousel 
     cycle
     hide-delimiters
     show-arrows-on-hover
     class="hidden-md-and-up"
     style="max-width: 300px; justify-content: center; margin-left: 0px;">
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      max-width="280"
    ></v-carousel-item>
  </v-carousel>
    <br>
<p class="text-center blue--text join">Enabling small scale farmers</p>
<p class="text-center become">We walk you the journey to achieve success in agriculture as a farmer
by providing what you need at the right moment through zalisha</p>

  <v-btn
    color="#4CAF50"
    dark
    :style="{left: '50%', transform:'translateX(-50%)'}"
  >
     <v-icon>mdi-google-play</v-icon>DOWNLOAD ZALISHA
  </v-btn>

  <br>
  
  <Timeline />

  <p class="text-center blue--text join">Zalisha for businesses</p>
<p class="text-center become">We provide a platform for farming companies , aggregators, farm input providers
and farmer cooperatives manage their activities and operations through zalisha
</p>

  <v-btn
    color="#4CAF50"
    dark
    :style="{left: '50%', transform:'translateX(-50%)'}"
  >
     request zalisha for businesses
  </v-btn>

  <br>
<Projects />


  </div>
</template>

<script>
import Timeline from '../components/timeline.vue';
import Projects from '../components/projects.vue';
  export default {
    components: { Timeline, Projects,},

  
    data () {
      return {
        items: [
          {
            src: 'mok3.png',
          },
          {
            src: 'market.svg',
          },
          {
            src: 'farm.svg',
          },
          {
            src: 'newsfeed.svg',
          },
        ],
      }
    },
  

  }

</script>

<style>
.row{
  display: flex;
  justify-content: space-around;
}
.become{
  font-size: 26px;
}
.join{
  font-size: 38px;
}
#why{
  font-size: 20px;
  line-height: 1.8em;

}
.home{
  margin-top: 100px;
  margin-left: 40px;
}
#card{
  padding: 18px;
}

</style>