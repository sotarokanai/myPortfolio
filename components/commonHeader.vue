<template>
    <div class="header">
        <div class="inner">
            <div class="container"> 
                <h1><a href="#">kazumakanai.com</a></h1>
                <p><a href="#">info</a></p>
            </div>         
        </div>
    </div>
</template>

<style lang="scss">
.header {
    color: $black;
    border-bottom: solid $black 2px;
    padding: 30px 0 16px;   
  .inner {
      width: 100vw;
      margin: 0 auto;      
      .container {
          display: flex;
          justify-content: space-between;
          align-items: flex-end;
          padding: 0 25px;
        h1 {
            font-size: 28px;
            display: inline-block;
        }
        p {
            font-size: 16px;
        }
      }
  } 
  a:hover {
    background: $black;
    color: rgb(87, 87, 87);
  }
}

@include mobile {
    .header {
        padding: v(40) 0 v(15);
        border-bottom: solid $black v(2);
        .container {
            padding: 0 v(10) !important;  
            h1 {
                font-size: v(50) !important;
            } 
            p {
            font-size: v(30) !important;
            }
        }
    } 
}

</style>