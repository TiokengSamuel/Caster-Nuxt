<template>
<div class="videos">
  <Nuxt-Child />
  <h1>videos</h1>
  <div v-for="video in videos" :key="video.id">
    <p>{{video.name}}</p>
  </div>
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
}
</script>

<style>

</style>