<template>
    <section class="main-header">
        <div class="logo"><img src="../assets/logo.png" alt=""></div>
        <!-- <ul>
                <li>Home</li>
                <li>Contact</li>
                <li>About us</li>
            </ul> -->
        <nav class="header-items">
            <router-link class="header-item" to="/">Home</router-link> |
            <router-link class="header-item" to="/about">About</router-link> |
            <router-link class="header-item" to="/about">Services</router-link> |
            <router-link class="header-item" to="/about">Products</router-link> |
            <router-link class="header-item" to="/about">Contact</router-link>
        </nav>
    </section>
</template>

<script>
export default {
    name: "HeaderComp"
}
</script>

<style>
.main-header {
    position: absolute;
    display: grid;
    grid-template-columns: 0.5fr 1fr;
    align-items: start;
    width: 100%;
    background: transparent;
    z-index: 3;
    color: white;
}

.logo {
    width: 30%;
    justify-self: center;
}

.logo img {
    width: 100%;
    height: 100%;
}

.header-items {
    justify-self: center;
    display: flex;
    gap: 20px;
    align-items: center;
}

.header-item::after {
    display: block;
    content: "";
    border-bottom: 3px solid #8be2f3;
    transform: scaleX(0);
    transition: transform 250ms ease-in-out;
}

.header-item:hover::after {
    border-bottom: 3px solid #8be2f3;
    cursor: pointer;
    transform: scale(1);
}

@media (max-width: 600px) {
    .header-items {
        display: none;
    }

    .logo {
        width: 60%;
    }
}
</style>