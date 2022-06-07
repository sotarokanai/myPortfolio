<template>
    <div class="topimg">
    </div>
</template>

<style lang="scss">
    .topimg {
        background: url("~/assets/img/1.jpg") center top no-repeat;
        height: 500px;
        width: 100vw;
        background-size: cover;
    }

    @include mobile {
        .topimg {
            height: 50vw;
            width: 100vw;
        }
    }

</style>