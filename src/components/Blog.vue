<template>
  <div class="Blog">
      <div class="container">
        <div class="konten-blog" v-for="(data, index) in blog" :value="data" :key="index">
            <div class="max-w-sm rounded overflow-hidden shadow-lg">
                <div class="foto-blog">
                    <img v-bind:src="data.image" class="img-fluid img-blog" @click="detailfilm(data.id)" v-bind:alt="data">
                </div>
                <div class="isi-blog">
                    <div class="font-bold text-xl mb-2">{{data.title}}</div>
                    <p class="text-gray-700 text-base">
                        {{data.isi}}
                    </p>
                </div>
                <div class="px-6 py-4">
                    <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2">#quran</span>
                    <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700">#dirumahaja</span>
                </div>
            </div>
        </div>
      </div>
      <div class="footer">
            <h5>Build &copy;2020. By DaarusyGibran</h5>
      </div>
  </div>
</template>

<script>
import Img1 from '../assets/quran3.jpg'
import Img2 from '../assets/quran5.jpg'
import Img3 from '../assets/quran6.jpg'
export default {
  name: 'Blog',
  data: () => ({
    blog: [
      { id: 1, title: 'Sahabat Al-Quran', isi: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus quia, nulla! Maiores et perferendis eaque, exercitationem praesentium nihil.', image: Img1 },
      { id: 2, title: 'Sahabat Al-Quran', isi: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus quia, nulla! Maiores et perferendis eaque, exercitationem praesentium nihil.', image: Img2 },
      { id: 3, title: 'Sahabat Al-Quran', isi: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus quia, nulla! Maiores et perferendis eaque, exercitationem praesentium nihil.', image: Img3 },
      { id: 4, title: 'Sahabat Al-Quran', isi: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus quia, nulla! Maiores et perferendis eaque, exercitationem praesentium nihil.', image: Img1 },
      { id: 5, title: 'Sahabat Al-Quran', isi: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus quia, nulla! Maiores et perferendis eaque, exercitationem praesentium nihil.', image: Img2 },
      { id: 6, title: 'Sahabat Al-Quran', isi: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus quia, nulla! Maiores et perferendis eaque, exercitationem praesentium nihil.', image: Img3 }
    ]
  })
}
</script>

<style>
    .Blog {
    padding-top: 20px;
    }
    .container {
    width: auto;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-auto-rows: minmax(50px, auto);
    background-color: #ffffff;
    }
    .konten-blog {
    padding: 20px;
    background-color: #FFFFFF;
    }
    .isi-blog {
    padding: 10px;
    }
    .footer {
    padding: 10px;
    grid-column: 1/5;
    background-color: #000;
    color: #fff;
    text-align: center;
    margin-top: 10px;
    }
</style>
