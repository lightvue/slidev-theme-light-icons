<template>
  <div
    class="layout-name absolute text-xs mt-2 text-opacity-60 dark:text-opacity-60 shadow bg"
  >
    <slot />
  </div>
</template>
  <style>
.layout-name {
  bottom: 0;
  left: 50%;
  transform: translateX(-50%);
  padding: 8px 15px;
}
.layout-name.shadow {
  box-shadow: 0px 0px 30px rgba(107, 106, 106, 0.2),
    0px 0px 10px rgba(107, 106, 106, 0.1);
}
.dark .layout-name.shadow {
  box-shadow: 0px 0px 30px rgba(199, 199, 199, 0.042),
    0px 0px 10px rgba(107, 106, 106, 0.08);
}
.layout-name.bg {
  background-color: rgba(255, 255, 255, 0.9);
}
.dark .layout-name.bg {
  background-color: rgba(15, 41, 39, 0.9);
}
</style>