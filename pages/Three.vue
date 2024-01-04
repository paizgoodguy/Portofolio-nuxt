<template>
  <div>
    <div class="page bg-lime-300" @click="GoToNext">
      <div class="screen-center flex items-center justify-center">
        <p class="text-5xl mx-auto pb-4">
          <span class="text-6xl font-bold">M</span>y other <br> skill
        </p>

        <ul class="list-disc ml-10">
          <li>Photography</li>
          <li>3D Art With Blender</li>
          <li>Adobe Lightroom</li>
          <li>Fluent In English</li>
          <!-- ... -->
        </ul>
      </div>
    </div>
    <nuxt-link to="/Four" id="next" style="visibility: hidden"></nuxt-link>
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
