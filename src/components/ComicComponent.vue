<template>
      <div class="col-2" >
        <div class="comic_image">
            <img :src="comic.thumb" :alt="comic.series">
        </div>
        <div class="comic_text">
            <p>{{ comic.series }}</p>
        </div>
       </div>
</template>

<script>
 export default {
        name:'ComicComponent',
        component: {

        },
        props: {
            comic : Object,

        }
        
    }

</script>

<style lang="scss" scoped>
    .container_mid {
        background-color: black ;
        height: 500px;        
        padding: 4rem;
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
    }

</style>
