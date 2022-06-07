<template>
    <div class="paragraph">
        <p><slot>inu</slot></p>
    </div>
</template>

<style lang="scss">
    .paragraph {
        margin-bottom: 34px;
        p {
            font-size: 14px;
            color:  $black;
        }
        a {
            color: $blue;
        }
    }

    @include mobile {
        .paragraph {
            margin-bottom: v(34);
            p {
                font-size: v(20);
                color:  $black;
            }
        }
    }
</style>