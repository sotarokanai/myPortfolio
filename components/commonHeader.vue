<template>
    <div class="header">
        <div class="inner">
            <div class="container"> 
                <h1><a @click="$router.push('/')">YYG NT Lab</a></h1>
                <p>Basesd in Gunma.<br>YYG NT Lab is developing a<br>visual expression.  <a @click="$router.push('/info')">info</a> <a @click="$router.push('/article')">article</a> <a href="https://twitter.com/YYG_NT_LAB" target="_blank">Twitter</a></p>
                <!-- <img src="~/assets/img/header_bottom.png" alt=""> -->
                <div id="p5Canvas"></div>
            </div>         
        </div>
    </div>
</template>

<script>
export default {
    mounted() {
        const script = function (p5) {
            let xPos, colSet;
            let r = 0;
            let g = 1;
            let y = 2;
            p5.setup = _ => {

                if(window.innerWidth > 750) {
                    var canvas = p5.createCanvas(1144, 66)
                    canvas.parent("p5Canvas");
                } else if (window.innerWidth < 750) {
                    var canvas = p5.createCanvas(680/750*window.innerWidth, 45/750*window.innerWidth)
                    canvas.parent("p5Canvas");
                }
                
                p5.background(255);
        
                p5.stroke(0);
                for (let i = 0; i < 200; i++) {
                    xPos = p5.random(p5.windowWidth);
                    p5.line(xPos, 0, xPos, p5.windowHeight);
                }
            }

            p5.mousePressed = _ => {
                colSet = p5.int(p5.random(0,3));
                p5.background(255);
                p5.stroke(0);
                for (let i = 0; i < 200; i++) {
                    xPos = p5.random(p5.windowWidth);
                    p5.line(xPos, 0, xPos, p5.windowHeight);
                }
            }

            p5.windowResized = _ => {
                if(window.innerWidth > 750) {
                    var canvas = p5.createCanvas(1144, 66)
                    canvas.parent("p5Canvas");
                } else if (window.innerWidth < 750) {
                    var canvas = p5.createCanvas(680/750*window.innerWidth, 45/750*window.innerWidth)
                    canvas.parent("p5Canvas");
                }
                // if(colSet == r ){
                //     p5.background(255, 61, 90);
                // } else if(colSet == g) {
                //     p5.background(99, 212, 30);
                // } else if(colSet == y) {
                //     p5.background(255, 233, 36);
                // }
                p5.background(255);
        
                p5.stroke(0);
                for (let i = 0; i < 200; i++) {
                    xPos = p5.random(p5.windowWidth);
                    p5.line(xPos, 0, xPos, p5.windowHeight);
                }
            }
    }

    const P5 = require('p5')
    new P5(script)
    }
}
</script>




<style lang="scss">
.header {
    .inner {
        width: 1144px;
        margin: 0 auto;
        h1 {
            font-size: 24px;
            margin-bottom: 18px;
            font-weight: bold;
            a {
                text-decoration: none;
            }
        }
        p {
            font-size: 13px;
            a {
                color: $blue;
            }
        }
        #p5Canvas {
            margin: 26px 0;
        }
    }    
}

@include mobile {
    .header {
        .inner {
            width: v(680);
            h1 {
                font-size: v(36);
                margin-bottom: v(13);
            }
            p {
                font-size: v(20);
                a {
                    color: $blue;
                }
            }
            #p5Canvas {
                height: v(45);
                width: v(680);
                margin: v(35) 0;
            }
        }
    }   
}

</style>
