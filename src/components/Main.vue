<script setup lang="ts">
import Content from "./Content.vue";
import BlendImage from "./BlendImage.vue";
import Card from "./Card.vue";
import Carousel from "./Carousel.vue";

const listPelanggan = [
  { nama: "Kabupaten", jumlah: 10 },
  { nama: "Kelurahan", jumlah: 156 },
  { nama: "Desa", jumlah: 1908 },
  { nama: "Pelanggan", jumlah: 3008 },
];
</script>

<template>
  <div class="bg-slate-900 w-full text-white py-6">
    <Content>
      <template #title>
        <h1
          class="mx-6 my-6 text-3xl font-bold bg-gradient-to-r from-slate-100 to-slate-400 bg-clip-text text-transparent"
        >
          #Internet Lebih Cepat!
        </h1>
      </template>
      <template #paragraf1>
        Era digital memberikan banyak kemudahan dalam beraktivitas sehari-hari,
        seperti meeting online, upload download, menayangkan sesi live dan
        streaming.
      </template>
      <template #subTitle>SahazNetwork Internet</template>
      <template #paragraf2>
        Hadir dengan bandwidth hingga 250 Mbps dan kuota unlimited. Sehingga
        kamu dapat melakukan kegiatan digital 24/7 tanpa perlu khawatir.
      </template>
    </Content>
  </div>
  <BlendImage>
    <template #img>
      <img
        class="object-cover w-full h-full"
        src="https://source.unsplash.com/400x350?internet"
        alt=""
      />
    </template>
    <div
      class="absolute inset-0 bg-gradient-to-t from-transparent to-slate-900 from-60%"
    ></div>
  </BlendImage>
  <div class="w-full bg-white py-6">
    <Content>
      <template #title>
        <h1
          class="mx-6 my-6 text-3xl font-bold bg-gradient-to-r from-amber-400 to-amber-600 bg-clip-text text-transparent"
        >
          Bermain Game Tanpa Lag!
        </h1>
      </template>
      <template #paragraf1>
        Tingkatkan level dan kuasai permainan untuk menjadi pemain profesional
        terbaik. Dengan jaringan Internet WiFi cepat dan stabil, lawan musuh
        kamu dengan kecepatan maksimum tanpa nge-lag.
      </template>
      <template #subTitle>SahazNetwork Gamers</template>
      <template #paragraf2>
        Biznet Home Gamers memiliki bandwidth hingga 250 Mbps dengan IP Public.
        Dapatkan pengalaman terbaik saat bermain game untuk terus jadi juara!
      </template>
    </Content>
  </div>
  <BlendImage>
    <template #img>
      <img
        class="object-cover w-full h-full"
        src="https://source.unsplash.com/400x350?gamers"
        alt=""
      />
    </template>
  </BlendImage>
  <div class="w-full bg-slate-900 text-white py-6">
    <Content>
      <template #title>
        <h1
          class="mx-6 my-6 text-3xl font-bold bg-gradient-to-r from-slate-100 to-slate-400 bg-clip-text text-transparent"
        >
          Hiburan Interaktif Untuk di Rumah
        </h1>
      </template>
      <template #paragraf1>
        Ciptakan momen bermakna dengan dukungan Internet WiFi terbaik dan
        program TV interaktif berkualitas di rumah kamu.
      </template>
      <template #subTitle>SahazNetwork Combo IPTV</template>
      <template #paragraf2>
        Hadir dengan kualitas resolusi gambar 4K terbaik dan bandwidth mulai
        dari 100 Mbps. Dapatkan konten hiburan berkualitas yang dapat dinikmati
        kapan saja.
      </template>
    </Content>
  </div>
  <BlendImage>
    <template #img>
      <img
        class="object-cover w-full h-full"
        src="https://source.unsplash.com/400x350?tv"
        alt=""
      />
    </template>
    <div
      class="absolute inset-0 bg-gradient-to-t from-transparent to-slate-900 from-60%"
    ></div>
  </BlendImage>
  <div class="w-full bg-white py-6">
    <div class="flex justify-center items-center">
      <h1 class="mx-6 my-6 text-3xl font-bold text-center">
        Pilihan Paket SahazNetwork
      </h1>
    </div>
    <Card />
  </div>
  <Carousel />
  <div class="w-full bg-slate-900 py-6">
    <div class="flex flex-col md:flex-row flex-wrap justify-center">
      <div
        class="md:w-1/2 p-6 box-border text-white text-center justify-center"
        v-for="{ nama, jumlah } in listPelanggan"
      >
        <h1 class="text-lg font-medium">{{ nama }}</h1>
        <div>
          <p class="text-2xl font-bold">{{ jumlah }}</p>
        </div>
      </div>
    </div>
  </div>
</template>
