<template>
    <div class="search-container">
        <input type="text" placeholder="Search or jump to.." class="search">
    </div>
</template>

<style scoped>

.search {
    border-radius: 5px;
    border: 1px solid #30363d;
    padding: 5px;
    width: 250px;
    -webkit-transition: all .5s ease;
    -moz-transition: all .5s ease;
    transition: all .5s ease;
    color: white;
    /* float: right; */
    background: #0d1117;
    /* border: #30363d; */
}
.search:focus {
    /* width: 210px; */
    outline: none;
    border: 3px solid #30363d;
}

.search::placeholder{
    color: white;
}


@media (min-width: 768px) {
    .search:focus{
        width: 300px;
    }
}

@media (min-width: 1024px) {

    .search:focus{
        width: 400px;   
    }
}
</style>