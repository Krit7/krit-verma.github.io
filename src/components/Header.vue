<template>
  <section>
    <nav id="cd-vertical-nav">
      <ul>
        <li>
          <a href="#section1" data-number="1">
            <span class="cd-dot"></span>
            <span class="cd-label">Home</span>
          </a>
        </li>
        <li>
          <a href="#section2" data-number="2">
            <span class="cd-dot"></span>
            <span class="cd-label">About Me</span>
          </a>
        </li>
        <li>
          <a href="#section3" data-number="3">
            <span class="cd-dot"></span>
            <span class="cd-label">My Work</span>
          </a>
        </li>
        <li>
          <a href="#section4" data-number="4">
            <span class="cd-dot"></span>
            <span class="cd-label">Contact</span>
          </a>
        </li>
      </ul>
    </nav>
    <a class="cd-nav-trigger cd-img-replace">
      Open navigation
      <span></span>
    </a>

    <section id="section1" class="cd-section main">
      <div class="container">
        <div class="row">
          <div class="col-md-12">
            <div class="content">
              <transition name="animated fadeInDown delay-1s" appear>
                <div>
                  <h2 class="header">I am</h2>
                  <transition name="fade" appear mode="out-in">
                    <span v-if="show==0" key="1" class="fadeContent">Krit Verma</span>
                    <span v-if="show==1" key="2" class="fadeContent">a Programmer</span>
                    <span v-if="show==2" key="3" class="fadeContent">a Developer</span>
                    <span v-if="show==3" key="4" class="fadeContent">a Researcher</span>
                  </transition>
                </div>
              </transition>
            </div>
            <transition name="animated fadeInUp delay-1s" appear>
              <div class="cd-down-arrow">
                <a href="#section2" class="cd-img-replace down-arrow">scroll down</a>
              </div>
            </transition>
          </div>
        </div>
      </div>
    </section>
    <AboutMe></AboutMe>
    <MyWork></MyWork>
    <contact-me></contact-me>
  </section>
</template>

<script>
import AboutMe from "./AboutMe.vue";
import MyWork from "./MyWork.vue";
import ContactMe from "./ContactMe.vue";
export default {
  data() {
    return {
      show: 0,
      val: false
    };
  },
  methods: {},
  created() {
    setInterval(() => {
      this.show = (this.show + 1) % 4;
    }, 4800);
  },
  components:{
    AboutMe:AboutMe,
    MyWork:MyWork,
    ContactMe:ContactMe,
  }
};
</script>
<style scoped>

/* HOME */
@import "../assets/css/style.css";
@import "../assets/css/reset.css";

.main {
  background-image: url("../assets/img/background-doodle.png");
  background-repeat: no-repeat;
  background-position: center top;
  background-size: cover;
  box-shadow: 0px 1px 5px 1px #e0dbdb47;
}

.content {
  text-align: center;
  margin-top: 17%;
  margin-left: -3%;
}
.header {
  font-size: 84px;
  line-height: 1.2;
  font-weight: 600;
  margin-bottom: 3%;
}
.fadeContent {
  color: #0cb4ce;
  font-size: 84px;
  line-height: 1.2;
  font-weight: 600;
  position: relative;
}

.fade-enter {
  opacity: 0;
}
.fade-enter-active {
  animation: width-in 1s ease-out forwards;
  transition: 1s;
}
.fade-leave {
  opacity: 1;
}
.fade-leave-active {
  animation: slide-out 1s ease-out forwards;
  transition: 1s;
  opacity: 0;
}

.fadeContent::after {
  position: absolute;
  left: 2%;
  width: 0;
  content: "";
  border-top: 3px solid #0cb4ce;
  bottom: -20px;
  transition: width 3.2s cubic-bezier(0.2, -0.36, 0.39, 0.94);
}

.fadeContent:hover::after {
  width: 96%;
}

.down-arrow {
  text-align: center;
  height: 75px;
  width: 75px;
  border: 0.02rem solid #303133;
  border-radius: 50%;
  position: relative;
  left: 45%;
  right: auto;
  margin: 6% 0;
  background-image: url("../assets/img/download-arrow2.png");
  background-size: 30px;
  background-repeat: no-repeat;
  background-position: 22px; 
}
.down-arrow:hover {
  background-color: #272727;
  background-image: url("../assets//img/download-arrow3.png");
}

/* HOME */


</style>
