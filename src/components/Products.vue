<template>
    <section class="products">
        <div class="heading">
            Products
        </div>
        <ProductFilterComp></ProductFilterComp>
        <!-- <div class="product-list">
            <div class="product-item">
                <div class="product-image"><img src="../assets/boatimg1.png" alt=""></div>
                <div class="product-title">London Smart Cruise</div>
                <div class="product-price">Rs 5,000 /day</div>
                <div class="product-redirect-icon"><img src="../assets/product-arrow.png" alt=""></div>
            </div>
            <div class="product-item">
                <div class="product-image"><img src="../assets/boatimg2.png" alt=""></div>
                <div class="product-title">London Smart Cruise</div>
                <div class="product-price">Rs 5,000 /day</div>
                <div class="product-redirect-icon"><img src="../assets/product-arrow.png" alt=""></div>
            </div>
            <div class="product-item">
                <div class="product-image"><img src="../assets/boatimg3.png" alt=""></div>
                <div class="product-title">London Smart Cruise</div>
                <div class="product-price">Rs 5,000 /day</div>
                <div class="product-redirect-icon"><img src="../assets/product-arrow.png" alt=""></div>
            </div>
        </div> -->
        <div class="product-list">
            <div class="product-item" id="product-item" v-for="product in this.products" v-bind:key="product.id">
                <div class="product-image"><img :src=product.imageURL alt=""></div>
                <div class="product-title">{{ product.title }}</div>
                <div class="product-price">{{ product.price }}</div>
                <div class="product-redirect-icon"><img src="../assets/product-arrow.png" alt=""></div>
            </div>
        </div>
        <b-pagination @change="paginationClicked" v-model="currentPage" :total-rows="rows" :per-page="perPage" pills align="center" aria-controls="product-item">
        </b-pagination>
    </section>
</template>

<script>
import ProductFilterComp from '@/components/ProductFilter.vue'
export default {
    name: "ProductListComp",
    components: { ProductFilterComp },
    data() {
        return {
            perPage: 3,
            currentPage: 1,
            products: [
                {
                    id:"1",
                    title: "London Smart Cruise",
                    price: "Rs 5,000 /day",
                    imageURL: "http://localhost:8080/img/boatimg1.11313d2e.png"
                },
                {
                    id:"2",
                    title: "London Smart Cruise",
                    price: "Rs 5,000 /day",
                    imageURL: "http://localhost:8080/img/boatimg2.de4dd83f.png"
                },
                {
                    id:"3",
                    title: "London Smart Cruise",
                    price: "Rs 5,000 /day",
                    imageURL: "http://localhost:8080/img/boatimg3.1dbc93eb.png"
                },
                {
                    id:"4",
                    title: "London Smart Cruise",
                    price: "Rs 5,000 /day",
                    imageURL: "http://localhost:8080/img/boatimg1.11313d2e.png"
                },
                {
                    id:"5",
                    title: "London Smart Cruise",
                    price: "Rs 5,000 /day",
                    imageURL: "http://localhost:8080/img/boatimg2.de4dd83f.png"
                },
                {
                    id:"6",
                    title: "London Smart Cruise",
                    price: "Rs 5,000 /day",
                    imageURL: "http://localhost:8080/img/boatimg3.1dbc93eb.png"
                },
            ]
        }
    },
    methods:{
        paginationClicked(){
            console.log("page changed")
        }
    },
    computed: {
      rows() {
        return this.products.length
      }
    }
    
}
</script>

<style>
.products {
    width: 100%;
}

.products .heading {
    width: 100%;
    text-align: center;
    font-size: 200%;
    font-family: 'Poppins', sans-serif;
    color: #1d3550;
    /* color: #1A2980; */
    margin: 4% 0;
    text-decoration: underline;
}

.products .product-list {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    justify-content: center;
    width: 90%;
    margin: 4% auto;
}

.product-item {
    display: flex;
    flex-direction: column;
    width: 80%;
    height: 400px;
    border-radius: 20px;
    /* background-color: #1d3550; */
    justify-self: center;
    align-items: center;
    gap: 1%;
    margin: 5% 0;
    box-shadow: inset 0 0 0 1px rgb(177 177 180 / 30%);
    overflow: hidden;
}

.product-item .product-image {
    width: 100%;
    height: 65%;
    overflow: hidden;
}

.product-item .product-image img {
    width: 100%;
    transition: 0.3s ease-in-out;
}

.product-item .product-image img:hover {
    width: 100%;
    transform: scale(1.1);
    cursor: pointer;
}

.product-item .product-title,
.product-item .product-price {
    width: 100%;
    text-align: center;
    font-size: 130%;
    font-weight: 600;
    font-family: 'Zilla Slab', serif;
    ;
    /* color: #26D0CE; */
    color: black;
    transition: 0.3s ease-in-out;
}

.product-item .product-title:hover {
    color: #476986;
    cursor: pointer;
}

.product-item .product-redirect-icon {
    padding: 2%;
}

.product-item .product-redirect-icon img {
    width: 70%;
    transition: 0.3s ease-in-out;
}

.product-item .product-redirect-icon img:hover {
    transform: translateX(85%);
    cursor: pointer;
}

</style>