<template>
    <section id="section2" data-aos="fade-in" class="cd-section section-about-me">
      <div class="container-fluid" style="text-align:center;">
        <div class="row">
          <div class="col-md-5">
            <img src="../assets/img/about-me.jpg" alt="" style="height:550px; width:auto;">
          </div>
          <div class="col-md-6 div-about-me">
            <span class="about-me">
              Ab<span class="about-me-border">out</span> Me
            </span>
            <p class="about-me-content">
              Hi! I am Krit , a {{calculate_age()}} year self-motivated Web Developer with some experience of working on multiple projects. Passionate and hardworking with penchant for meeting deadlines. Interested in role with company promoting best practices and offering diverse projects and learning.
            </p>
            <p class="about-me-content">Currently seeking <strong>opportunitites</strong> as a <br> <strong style="color: #0cb4ce">Web Developer   <strong>|</strong>   Software Developer</strong></p>
          </div>
          <div class="col-md-1"></div>
        </div>
      </div>
    </section>
</template>

<script>
export default {
    methods:{
      calculate_age() { 
        var dob=new Date(1998, 11, 7);
        var diff_ms = Date.now() - dob.getTime();
        var age_dt = new Date(diff_ms); 
        return Math.abs(age_dt.getUTCFullYear() - 1970);
      }
    }
}
</script>

<style scoped>

/* ABOUT ME */
.section-about-me{
  padding: 5rem 0;
  box-shadow: 0px 1px 5px 1px #e0dbdb47;
  /* background-color:#0d0d0d; */
}
.about-me {
  font-size: 64px;
  font-weight: 700;
  color: #303133;
}
.about-me-border {
  position: relative;
  
}
.about-me-border::after {
  position: absolute;
  content: "";
  border-bottom: 2px solid #0cb4ce;
  bottom: 0;
  left: 20%;
  width: 75%;
  margin-bottom: -15%;
}
.about-me-content {
  margin: 60px 0;
  line-height: 1.75;
  color: #777777;
}
.about-me-content  strong{
  color: #303133;
  font-weight: 500;
}

/* ABOUT ME */
</style>
