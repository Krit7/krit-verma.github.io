<template>
  <div>
    <section class="navpanel">
      <div class="container-fluid">
        <nav class="navbar navbar-expand-lg navbar-light fixed-top">
          <a class="navbar-brand" href="#section1">Krit Verma</a>
          <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="nav navbar-nav ml-auto">
              <li class="nav-item active">
                <a class="nav-link" href="#section1">
                  Home
                  <span class="sr-only">(current)</span>
                </a>
              </li>
              <li class="nav-item non-active">
                <a class="nav-link" href="#section2">About Me</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#section3">My Work</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" target="_blank" href="https://drive.google.com/file/d/19gBlKP1L52vTQf1hHUSjQLr3DWz2iDnc/view?usp=sharing">Resume</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#section4">Contact</a>
              </li>
            </ul>
          </div>
        </nav>
      </div>
    </section>
  </div>
</template>

<script>
$(window).scroll(function(){
	$('nav').toggleClass('scrolled', $(this).scrollTop() > 25);
});
export default {
  
};
</script>

<style scoped>
.container-fluid{
  padding: 0 !important;
}
.navbar{
  padding: 1rem 2rem .5rem 2rem;
  height: 75px;
  box-shadow: 0px 1px 5px 1px #e0dbdb47;
}
.navpanel{
  position: relative;
  z-index: 999;
}
.navbar-light .navbar-brand{
  padding-left: 40px;
  font-size: 26px;
  position: relative;
  top:-5px;
}
.nav-item{
  padding: 0 10px 10px 10px;
}

.scrolled{
  background:#fff;
  height: 65px;
}
</style>