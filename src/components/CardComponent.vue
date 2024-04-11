<template>
  <div class="row">
        <div class="col-12 col-md-4 col-lg-2" v-for="(item, index) in items" :key="index">
            <div class="image"><img :src="item.thumb" :alt="item.series"></div>
            <h5>{{ item.series }}</h5>
        </div>
        <div class="text-center"><a href="#">load more</a></div>
    </div>

</template>

<script>
    export default {
        name: 'CardComponent.vue',
     props: ['items']
    }
</script>

<style lang="scss" scoped>
// .row {
//         .image {
//             padding: 20px 0;
//             img {
//             width: 100%;
//             height: 300px;
//             }
//             img:hover {
//                 cursor: pointer;
                
//             }
//         }
//         h5 {
//             color: white;
//             text-transform: uppercase;
//             padding: 10px 0;
//         }
//         .text-center {
//             padding: 30px;
//         }
//         a {
//             text-decoration: none;
//             color: white;
//             text-transform: uppercase;
//             font-weight: 500;
//             font-size: 1.2rem;
//             padding: 10px 100px;
//             background-color: lightblue;
//         }
//     }

</style>