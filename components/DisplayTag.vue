<template>
  <div class="layout-name absolute text-xs mt-2 shadow bg">
    <slot />
  </div>
</template>
<style>
.layout-name {
  bottom: 30px;
  left: 50%;
  transform: translateX(-50%);
  padding: 8px 12px;
  cursor: pointer;
  opacity: 0.7;
  transition: all 0.3s ease-in-out;
  border-radius: 4px;
}
.layout-name:hover {
  opacity: 1;
}
.layout-name.shadow {
  box-shadow: 0px 0px 30px rgba(107, 106, 106, 0.2), 0px 0px 10px rgba(107, 106, 106, 0.1);
}
.dark .layout-name.shadow {
  box-shadow: 0px 0px 30px rgba(199, 199, 199, 0.042), 0px 0px 10px rgba(107, 106, 106, 0.08);
}
.layout-name.bg {
  background-color: rgba(255, 255, 255, 0.9);
}
.dark .layout-name.bg {
  background-color: rgba(15, 41, 39, 0.9);
}
</style>
