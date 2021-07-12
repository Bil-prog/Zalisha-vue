<template>
<v-container>
   <v-timeline
    align-top
    :dense="$vuetify.breakpoint.smAndDown"
  >
    <v-timeline-item
      v-for="(item, i) in items"
      :key="i"
      :color="item.color"
      :title="item.title"
      :content="item.content"
      :dot="item.dot"
    >
      <v-card
        :color="item.color"
        
      >
        <v-card-title  class="text-h6">
         {{ item.title }}
        </v-card-title>
        <v-card-text class=" text--black">
          {{ item.content }}
        </v-card-text>
      </v-card>
    </v-timeline-item>
    
  </v-timeline>
 </v-container> 
</template>

<script>
 export default {
   data: () => ({
      items: [
        { 
          title: 'Financial services',  
          content: 'we offer credit scoring services to our farmers to enable them access financial services',  
          color: '#81D4FA',
          dot: '#4CAF50',
        },
        {
          title: 'Precision farming',  
          content: 'access agronomy and weather information depending on your geolocation using IoT solutions using your phone',  
          color: '#A5D6A7',
          dot: '#4CAF50',
        },
        {
          title: 'Get market access',  
          content: 'do on farm record keeping, realtime and efficiently on zalisha,both for individual and co-operatives',  
          color: '#FFFFFF',
          dot: '#4CAF50',
        },
        {
          title: 'Contract farming',  
          content:'we enable contract farming through our interlinked solutions',  
          color: '#B2FF59',
          dot: '#4CAF50',
          
        },
        {
          title: 'Do record keeping',  
          content: 'we enable proper and automated record keeping using IoT solutions',  
          color: '#64FFDA',
          dot: '#4CAF50', 
        },
        
      ],
    }),

}
</script>

<style>

  
</style>