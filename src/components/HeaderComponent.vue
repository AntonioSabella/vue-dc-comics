<template>
    <header id="site_header">
        <div class="container">
            <div class="logo_box">
                <img width="50" src="@/assets/img/dc-logo.png" alt="logo DC">
            </div>
            <div class="page_menu">
                <ul class="link_list">
                 <li class="list_item">
                     <a href="#">Characters</a>
                 </li>
                 <li class="list_item">
                     <a href="#">Comics</a>
                 </li>
                 <li class="list_item">
                     <a href="#">Movies</a>
                 </li>
                 <li class="list_item">
                     <a href="#">Tv</a>
                 </li>
                 <li class="list_item">
                     <a href="#">Games</a>
                 </li>
                 <li class="list_item">
                     <a href="#">Collectibles</a>
                 </li>
                 <li class="list_item">
                     <a href="#">Videos</a>
                 </li>
                 <li class="list_item">
                     <a href="#">Fans</a>
                 </li>
                 <li class="list_item">
                     <a href="#">News</a>
                 </li>
                 <li class="list_item">
                     <a href="#">Shop</a>
                 </li>
                </ul>
            </div>
        </div>
    </header>
</template>

<script>

</script>

<style lang="scss" scoped>
    header {
     background-color: white;
     width: 100%;
    }

    .container {
        display: flex;
        justify-content: space-around;
        align-items: flex-end;
        padding: 1rem 1rem 0 1rem;
    }

    .logo_box {
        padding-bottom: 0.5rem;
        
    }

    .link_list {
        display: flex;
        list-style: none;
        column-gap: 1rem;
        font-size: 12px;
        font-weight: 600;

    }

    .list_item:hover {
        border-bottom: 5px solid cornflowerblue;
    }

    .list_item:hover a {
        color: cornflowerblue;
    }

    .list_item {
        padding-bottom: 2rem;
        
    }
    .list_item>a {
        text-decoration: none;
        color: gray;
    }
</style>