<template>
  <div>
    <div class="page" @click="GoToNext">
      <div class="flex items-center justify-center mt-10">
        <div class="flex-1">
          <p class="text-5xl mx-auto text-center pb-4">
            Hello, my name is
          </p>
          <p class="text-4xl font-bold mx-auto text-center pb-4">
            M. Faizal Azzam
          </p>
          <div class="container m-auto">
            <div class="flex">
          <div class="flex-1 bg-gray-200 shadow-inner rounded-lg">

          <img
            src="~/assets/img/wujudsaya.png"
            class="object-scale-down h-96 w-full "
            alt=""
          />
        </div>
        </div>
      </div>
          <nuxt-link
            to="/Second"
            id="next"
            style="visibility: hidden"
          ></nuxt-link>
          <p class="text-md text-center pb-4 mt-8">
            I am a
          </p>
          <div
            class="flex flex-wrap text-center space-x-6 items-center justify-center"
          >
            <div class="flex-none">
              <li class="text-xl text-center">Vocational School Graduate</li>
            </div>
            <div class="flex-none">
              <li class="text-xl text-center">
                Computer Science Major
              </li>
            </div>
          </div>
          <div
            class="flex flex-wrap text-center space-x-6 items-center justify-center"
          >
            <div class="flex-none">
              <li class="text-xl text-center">Apprentice Programmer</li>
            </div>
            <div class="flex-none">
              <li class="text-xl text-center">FrontEnd Web Dev Wannabe</li>
            </div>
          </div>
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

<style scoped>
.bg-profile{
  animation: bg-profile 1s;
}

@keyframes bg-profile {
  from{transform:translateX(-20rem) ;}
  to{transform:translateX(0)}
}
</style>
