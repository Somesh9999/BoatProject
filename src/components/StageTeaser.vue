<template>
    <section class="stage-teaser">
        <div class="cover1"></div>
        <div class="cover2"></div>
        <div class="teaser-content">
            <div class="teaser-heading">Some Title goes here</div>
            <div class="teaser-description">Some Description goes here</div>
        </div>
        <!-- <div class="stage-buttons">
            <div class="stage-button-item" @click="paginationClicked">Add a Listing</div>
            <div class="stage-button-item">Login to Website</div>
        </div> -->
    </section>
</template>

<script>
export default {
    name: "StageTeaserComp"
}
</script>

<style>
.stage-teaser {
    height: 600px;
    width: 100%;
    margin: 0 0 6% 0;
    position: relative;
}

.cover1 {
    width: 100%;
    height: 100%;
    background-image: url("../assets/stage-teaser2.jpg");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    z-index: 2;
    position: absolute;
}

.cover2 {
    width: 100%;
    height: 100%;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    z-index: 2;
    background-image: linear-gradient(174deg, #1d3550, transparent);
    position: absolute;
}

.teaser-content {
    position: absolute;
    top: 40%;
    width: 100%;
    display: flex;
    flex-direction: column;
    gap: 10px;
    color: white;
    z-index: 6;
    font-family: 'Poppins', sans-serif;
    text-align: center;
}

.teaser-heading {
    font-size: 300%;
}

.teaser-description {
    font-size: 160%;
}

@media (max-width: 600px) {
    .stage-teaser {
        height: 460px;
    }
}
</style>