<template>
  <div>
      We are in video {{$route.params.id}}
  </div>
</template>

<script>
export default {
  data() {
        return{
            videos: [{
                    id: "16",
                    name: "Intro in Nuxt"
                },
                {
                    id:"1",
                    name: "Intro in Vue"
                },
                {
                    id: "10",
                    name: "Advanced concepts"

                }]
        }
    },
    computed: {
      videos() {
        return this.videos.find(v => v.id == this.$route.params.id)
      }
    }
}
</script>

<style lang="scss" scoped>

</style>

</style>