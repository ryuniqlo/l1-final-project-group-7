<script setup>
import SearchBar from '../components/SearchBar.vue'
import Listing from '../components/Listing.vue'
import AddListing from '../components/AddListing.vue'
</script>

<template>
  <main>
    <SearchBar /> <br><br>

    <h1 class= "listings"> My Listings</h1> <br><br><br>

    <div class = "container">
    <div class = "listing">
    <Listing />
  </div>
  <div class = "addlisting">
    <AddListing />
  </div>
</div>
  </main>
</template>

<style scoped>
.container {
  display: flex;
  justify-content: space-between;
}

.listing{
  flex-basis: 60%;
}

.addlisting {
  flex-basis: 40%;
  margin-left: 300px;
}
.listings{
  padding-left:300px;
  color : white
}

</style>