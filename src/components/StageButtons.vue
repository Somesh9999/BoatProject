<template>
    <section class="stage-buttons">
        <div class="stage-button-item" @click="paginationClicked">Add a Listing</div>
        <div class="stage-button-item">Login to Website</div>
    </section>
</template>

<script>
export default {
name:"StageButtonComp"
}
</script>

<style>
.stage-buttons {
    display: flex;
    gap: 50px;
    top: 108%;
    width: 100%;
    justify-content: center;
    font-family: 'Poppins', sans-serif;
    font-size: 100%;
    font-weight: 500;
    text-align: center;
}

.stage-button-item {
    background: transparent;
    color: #1d3550;
    border-radius: 10px;
    border: 2px solid #1d3550;
    padding: 2%;
    width: 22%;
    justify-self: center;
}

.stage-button-item:hover {
    cursor: pointer;
    background-color: #1d3550;
    color: white;
    transition: 0.4s;
}
</style>