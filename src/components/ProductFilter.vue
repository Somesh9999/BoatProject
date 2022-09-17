<template>
  <section class="product-filter">
    <img src="../assets/filter.png" alt="">
    <div class="filter-item-list">
      <div class="filter-item">
        Price
        <input type="range" class="price-range">
      </div>
      <div class="filter-item">
        Owner
        <b-dropdown id="dropdown-1" text="Select" class="m-md-2">
          <b-dropdown-item>First Action</b-dropdown-item>
          <b-dropdown-item>Second Action</b-dropdown-item>
          <b-dropdown-item>Third Action</b-dropdown-item>
          <b-dropdown-divider></b-dropdown-divider>
          <b-dropdown-item active>Active action</b-dropdown-item>
          <b-dropdown-item disabled>Disabled action</b-dropdown-item>
        </b-dropdown>
      </div>
      <div class="filter-item">
        Location
        <b-dropdown id="dropdown-2" text="Select" class="m-md-2">
          <b-dropdown-item>First Action</b-dropdown-item>
          <b-dropdown-item>Second Action</b-dropdown-item>
          <b-dropdown-item>Third Action</b-dropdown-item>
          <b-dropdown-divider></b-dropdown-divider>
          <b-dropdown-item active>Active action</b-dropdown-item>
          <b-dropdown-item disabled>Disabled action</b-dropdown-item>
        </b-dropdown>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ProductFilterComp"
}
</script>

<style>
.product-filter {
  width: 80%;
  height: 80px;
  display: flex;
  justify-content: left;
  gap: 20%;
  align-items: center;
  margin: 3% auto;
  box-shadow: inset 0 0 0 1px rgb(177 177 180 / 30%);
  border-radius: 20px;
  font-size: 100%;
  font-family: 'Poppins', sans-serif;
}

.product-filter img {
  width: 4%;
  justify-self: start;
  margin-left: 2%;
}

.filter-item-list {
  display: flex;
  gap: 5%;
  align-items: center;
  justify-content: center;
}

.filter-item {
  display: flex;
  flex-direction: row;
  gap: 5%;
  align-items: center;
}

.filter-item .price-range {

  accent-color: #1d3550;
}

.filter-item .btn {
  background-color: #1d3550;
  color: white;
  transition: 0.3s ease-in-out;
}

.filter-item .btn:hover {
  background-color: #476986;
}


@media (max-width: 600px) {
  .product-filter {
    height: 170px;
  }

  .filter-item-list {
    display: flex;
    flex-direction: column;
    gap: 15px;
    align-items: start;
    justify-content: start;
  }
}

/* @media only screen and (min-width: 320px) and (max-width: 425px) {
  .product-filter {
    height: 170px;
  }

  .filter-item-list {
    display: flex;
    flex-direction: column;
    gap: 15px;
    align-items: start;
    justify-content: start;
  }
} */
</style>