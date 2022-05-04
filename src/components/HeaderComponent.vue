<template>
    <header id="site_header">
        <div class="container">
            <div class="logo_box">
                <img width="50" src="@/assets/img/dc-logo.png" alt="logo DC">
            </div>
            <div class="page_menu">
                <ul class="link_list">
                 <li class="list_item" v-for="(section, index) in navSections" :key="index">
                     <a href="#">{{section.nome}}</a>
                 </li>
                
                </ul>
            </div>
        </div>
    </header>
</template>

<script>
    export default {
        name: 'HeaderComponent',
        data () {
            return {
                navSections: [
                    {
                        nome: "Characters",
                    },
                    {
                        nome: "Comics",
                    },
                    {
                        nome: "Movies",
                    },
                    {
                        nome: "Tv",
                    },
                    {
                        nome: "Games",
                    },
                    {
                        nome: "Collectibles",
                    },
                    {
                        nome: "Videos",
                    },
                    {
                        nome: "Fans",
                    },
                    {
                        nome: "News",
                    },
                    {
                        nome: "Shop",
                    },
                ]
            }
        }
    }
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
       border-bottom: 5px solid rgb(58, 116, 223);
    }

    .list_item:hover a {
        color: rgb(58, 116, 223);
    }

    .list_item {
        padding-bottom: 2rem;
        border-bottom: 5px solid transparent; 
    }
    .list_item>a {
        text-decoration: none;
        color: gray;
    }
</style>