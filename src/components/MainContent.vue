<template>
  <div class="h-full w-full">
    <div class="mx-2 my-5">
      <search-bar></search-bar>
    </div>
    <div class="m-2">
      <h1 class="text-2xl font-bold my-3">Offers</h1>
      <the-carousel></the-carousel>
    </div>
    <div class="m-2">
      <h1 class="text-2xl font-bold my-3">Choose by Class</h1>
      <class-grid></class-grid>
    </div>
  </div>
  <div class="m-4">
    <h1 class="text-2xl font-bold my-3">Featured Novels</h1>
    <horizontal-scroll :items="featuredNovels"></horizontal-scroll>
  </div>
  <div class="m-4">
    <h1 class="text-2xl font-bold my-3">Best Novels of all time</h1>
    <horizontal-scroll :items="bestNovels"></horizontal-scroll>
  </div>
  <div class="m-4">
    <h1 class="text-2xl font-bold mb-3">ISC Board Best Picks</h1>
    <horizontal-scroll :items="featuredNovels"></horizontal-scroll>
  </div>
</template>

<script>
import SearchBar from "./SearchBar.vue";
import TheCarousel from "./TheCarousel.vue";
import ClassGrid from "./ClassGrid.vue";
import HorizontalScroll from "./HorizontalScroll.vue";

export default {
  components: {
    "search-bar": SearchBar,
    "the-carousel": TheCarousel,
    "class-grid": ClassGrid,
    "horizontal-scroll": HorizontalScroll,
  },
  data() {
    return {
      featuredNovels: [
        {
          id: 1,
          name: "Greta Garbo in Anna Karenina",
          author: "Clarence Brown",
          discountPrice: 20,
          price: 400,
          discount: "50%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2019/11/81Y7nR4h6-L-687x1024.jpg",
        },
        {
          id: 2,
          name: "To Kill a Mockingbird",
          author: "Harper Lee",
          discountPrice: 575,
          price: 870,
          discount: "40%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2019/11/91smIBwwTgL-682x1024.jpg",
        },
        {
          id: 3,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 175,
          price: 600,
          discount: "70%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2019/11/715nOVKGKHL-667x1024.jpg",
        },
        {
          id: 4,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 375,
          price: 563,
          discount: "30%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2018/06/Jemisin_FifthSeason-TP.jpg",
        },
        {
          id: 5,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 265,
          price: 540,
          discount: "20%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2019/09/817FNKcZ1pL-663x1024.jpg",
        },
        {
          id: 6,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 321,
          price: 425,
          discount: "10%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2018/08/Salvage-the-Bones-Jesmyn-Ward.jpg",
        },
        {
          id: 7,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 200,
          price: 400,
          discount: "50%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2018/03/the-flamethrowers-9781439142011_hr-671x1024.jpg",
        },
        {
          id: 8,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 245,
          price: 725,
          discount: "62%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2019/11/all-my-puny-sorrows-665x1024.jpg",
        },
        {
          id: 9,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 150,
          price: 501,
          discount: "75%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2019/11/9496603.0-1366x2049-683x1024.jpg",
        },
        {
          id: 10,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 354,
          price: 505,
          discount: "22%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2015/05/sellout-683x1024.jpg",
        },
        {
          id: 11,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 452,
          price: 685,
          discount: "11%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2015/08/The-Sympathizer-by-Viet-Thanh-Nguyen.jpg",
        },
        {
          id: 12,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 273,
          price: 577,
          discount: "11%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2017/05/alittlelifecover.jpg",
        },
      ],
      bestNovels: [
        {
          id: 1,
          name: "Greta Garbo in Anna Karenina",
          author: "Clarence Brown",
          discountPrice: 20,
          price: 400,
          discount: "50%",
          image:
            "https://www.portersquarebooks.com/sites/portersquarebooks.com/files/teaspoonearthandsea.jpg",
        },
        {
          id: 2,
          name: "To Kill a Mockingbird",
          author: "Harper Lee",
          discountPrice: 575,
          price: 870,
          discount: "40%",
          image:
            "https://www.portersquarebooks.com/sites/portersquarebooks.com/files/thegoldfinch.jpg",
        },
        {
          id: 3,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 175,
          price: 600,
          discount: "70%",
          image:
            "https://www.portersquarebooks.com/sites/portersquarebooks.com/files/fromthememoirs.jpg",
        },
        {
          id: 4,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 375,
          price: 563,
          discount: "30%",
          image:
            "https://www.portersquarebooks.com/sites/portersquarebooks.com/files/smallfortune.jpg",
        },
        {
          id: 5,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 265,
          price: 540,
          discount: "20%",
          image:
            "https://www.portersquarebooks.com/sites/portersquarebooks.com/files/morethanthis.jpg",
        },
        {
          id: 6,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 321,
          price: 425,
          discount: "10%",
          image:
            "https://www.portersquarebooks.com/sites/portersquarebooks.com/files/josephanton.jpg",
        },
        {
          id: 7,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 200,
          price: 400,
          discount: "50%",
          image:
            "https://www.portersquarebooks.com/sites/portersquarebooks.com/files/aerogrammes.jpg",
        },
        {
          id: 8,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 245,
          price: 725,
          discount: "62%",
          image:
            "https://www.portersquarebooks.com/sites/portersquarebooks.com/files/subliminal.jpg",
        },
        {
          id: 9,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 150,
          price: 501,
          discount: "75%",
          image:
            "https://www.portersquarebooks.com/sites/portersquarebooks.com/files/wealthofnations.jpg",
        },
        {
          id: 10,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 354,
          price: 505,
          discount: "22%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2015/05/sellout-683x1024.jpg",
        },
        {
          id: 11,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 452,
          price: 685,
          discount: "11%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2015/08/The-Sympathizer-by-Viet-Thanh-Nguyen.jpg",
        },
        {
          id: 12,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 273,
          price: 577,
          discount: "11%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2017/05/alittlelifecover.jpg",
        },
      ],
      topRatedNovels: [
        {
          id: 1,
          name: "Greta Garbo in Anna Karenina",
          author: "Clarence Brown",
          discountPrice: 20,
          price: 400,
          discount: "50%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2019/11/81Y7nR4h6-L-687x1024.jpg",
        },
        {
          id: 2,
          name: "To Kill a Mockingbird",
          author: "Harper Lee",
          discountPrice: 575,
          price: 870,
          discount: "40%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2019/11/91smIBwwTgL-682x1024.jpg",
        },
        {
          id: 3,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 175,
          price: 600,
          discount: "70%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2019/11/715nOVKGKHL-667x1024.jpg",
        },
        {
          id: 4,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 375,
          price: 563,
          discount: "30%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2018/06/Jemisin_FifthSeason-TP.jpg",
        },
        {
          id: 5,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 265,
          price: 540,
          discount: "20%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2019/09/817FNKcZ1pL-663x1024.jpg",
        },
        {
          id: 7,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 200,
          price: 400,
          discount: "50%",
          image:
            "https://www.portersquarebooks.com/sites/portersquarebooks.com/files/aerogrammes.jpg",
        },
        {
          id: 8,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 245,
          price: 725,
          discount: "62%",
          image:
            "https://www.portersquarebooks.com/sites/portersquarebooks.com/files/subliminal.jpg",
        },
        {
          id: 9,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 150,
          price: 501,
          discount: "75%",
          image:
            "https://www.portersquarebooks.com/sites/portersquarebooks.com/files/wealthofnations.jpg",
        },
        {
          id: 10,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 354,
          price: 505,
          discount: "22%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2015/05/sellout-683x1024.jpg",
        },
        {
          id: 11,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 452,
          price: 685,
          discount: "11%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2015/08/The-Sympathizer-by-Viet-Thanh-Nguyen.jpg",
        },
        {
          id: 12,
          name: "Zero to One Notes",
          author: "Peter Thiel",
          discountPrice: 273,
          price: 577,
          discount: "11%",
          image:
            "https://s26162.pcdn.co/wp-content/uploads/2017/05/alittlelifecover.jpg",
        },
      ],
    };
  },
};
</script>
