<template>
    <section id="section4" data-aos="fade-in" class="cd-section section-contact-me">
        <div class="container-fluid parallax">
            <div class="row">
                <div class="col-md-12">
                    <h4 class="get-in-touch">Get <span class="get-in-touch-border">in t</span>ouch</h4>
                </div>
            </div>
            <div class="row contact-row">
                <div class="border-col"></div>
                <div class="col-lg-3 col-md-3 col-sm-1 col-contact-details">
                    <div class="contact-content">
                        <div class="contact-favicon">
                            <i class="fa fa-envelope-o fa-5x fa-class" aria-hidden="true"></i>
                        </div>
                        <h4 class="contact-header">Drop A Line</h4>
                        <span>
                            <a href="mailto:kritverma27@gmail.com" target="blank" class="contact-link">kritverm27@gmail.com</a>
                        </span>
                    </div>
                </div>
                <div class="col-lg-3 col-md-3 col-sm-1 col-contact-details">
                    <div class="contact-content">
                        <div class="contact-favicon">
                            <i class="fa fa-mobile fa-5x fa-class" aria-hidden="true"></i>
                        </div>
                        <h4 class="contact-header">Contact</h4>
                        <span>
                            <a class="contact-link">+91-9999366967</a>
                        </span>
                    </div>
                </div>
                <div class="col-lg-3 col-md-3 col-sm-1 col-contact-details">
                    <div class="contact-content">
                        <div class="contact-favicon">
                            <i class="fa fa-map-marker fa-5x fa-class" aria-hidden="true"></i>
                        </div>
                        <h4 class="contact-header">Located</h4>
                        <span>
                            <a class="contact-link">Delhi, India</a>
                        </span>
                    </div>
                </div>
                <div class="border-col"></div>
            </div><div class="row hover-me-row">
                <div class="col-md-12 hover-me-col">
                    <div class="hover">
                        <span>Social Links</span>
                        <a class="social-link" href="https://www.linkedin.com/in/kritverma7" target="_blank"><i class="fa fa-linkedin" aria-hidden="true"></i></a>
                        <a class="social-link" href="https://github.com/Krit7" target="_blank"><i class="fa fa-github" aria-hidden="true"></i></a>
                        <a class="social-link" href="https://www.hackerrank.com/krit17348" target="_blank"><i class="fa fa-code" aria-hidden="true"></i></a>
                        <a class="social-link" href="https://www.instagram.com/kritvermax/" target="_blank"><i class="fa fa-instagram" aria-hidden="true"></i></a>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>


<script>
export default {
    
}
</script>

<style scoped>

.section-contact-me{
    padding-top: 0;
}
.parallax {
  background-image: url("../assets/img/contact-me-bg.jpg");
  height: 400px;
  background-attachment: fixed;
  background-repeat: no-repeat;
  background-size: cover;
  text-align: center;
}

.get-in-touch{
    padding-top: 72px;
    font-size: 75px;
    font-weight: bolder !important;
    color: white;
}

.get-in-touch-border {
  position: relative;
}

.get-in-touch-border::after {
  position: absolute;
  content: "";
  border-bottom: 2px solid white;
  bottom: 0;
  left: 20%;
  width: 75%;
  margin-bottom: -15%;
}
.contact-row{
    margin-top: 100px;
    /* background-color: #f7f7f7; */
}
.border-col{
    width: 12.66%;
}

.col-contact-details{
    height: 250px;
    background-color: white;
    /* border: 0.1px solid #e0dbdb47; */
    box-shadow: 1px 1px 5px 1px  #eaeaea;
}

.contact-content{
    margin: 15%;
}
.fa-class{
    color: #69c6da;
}
.contact-favicon{
    margin: 15px 0;
}

.contact-header{
    font-weight: 700;
    margin: 15px 0;
}

.contact-link{
    color: #68696a;
    text-decoration: none;
    margin: 15px 0;
}


.hover-me-row{
    margin-top: 5%;
}

.hover {
  position: relative;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 300px;
  height: 75px;
  background-color: #4DB6AC;
  border-radius: 99px;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12), 0 1px 2px rgba(0, 0, 0, 0.24);
  transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
  overflow: hidden;
}
.hover:before, .hover:after {
  position: absolute;
  top: 0;
  display: flex;
  align-items: center;
  width: 50%;
  height: 100%;
  transition: 0.25s linear;
  z-index: 1;
}
.hover:before {
  content: '';
  left: 0;
  justify-content: flex-end;
  background-color: #50b5ce;
}
.hover:after {
  content: '';
  right: 0;
  justify-content: flex-start;
  background-color: #50b5ce;
}
.hover:hover {
  background-color: #50b5ce;
  box-shadow: 0 14px 28px rgba(0, 0, 0, 0.25), 0 10px 10px rgba(0, 0, 0, 0.22);
}
.hover:hover span {
  opacity: 0;
  z-index: -3;
}
.hover:hover:before {
  opacity: 0.5;
  transform: translateY(-100%);
}
.hover:hover:after {
  opacity: 0.5;
  transform: translateY(100%);
}
.hover span {
  position: absolute;
  top: 0;
  left: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
  color: whitesmoke;
  font-family: 'Fira Mono', monospace;
  font-size: 24px;
  font-weight: 700;
  opacity: 1;
  transition: opacity 0.25s;
  z-index: 2;
}
.hover .social-link {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  width: 25%;
  height: 100%;
  color: whitesmoke;
  font-size: 24px;
  text-decoration: none;
  transition: 0.25s;
}
.hover .social-link i {
  text-shadow: 1px 1px rgba(70, 98, 127, 0.7);
  transform: scale(1);
}
.hover .social-link:hover {
  background-color: rgba(245, 245, 245, 0.1);
}
.hover .social-link:hover i {
  animation: bounce 0.4s linear;
}

@keyframes bounce {
  40% {
    transform: scale(1.4);
  }
  60% {
    transform: scale(0.8);
  }
  80% {
    transform: scale(1.2);
  }
  100% {
    transform: scale(1);
  }
}

</style>