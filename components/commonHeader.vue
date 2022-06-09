<template>
    <div class="header">
        <div class="inner">
            <div class="container"> 
                <h1><a @click="$router.push('/')">SOTARO KANAI</a></h1>
                <p><a @click="$router.push('/info')">profile</a>
                <a href="https://www.instagram.com/sotarokanai/" target="_blank">Instagram</a></p>
                <img src="~/assets/img/other/header_bottom.png" alt="">
            </div>         
        </div>
    </div>
</template>

<script>
export default {
    mounted() {
        
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
        img {
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
