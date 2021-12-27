<template>
  <div class="container mt-5">
    <div class="card">
      <div class="card-content">
        <div class="media">
          <div class="media-content">
            <p class="title is-4">Skills</p>
          </div>
        </div>

        <div class="content">
          <div class="columns is-multiline">
            <div class="column is-6" v-for="(data, i) in skills" :key="i">
              <Progress :lang="data.lang" :level="data.level" :num="data.num" :url="data.url" :color="data.color"/>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Progress from "../components/ProgressBar.vue";
export default {
  name: "Skills",
  components: { Progress },
  data(){
      return{
          skills:[
              {
                  lang: "JavaScript",
                  level: "Advanced",
                  num: "75",
                  url:"https://i.imgur.com/Buw4ffO.png",
                  color: "is-warning"
              },
              {
                  lang: "NodeJS",
                  level: "Advance",
                  num: "75",
                  url:"https://i.imgur.com/OOkygXN.png",
                  color: "is-primary"
              },
              {
                  lang: "VueJS",
                  level: "Advance",
                  num: "75",
                  url:"https://i.imgur.com/65QJ1B2.png",
                  color: "is-primary"
              },
              {
                  lang: "Python",
                  level: "Intermediate",
                  num: "50",
                  url:"https://i.imgur.com/ndkiuZV.png",
                  color: "is-info"
              },
              {
                  lang: "Java",
                  level: "Intermediate",
                  num: "50",
                  url:"https://i.imgur.com/kUCY1qD.png",
                  color: "is-danger"
              },
              {
                  lang: "C",
                  level: "Basic",
                  num: "25",
                  url:"https://i.imgur.com/b4GCbGs.png",
                  color: "is-link"
              },
              {
                  lang: "React Native",
                  level: "Basic",
                  num: "25",
                  url:"https://i.imgur.com/MRRGvZ4.png",
                  color: "is-info"
              },
              {
                  lang: "Golang",
                  level: "Basic",
                  num: "25",
                  url:"https://i.imgur.com/Pjv8dHw.png",
                  color: "is-info"
              },
          ]
      }
  }
};
</script>

<style></style>
