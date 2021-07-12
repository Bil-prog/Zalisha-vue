<template>
      <v-container>
      <v-item-group
        multiple
      >
        <v-row>
          <v-col
            v-for="(item, i) in items"
            :key="i"
            cols="12"
            sm="4"
          >
            <v-item>
              <v-img
                :src="item.src"
                height="330"
                width="500"
              >

              </v-img>
            </v-item>
          </v-col>
        </v-row>
      </v-item-group>
    </v-container>
</template>

<script>
export default {
    data: () => ({
      items: [
        {
          src: 'zalisha1..PNG',
        },
        {
          src: 'zalisha2..PNG',
        },
      ],
    }),

}
</script>

<style>

</style>