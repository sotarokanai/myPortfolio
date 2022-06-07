<template>
   <div class="main">
        <div class="inner"> 
            <commonHeader></commonHeader>
            <Nuxt />
        </div>
  </div>
</template>

<style lang="scss">
.main {
  width: 100%;
  overflow: hidden;
  padding: 68px 0; 
    
}

@include mobile {
  .main {
    padding: v(52) 0;
  }
}
</style>