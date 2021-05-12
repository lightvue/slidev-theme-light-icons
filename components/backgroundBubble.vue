<template>
  <div class="relative h-full w-full">
    <div
      class="absolute"
      :style="{
        height: '200px',
        width: '200px',
        bottom: '-100px',
        left: '-100px',
        zIndex: '-10',
        opacity: '40%',
      }"
    >
      <img src="../assets/images/Ellipse1.png" alt="" />
    </div>
    <div
      class="absolute"
      :style="{
        height: '200px',
        width: '200px',
        bottom: '-100px',
        right: '-50px',
        zIndex: '-10',
        opacity: '40%',
      }"
    >
      <img src="../assets/images/Ellipse2.png" alt="" />
    </div>
    <div
      class="absolute"
      :style="{
        height: '200px',
        width: '200px',
        top: '-100px',
        left: '-100px',
        zIndex: '-10',
        opacity: '40%',
      }"
    >
      <img src="../assets/images/Ellipse3.png" alt="" />
    </div>
  </div>
</template>