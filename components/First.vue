<template>
  <div>
    <div class="page bg-lime-300" @click="GoToNext">
      <div class="screen-center flex items-center justify-center ">
        <div class="flex-1 ">
          <img
            src="~/assets/img/mukasaya.jpeg"
            class="object-scale-down h-48 w-full mb-6 "
            alt=""
          />
          <p class="text-6xl font-bold mx-auto text-center pb-4">M. Faizal Azzam</p>
          <div class="flex flex-wrap text-center space-x-6 ">
            <div class="flex-none">
              <li class="text-xl ">Lulusan SMK</li>
            </div>
            <div class="flex-none">
              <li class="text-xl ">Jurusan Pemrograman Perangkat Lunak</li>
            </div>
          </div>
          <div class="flex flex-wrap text-center space-x-6">
            <div class="flex-none">
              <li class="text-xl ">Apprentice Programmer</li>
            </div>
            <div class="flex-none">
              <li class="text-xl ">FrontEnd Web Dev Wannabe</li>
            </div>
          </div>
          <nuxt-link
            to="/Second"
            id="next"
            style="visibility: hidden"
          ></nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    GoToNext() {
      document.getElementById("next").click();
    },
  },
};
</script>

<style scoped></style>
