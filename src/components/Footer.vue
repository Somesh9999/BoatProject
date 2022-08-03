<template>
  <section class="footer">

    <div class="footer-item-list">
        <div class="footer-item"><img src="../assets/facebook-brands.svg" alt="" width="100%" ></div>
        <div class="footer-item"><img src="../assets/linkedin-brands.svg" alt="" width="100%" ></div>
        <div class="footer-item"><img src="../assets/instagram-brands.svg" alt="" width="100%"></div>
        <div class="footer-item"><img src="../assets/twitter-brands.svg" alt="" width="100%"></div>
    </div>
    <div class="footer-copyright">© 2022 Copyright: ABC.com</div>
  </section>
</template>

<script>
export default {
name:"FooterComp"
}
</script>

<style>
.footer{
    display: flex;
    align-items: center;
    height: 150px;
    background-image: linear-gradient(174deg, #1d3550, transparent);
    background-color: black;
    color: white;
    padding: 0 8%;
    margin: 2% 0 0 0;
}
.footer-item-list{
    display: flex;
    justify-content: start;
    gap: 3%;
}
.footer-item{
    width: 3%;
}

.footer-item img{
    filter: invert(100%) sepia(0%) saturate(0%) hue-rotate(16deg) brightness(104%) contrast(102%);
}

.footer-copyright{
    font-size: 100%;
    font-family: 'Poppins', sans-serif;
    width: 30%;
    text-align: right;
}
</style>