<template>
    <div class="article">
        <div class="content-area">
            <articleTtl
            :linkPath='`article/01`'
            >あとで何かけるかな</articleTtl>
            <articleTtl
            :linkPath='`article/02`'
            >あとで何かけるかな</articleTtl>
        </div>
    </div>
    
</template>

<style lang="scss">
.article {
    width: 100%;
    overflow: hidden;
    .content-area {
        padding-top: 38px;
        width: 1144px;
        margin: 0 auto;
    }
}

@include mobile {
    .article {
        .content-area {
            width: v(680);
            padding-top: v(38);
        }
    }
}
</style>