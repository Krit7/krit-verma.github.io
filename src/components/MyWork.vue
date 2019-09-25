<template>
    <section id="section3" data-aos="fade-in" class="cd-section section-my-work">
      <div class="container-fluid" style="text-align:center;">
        <div class="row">
          <div class="col-md-12">
              <h2 class="my-work">M<span class="my-work-border">y W</span>ork</h2>
              <div class="work-quote">
                <p>Don't Be <strong>Busy.</strong> Be <strong>Productive.</strong></p>
              </div>
          </div>
        </div>
      </div>
      <div class="container-fluid project-container">
        <div class="row project-row">
            <li class="col-lg-4 col-md-6 project-col" v-for="(project,i) in projects" v-bind:key="i">
                <div v-if="i%2==0" data-aos="fade-up" data-aos-duration="1500" class="project-hover-div">
                    <a :href="project.Link" target="blank" class="project-link">
                        <div class="container project-box">
                            <div class="project-details">
                                <h4 class="project-title">{{project.Name}}</h4>
                                <hr class="divider">
                                <p class="project-description">{{project.Description}}</p>
                            </div>
                        </div>
                    </a>
                </div>
                <div v-else data-aos="fade-down" data-aos-duration="1500">
                    <a :href="project.Link" target="blank" class="project-link">
                        <div class="container project-box">
                            <div class="project-details">
                                <h4 class="project-title">{{project.Name}}</h4>
                                <hr class="divider">
                                <p class="project-description">{{project.Description}}</p>
                            </div>
                        </div>
                    </a>
                </div>
            </li>
        </div>
      </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            projects:[
                {
                    Name:"Publication",
                    Description: "Title: - Mapping Robotic Affordances with Pre-requisite Learning Interventions for Children with Autism Spectrum Disorder",
                    Link: "#"
                },
                {
                    Name:"Blog Site",
                    Description: "A blog site for single user built on Node.js, using REST-Api and CRUDE commands and MongoDB as a database",
                    Link: "https://github.com/Krit7/Blog-Site-RESTAPI"
                },
                {
                    Name:"Color Game",
                    Description: "A colour guessing game from rangomly generated RGB values",
                    Link: "https://github.com/Krit7/Color-Game"
                },
                {
                    Name:"Do I Know You",
                    Description: "A gadget, which offers you security at your house from unwanted accident and for security purposes",
                    Link: "https://sites.google.com/iiitd.ac.in/doiknowyou/home?authuser=0"
                },
                {
                    Name:"Library Management System",
                    Description: "Library Management system built on Node.js and MongoDB as database with Facebook and Google login support and Instamojo payment gateway",
                    Link: "https://github.com/Krit7/Library-Management-System"
                },
                {
                    Name:"Mini Quiz App",
                    Description: "A vue application built while learning, using transition effects ",
                    Link: "https://github.com/Krit7/Mini-Quiz-App"
                },
                {
                    Name:"Patatap Clone",
                    Description: "A website with audio and visual effects built while exploring various API's",
                    Link: "https://github.com/Krit7/Patatap-Clone"
                },
                {
                    Name:"Cinntra.com",
                    Description: "Designed and maintainted this website during my internship",
                    Link: "http://cinntra.com/"
                },
                {
                    Name:"QuizzWizz",
                    Description: "Designed the landing page for this website during my internship",
                    Link: "https://github.com/Krit7/QuizzWizz"
                }
            ]
        }
    }
}
</script>

<style scoped>

.section-my-work{
    padding: 5rem 0 0 0;
    box-shadow: 0px 1px 5px 1px #e0dbdb47;
}
.my-work{
  font-size: 64px;
  font-weight: 700;
  color: #303133;
}

.work-quote{
    font-size: 18px;
    line-height: 1.75;
    margin: 18px 0px 0px 0px;
    color: #777777;
}

.my-work-border {
  position: relative;
  
}
.my-work-border::after {
  position: absolute;
  content: "";
  border-bottom: 2px solid #0cb4ce;
  bottom: 0;
  left: 20%;
  width: 75%;
  margin-bottom: -65%;
}

.project-container{
    padding: 0px;
    margin: 75px 0 0 0;
}

.project-col{
    padding: 0 1px 2px 1px;
    list-style: none;
}

.project-hover-div:hover{
    background-color: pink;
    color: black;
    z-index: 999;
}

.project-link:hover{
    color: white;
    text-decoration: none;
}

.project-row{
   margin: 1px;
}

.project-box{
    background-color: #4e5052;
    text-align: center;
    width: 100%;
    height: 360px;
}

.project-details{
    color: white;
    padding: 135px 10px 10px 0;
}

.project-title{
    font: 900;
}

.divider{
    border: 0.3px solid white;
}

.project-description{
    line-height: 1.5;
}
</style>