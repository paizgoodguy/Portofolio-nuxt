<template>

  <main>

  <First />
  </main>
</template>

<script>

export default {
  name: "IndexPage",




  // transition (to, from) {
  //   const getDepth = (path) => {
  //   return path.split('/').filter(seg => seg.length > 0).length;
  // }

  // const toDepth = getDepth(to.path);
  // const fromDepth = getDepth(from.path);

  // if (toDepth > fromDepth) {
  //   to.meta.pageTransition = { name: 'page-left' };
  //   from.meta.pageTransition = { name: 'page-left' };
  // } else {
  //   to.meta.pageTransition = { name: 'page-right' };
  //   from.meta.pageTransition = { name: 'page-right' };
  // }
  // }
};
</script>

<style>
.screen-center {
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  position: fixed;
}

.page {
  min-height: 100vh;
  width: 100%;
  overflow: hidden;
}

/* .page-left-enter-active,
.page-right-enter-active,
.page-left-leave-active,
.page-right-leave-active {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  transition: all 150ms linear;
}

.page-left-enter-from, .page-right-leave-to {
  transform: translateX(100%);
}

.page-left-leave-to, .page-right-enter-from {
  transform: translateX(-100%);
}

.page-left-enter-to, .page-right-enter-to {
  transform: translateX(0);
} */

.page-enter-active,
.page-leave-active {
  transition: opacity 0.3s;
}

.page-enter,
.page-leave-active {
  opacity: .5;
}
</style>
