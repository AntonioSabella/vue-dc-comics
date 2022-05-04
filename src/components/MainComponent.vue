<template>
    <main id="site_main">
        <div class="container_top">
            <div class="current_series">
                <p>Current Series</p>
            </div>
        </div>
        <div class="container_mid">
            <div class="inside_container">
           <ComicComponent :comic="comic" v-for="comic in comics" :key="comic.series"/>
                 
             </div>
             <div class="load_more">
                 <p>Load More</p>
             </div>
        </div>
    
        <div class="container_bottom">
            <div class="dc_actions">
                <div class="dc_action" v-for="action in dcActions" :key="action.id">
                    <img :src="action.image" :alt="action.feature">
                    <p>{{action.feature}}</p>
                </div>
               
            </div>
        </div>
    </main>
</template>

<script>
import ComicComponent from "@/components/ComicComponent.vue";
     export default {
        name: 'MainComponent',
        data () {
            return {
                dcActions: [
                    {
                       id: 1,
                       feature: "Digital Comics",
                       image: require("../assets/img/buy-comics-digital-comics.png"),
                    },
                    {
                        id: 2,
                        feature: "DC Merchandise",
                        image: require("../assets/img/buy-comics-merchandise.png"),
                    },
                    {
                        id: 3,
                        feature: "Subscription",
                        image: require("../assets/img/buy-comics-subscriptions.png"),
                    },
                    {
                        id: 4,
                        feature: "Comic Shop Locator",
                        image: require("../assets/img/buy-comics-shop-locator.png"),
                    },
                    {
                        id: 5,
                        feature: "DC Power Visa",
                        image: require("../assets/img/buy-dc-power-visa.svg"),
                    },
                ],
                comics: [
                        {
                            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                            "price": "$19.99",
                            "series": "Action Comics",
                            "type": "comic book"
                        },
                        {
                            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                            "price": "$3.99",
                            "series": "American Vampire 1976",
                            "type": "comic book"
                        },
                        {
                            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                            "price": "$16.99",
                            "series": "Aquaman",
                            "type": "graphic novel"
                        },
                        {
                            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                            "price": "$2.99",
                            "series": "Batgirl",
                            "type": "comic book"
                        },
                        {
                            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                            "price": "$3.99",
                            "series": "Batman",
                            "type": "comic book"
                        },
                        {
                            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                            "price": "$2.99",
                            "series": "Batman Beyond",
                            "type": "comic book"
                        },
                        {
                            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                            "price": "$3.99",
                            "series": "Batman/Superman",
                            "type": "comic book"
                        },
                        {
                            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                            "price": "$4.99",
                            "series": "Batman/Superman Annual",
                            "type": "comic book"
                        },
                        {
                            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                            "price": "$5.99",
                            "series": "Batman: The Joker War Zone",
                            "type": "comic book"
                        },
                        {
                            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                            "price": "$6.99",
                            "series": "Batman: Three Jokers",
                            "type": "comic book"
                        },
                        {
                            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                            "price": "$4.99",
                            "series": "Batman: White Knight Presents: Harley Quinn",
                            "type": "comic book"
                        },
                        {
                            "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                            "price": "$16.99",
                            "series": "Catwoman",
                            "type": "graphic novel"
                        }
                ]
            }
        },
        components: {
            ComicComponent,
        },
    }
</script>

<style lang="scss" scoped>
    main {
     width: 100%;
    }

    .container_top {
        height: 400px;
        background-image: url("@/assets/img/jumbotron.jpg");
        background-size: cover;
        background-repeat: no-repeat;
        padding: 3rem 10rem;
        position: relative;
        .current_series {
            background-color: rgb(58, 116, 223);
            width: 150px;
            height: 50px;
            position: absolute;
            bottom: -1.2rem;
            left: 12rem;
            text-align: center;
            padding: 0.6rem 1rem;
            p {
                color: white;
                font-size: 14px;
                font-weight: 600;
                text-transform: uppercase;
            }
        }
    }

    .container_mid {
        background-color: black ;
        height: 600px;        
        padding: 4rem;
        position: relative;
        z-index: -1;
        .inside_container {
            display: flex;
            flex-wrap: wrap;
            column-gap: 1rem;
            row-gap: 2rem;
            width: 80%;
            margin: auto;
            .col-2{
                width: 15%;
                .comic_image{
                    height: 150px;
               img{
                   max-width: 100%;
                   object-fit: cover;
                   aspect-ratio: 1/1;
                   object-position: top;
                   border-radius: 0.2rem;
               }
           }
            }
         
        }
        .load_more {
            width: 150px;
            height: 40px;
            background-color: rgb(58, 116, 223);
            margin-top: 2rem;
            padding: 0.6rem;
            display: flex;
            align-items: center;
            justify-content: center;
            position: absolute;
            bottom: 3rem;
            left: 42%;
            p {
                color: white;
                font-size: 14px;
                font-weight: 600;
                text-transform: uppercase;
            }
        }
    }

    .container_bottom {
        height: 20%;
        background-color: rgb(58, 116, 223);
        position: relative;
        z-index: 1;
        .dc_actions {
            padding: 3rem 0;
            margin: auto;
            display: flex;
            justify-content: center;
            align-items: center;
            column-gap: 2rem;
            .dc_action {
                color: white;
                display: flex;
                align-items: center;
                column-gap: 0.6rem;
                img {
                    width: 35px;
                }
            }
        }
    }
</style>