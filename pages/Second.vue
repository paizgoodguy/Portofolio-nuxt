<template>
  <div class="page bg-lime-300" @click="GoToNext">
    <div class="screen-center">
      <div>
        <div class="heading">
        <p class="text-5xl mx-auto text-center pb-4 ">
          Front End Framework that i use
        </p>
        <hr color="black" />
      </div>
        <div class="flex flex-wrap mt-6">
          <div class="flex-1 item-1">
            <div class="flex flex-wrap items-center justify-center ">
              <div class="flex-none w-28 ">
                <img
                  src="~/assets/img/vue.png"
                  class="object-scale-down h-16 w-28"
                  alt=""
                />
              </div>
              <div class="flex-1">
                <p class="max-w-sm">Vue.Js</p>
              </div>
            </div>
          </div>
          <div class="flex-1 item-2">
            <div class="flex flex-wrap items-center justify-center">
              <div class="flex-1">
                <img
                  src="~/assets/img/Nuxt.png"
                  class="object-scale-down h-16 w-28"
                  alt=""
                />
              </div>
              <div class="flex-1">
                <p class="max-w-sm">Nuxt.Js</p>
              </div>
            </div>
          </div>
          <div class="flex-1 item-3">
            <div class="flex flex-wrap items-center justify-center">
              <div class="flex-1">
                <img
                  src="~/assets/img/Vuetify.webp"
                  class="object-scale-down h-16 w-28"
                  alt=""
                />
              </div>
              <div class="flex-1">
                <p class="max-w-sm">Vuetify</p>
              </div>
            </div>
          </div>
        </div>

        <div class="flex flex-wrap mt-6">
          <div class="flex-1 item-4">
            <div class="flex flex-wrap items-center justify-end mr-10 ">
              <div class="flex-none ">
                <img
                  src="~/assets/img/Bootstrap.png"
                  class="object-scale-down h-16 w-28"
                  alt=""
                />
              </div>
              <div class="flex-none">
                <p class="max-w-sm">Bootstrap</p>
              </div>
            </div>
          </div>
          <div class="flex-1 item-5">
            <div class="flex flex-wrap items-center">
              <div class="flex-none">
                <img
                  src="~/assets/img/Tailwind.png"
                  class="object-scale-down h-16 w-28"
                  alt=""
                />
              </div>
              <div class="flex-none">
                <p class="max-w-sm">Tailwind</p>
              </div>
            </div>
          </div>
        </div>

        <nuxt-link to="/Three" id="next" style="visibility: hidden"></nuxt-link>
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
.heading {
  animation: heading 1s;

}

@keyframes heading {
  from {transform: translateX(-20rem);}
  to {transform: translateX(0rem);}
}
.item-1 {
  animation: item-1 1s;

}

@keyframes item-1 {
  from {transform: translateY(20rem);}
  to {transform: translateY(0rem);}
}

.item-2 {
  animation: item-2 1.2s;


}

@keyframes item-2 {
  from {transform: translateY(24rem);}
  to {transform: translateY(0rem);}
}

.item-3 {
  animation: item-3 1.4s;

}

@keyframes item-3 {
  from {transform: translateY(28rem);}
  to {transform: translateY(0rem);}
}

.item-4 {
  animation: item-4 1.6s;

}

@keyframes item-4 {
  from {transform: translateY(32rem);}
  to {transform: translateY(0rem);}
}

.item-5 {
  animation: item-5 1.8s;

}

@keyframes item-5 {
  from {transform: translateY(36rem);}
  to {transform: translateY(0rem);}
}


</style>
