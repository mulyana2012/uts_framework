<script>
export default {
  data() {
    return {
      data_images: [
        {
          id: 1,
          logo_name: 'CHELSEA',
          logo_file: 'bola1.png',
          palyed: 8,
          scores: 4,
          lose: 0,
          rating: 5,
        },
        {
          id: 2,
          logo_name: 'WINBLEDON',
          logo_file: 'bola2.png',
          palyed: 6,
          scores: 2,
          lose: 2,
          rating: 3,
        },
        {
          id: 3,
          logo_name: 'Bournemouth',
          logo_file: 'bola3.png',
          palyed: 6,
          scores: 2,
          lose: 2,
          rating: 3,
        },
        {
          id: 4,
          logo_name: 'Newcastle United',
          logo_file: 'bola4.png',
          palyed: 6,
          scores: 2,
          lose: 2,
          rating: 3,
        },
        {
          id: 5,
          logo_name: 'Tottenham Hotspur',
          logo_file: 'bola5.png',
          palyed: 6,
          scores: 2,
          lose: 2,
          rating: 3,
        },
        {
          id: 6,
          logo_name: 'CHAMPION TEAM',
          logo_file: 'bola6.png',
          palyed: 6,
          scores: 2,
          lose: 2,
          rating: 3,
        },
        {
          id: 7,
          logo_name: 'SOCCER CLUB',
          logo_file: 'bola7.png',
          palyed: 6,
          scores: 2,
          lose: 2,
          rating: 3,
        },
        {
          id: 8,
          logo_name: 'REAL MADRID',
          logo_file: 'bola8.png',
          palyed: 6,
          scores: 2,
          lose: 2,
          rating: 3,
        },
        {
          id: 9,
          logo_name: 'ALMERIA',
          logo_file: 'bola9.png',
          palyed: 6,
          scores: 2,
          lose: 2,
          rating: 3,
        },
        {
          id: 10,
          logo_name: 'FC BAZENHEID',
          logo_file: 'bola10.png',
          palyed: 6,
          scores: 2,
          lose: 2,
          rating: 3,
        },
      ],
    };
  },
};
</script>
<template>
  <div>
    <div class="row row-cols-1 row-cols-md-5 g-4">
      <div v-for="data_images in data_images" class="col">
        <a class="btn btn-link btn-block">
          <router-link :to="'/detail/' + data_images.id">
            <div class="col">
              <div class="card h-100">
                <div class="card-body">
                  <img :src="'/src/assets/logo_bola/' + data_images.logo_file" class="card-img-top" alt="404" />
                </div>
                <h6 id="text__decotation" class="text-center">
                  {{ data_images.logo_name }}
                </h6>
              </div>
            </div>
          </router-link>
        </a>
      </div>
    </div>
  </div>
</template>

<style>
img {
  width: 170px;
}
</style>
