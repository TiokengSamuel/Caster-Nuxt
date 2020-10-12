<template>
<div class="videos">
  <h1>videos</h1>
  <div v-for="video in videos" :key="video.id"></div>
  {{videos.id}}
</div>
</template>

<script>
export default {
    data() {
        return{
            videos: [
                {
                    id: '16',
                    name: 'Intro in Nuxt'
                },
                {
                    id: '21',
                    name: 'Intro in Vue'
                },
                {
                    id: '10',
                    name: 'Advanced concepts'

                }
            ]
        }
    },
}
</script>

<style lang="scss" scoped>

</style>