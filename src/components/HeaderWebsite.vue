<template>
  <header class="container-fluid">
    <img src="../assets/img_header.png" alt="code aplication ordinateur">
    <div class="menu">
        <input type="checkbox" id="toggle" />
        <label id="show-menu" for="toggle">
            <div class="btn">
            <i class="material-icons md-36 toggleBtn menuBtn">menu</i>
            <i class="material-icons md-36 toggleBtn closeBtn">close</i>
            </div>
            <div class="btn">
                <a class="text-decoration-none" href="#presentation">Présentation</a>
            </div>
            <div class="btn">
                <a class="text-decoration-none" href="#services">Services</a>
            </div>
            <div class="btn">
                <a class="text-decoration-none" href="#competences">Compétences</a>
            </div>
            <div class="btn">
                <a class="text-decoration-none" href="#contact">Portfolio</a>
            </div>
        </label>
    </div>
    <div id="header_presentation">
        <h1 class="h3 text-uppercase">Christophe Da Silva</h1>
        <h2 class="h1">DEVELOPPEMENT WEB FULL STACK</h2>
    </div>
  </header>
</template>

<script setup>

</script>

<style scoped>

header {
    width: 100%;  
}

img {
  width: 100%;
  height: 600px;
  object-fit: cover;
}

input {position: absolute; display: none}

* {
  -webkit-touch-callout: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.menu {
  margin: 0 auto;
  position: absolute;
  bottom: 52%;
  left: 30%;
  margin-left: -25px;
  margin-top: -25px;
  z-index: 1; 
}

.btn {
  width: 105px;
  height: 80px;
  border-radius: 100px;
  position: absolute;
  overflow: hidden;
  cursor: pointer;
}

.material-icons.md-36  { font-size: 36px; color: #03A9F4 }

.btn {
  background: #ECEFF1;
  font-size: 15px;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
      -ms-flex-pack: center;
          justify-content: center;
  -webkit-box-align: center;
      -ms-flex-align: center;
          align-items: center;
  box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
  
  -webkit-transition: all 0.3s cubic-bezier(.25,.8,.25,1);
  transition: all 0.3s cubic-bezier(.25,.8,.25,1);
}

.btn:not(:first-child) {
  opacity: 0;
  -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=0)";
  z-index: -2;
  
  -webkit-transition: all 0.6s cubic-bezier(.87,-.41,.19,1.44);
  transition: all 0.6s cubic-bezier(.87,-.41,.19,1.44);
}

.btn:nth-child(2) {top:0px;-webkit-transition-delay: 0s;transition-delay: 0s}
.btn:nth-child(3) {top:0px;left:0px;-webkit-transition-delay: 0.1s;transition-delay: 0.1s}
.btn:nth-child(4) {left:0px;;-webkit-transition-delay: 0.2s;;transition-delay: 0.2s}
.btn:nth-child(5) {top:0px;left:0px;-webkit-transition-delay: 0.3s;transition-delay: 0.3s}


input#toggle:checked ~ #show-menu .btn:nth-child(2) {
  top:-150px;opacity:1;-ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
}
input#toggle:checked ~ #show-menu .btn:nth-child(3) {
  left:150px;opacity:1;-ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
}
input#toggle:checked ~ #show-menu .btn:nth-child(4) {
  top:150px;opacity:1;-ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
}
input#toggle:checked ~ #show-menu .btn:nth-child(5) {
  left:-150px;opacity:1;-ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
}

a  { color: #03A9F4 }

a, .green {
    background-color: #ECEFF1;;
}

.menuBtn, .closeBtn {
  position: absolute;
  transition: all 0.3s ease;
}

.closeBtn {
  transform: translateY(50px);
  opacity: 0;
}

input#toggle:checked ~ #show-menu .btn .menuBtn {
  transform: translateY(-50px);
  opacity: 0;
}

input#toggle:checked ~ #show-menu .btn .closeBtn {
  transform: translateY(0px);
  opacity: 1;
}

#header_presentation {
  font-family:  Helvetica, Arial, sans-serif;
  margin: auto;
  margin-top: 30px;
  position: absolute;
  top: 0%;
  left: 9%;
  text-align: center;
  color: black; 
}

h2 {
  border-bottom: 3px solid black;
}

</style>
