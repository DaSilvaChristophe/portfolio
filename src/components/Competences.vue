<template>
    <section id="competences" class="container mb-5">
        <div class="mx-auto ligne my-5"></div>
        <h1 class="text-center w-100">COMPETENCES</h1>
        <div class='animation-example'>
            <div class='item'>
                <div class='line'></div>
                <div class='dot'></div>
                <div class='circle text-center'>
                    <ul class="list-unstyled">
                    <p class="text-uppercase fw-bold mb-2">Langages & Frameworks</p>
                    <li class="text-uppercase">Javascript</li>
                    <li class="text-uppercase">Vue.js v2 & v3</li>
                    <li class="text-uppercase">Bootstrap v4 & v5</li>
                    <li>HTML5</li>
                    <li>CSS3/SCSS</li>
                    </ul>
                </div>
            </div>
            <div class='item'>
                <div class='line'></div>
                <div class='dot'></div>
                <div class='circle text-center'>
                    <ul class="list-unstyled">
                    <p class="text-uppercase fw-bold mb-2">Backend & Databases</p>
                    <li class="text-uppercase">Node.js</li>
                    <li class="text-uppercase">Express & Nest.js</li>
                    <li class="text-uppercase">MySQL</li>
                    <li class="text-uppercase">MongoDB</li> 
                    </ul>
                </div>
            </div>
            
            <div class='item'>
                <div class='line'></div>
                <div class='dot'></div>
                <div class='circle text-center'>
                    <ul class="list-unstyled">
                    <p class="text-uppercase fw-bold mb-2">Others</p>
                    <li class="text-uppercase">Audit & Optimisation SEO</li>
                    <li class="text-uppercase">Adobe XD & Acrobat Pro</li>
                    <li class="text-uppercase">Merise</li>
                    <li class="text-uppercase">Méthodologie BEM</li>
                    <li class="text-uppercase">CMS (Wix & Shopify E-commerce)</li>
                    <li class="text-uppercase">Google Analytics / Business</li>
                    <li class="text-uppercase">Accessibilité</li>  
                    </ul>
                </div>
            </div>
            <div class='item -type2'>
                <div class='line'></div>
                <div class='dot'></div>
                <div class='circle'>
                    <p class="text-uppercase fw-bold pt-4 ps-4">API REST</p>
                </div>
            </div>
            <div class='item -type2'>
                <div class='circle text-center'>
                    <ul class="list-unstyled">
                    <p class="text-uppercase fw-bold mb-2">Version Control</p>
                    <li class="text-uppercase">Git</li>
                    <li class="text-uppercase">Git Hub</li>
                    </ul>
                </div>
            </div>
            <div class='center'>
                <div class='circle'></div>
                <div class='circle'></div>
                <div class='circle'></div>
            </div>
        </div>
    </section>
</template>
  
<script> 

  export default {
    name: 'Competences',
  }
  
</script>
  
<style lang="scss" scoped>

.ligne {
  width: 100%;
  margin-right: 5%;
  height: 1px;
  background-color: #999999;
  opacity: 1;
}

h1 {
	font-family:  Helvetica, Arial, sans-serif;
}

.animation-example {
    position: relative;
    top: 50%;
    left: 50%;
    transform: translateX(-50%) translateY(-50%);
    height: 90vmin;
    width: 90vmin;
    
    > .item {
        position: absolute;
        top: 0%;
        left: 50%;
        height: 50%;
        width: 50%;
        transform: translateX(-50%);
        transform-origin: 50% 100%;
        pointer-events: none;
    }
    
    > .item:nth-child(2) {
        transform: translateX(-148%) translateY(91%) ;
    }
    
    > .item:nth-child(3) {
        transform: translateX(50%) translateY(90%);
    }
    
    > .item > .line {
        height: 100%;
        width: "calc(50% + 1px)";
        border-right: 2px dashed #5bc0eb;
    }
    
    > .item > .dot {
        position: absolute;
        left: 50%;
        top: 10%;
        transform: translateX(-50%) translateY(-50%);
        height: 100%;
        width: 100%;
        animation: move-dot1 5.5s linear infinite;
    }
    
    > .item > .dot::after {
        content: '';
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translateX(-50%) translateY(-50%);
        height: 5%;
        width: 5%;
        background: #fff;
        border: 2px solid #5bc0eb;
        border-radius: 50%;
    }

    > .item > .circle {
        position: absolute;
        top: -5%;
        left: 50%;
        transform: translateX(-50%);
        height: 40%;
        width: 100%;
        border-radius: 10%;
        background: transparent;
    }
    
    > .item.-type2 {
        top: 0;
        left: 0%;
        transform: none;
        transform-origin: 100% 100%;
    }

    > .item.-type2:nth-child(5) {
        transform: scaleX(100%) translateX(160%) translateY(20%) ;
    }
    
    > .item.-type2 > .line {
        position: absolute;
        top: 30%;
        left: "calc(30% - 1px)";
        width: 70%;
        height: 40%;
        border-right: none;
        border-left: 2px dashed #5bc0eb;
        border-bottom: 2px dashed #5bc0eb;
    }
    
    > .item.-type2 > .dot {
        top: 30%;
        left: 30%;
        animation: move-dot2 4s linear infinite;
    }
    
    > .item.-type2 > .circle {
        top: 30%;
        left: 30%;
        transform: translateX(-50%) translateY(-50%);
    }
    
    > .item:nth-of-type(1) > .dot {
        animation-delay: 0;
    }
    
    > .item:nth-of-type(7) > .dot {
        animation-delay: .5s;
    }
    
    > .item:nth-of-type(2) > .dot {
        animation-delay: 1s;
    }
    
    > .item:nth-of-type(6) > .dot {
        animation-delay: 1.5s;
    }
    
    > .item:nth-of-type(3) > .dot {
        animation-delay: 2s;
    }
    
    > .item:nth-of-type(5) > .dot {
        animation-delay: 2.5s;
    }
    
    > .item:nth-of-type(4) > .dot {
        animation-delay: 3s;
    }
    
    > .item:nth-of-type(8) > .dot {
        animation-delay: 3.5s;
    }
    
    > .center {
        position: absolute;
        top: 54%;
        left: 50%;
        transform: translateX(-50%) translateY(-50%);
        height: 50%;
        width: 50%;
    }
    
    > .center > .circle {
        position: absolute;
        top: 41.5%;
        left: 50%;
        transform: translateX(-50%) translateY(-50%);
        border-radius: 50%;
    }
    
    > .center > .circle:nth-child(1) {
        height: 100%;
        width: 100%;
        background: #fff;
        box-shadow: 0 0 3vmin rgba(0, 0, 0, .1);
    }
    
    > .center > .circle:nth-child(2) {
        height: 80%;
        width: 80%;
        border: 2px solid #5bc0eb;
    }
    
    > .center > .circle:nth-child(3) {
        height: 50%;
        width: 50%;
        background: #5bc0eb;
    }
}

@keyframes move-dot1 {
    0% {
        transform: translateX(-50%) translateY(-50%);
    }
    
    20% {
        transform: translateX(-50%) translateY(30%);
    }
    
    100% { 
        transform: translateX(-50%) translateY(30%);
    }
}


@keyframes move-dot2 {
    0% {
        transform: translateX(-50%) translateY(-50%);
    }
    
    15% {
        transform: translateX(-50%) translateY(-10%);
    }
    
    30% {
        transform: translateX(-10%) translateY(-10%);
    }
    
    100% { 
        transform: translateX(-10%) translateY(-10%);
    }
}

</style>