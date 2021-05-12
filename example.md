---
theme: none
layout: intro
image: 'https://source.unsplash.com/collection/94734566/1920x1080'
---

  <div class="absolute pt-6 left-12">
    <span @click="next" class="py-1 rounded cursor-pointer hover:bg-white hover:bg-opacity-10">
      Press Space for next page <light-icon icon="arrow-narrow-right" size="24px"/> 
    </span>
  </div>

  <div class="mb-4 absolute bottom-4 left-12">
    <span class="text-6xl text-primary-lighter text-opacity-80" style="font-weight:500;" >
    Slidev Theme
    </span>
    <div class="text-9xl text-white text-opacity-60" style="font-weight:600;" >
    LIGHT ICONS
    </div> 
  </div>


---
layout: image-header-intro
imageHeader: '../assets/images/light-vue-logo.svg'
---
  <div class="leading-snug text-black dark:text-white text-opacity-60 dark:text-opacity-60 mt-4">
    The Emerging UI Component library for Vue 3.x & Vue 2.x
  </div> 
  <div class="pt-6">
    <span @click="next" class="py-1 rounded cursor-pointer hover:bg-white hover:bg-opacity-10">
      Press Space for next page <carbon:arrow-right class="inline"/>
    </span>
  </div>


---
layout: image-header-intro
imageHeader: '../assets/images/light-vue-logo.svg'
imageRight: '../assets/images/light-vue-landing.svg'
---
  <div class="leading-snug text-black dark:text-white text-opacity-60 dark:text-opacity-60 mt-4">
    The Emerging UI Component library for Vue 3.x & Vue 2.x
  </div>


---
layout: image-left
image: '../assets/images/light-icons-landing.svg'
equal: true
---
  <div class="">
    <h1 class="text-primary dark:text-primary-lighter" >Premium collection of light icons</h1>
  </div>
  <div class="leading-snug text-black dark:text-white text-opacity-60 dark:text-opacity-60">
    UI Library hands out everything you need to create contemporary, engaging, and responsive web applications. A platform set to offer unlimited light customizable UI variants and an implementation playground to define how your components would look to and fro.
  </div>


---
layout: dynamic-image
image: 'https://source.unsplash.com/collection/94734566/1920x1080'
equal: true
left: false
---
  <div class="text-primary dark:text-primary-lighter pb-2 pt-4">
    <span class="">
      For Installation
    </span>
  </div>


```ts
npm install light-icons --save
```

  <div class="text-primary dark:text-primary-lighter pb-2 pt-4">
    <span class="">
      Import CSS file
    </span>
  </div>

```ts
/* import in CSS files [with CSS Loader] */
@import "~light-icons/dist/light-icon.css";
```

  <div class="text-black dark:text-white text-opacity-80 dark:text-opacity-80 pb-2 pt-4">
    <span class="block pb-2 text-primary dark:text-primary-lighter">
      How to use
    </span>
    <span class="text-xs " >
      Add 
      <kbd style="font-size: 0.6rem;" >light-icon-*</kbd>
      class, either in
      <kbd style="font-size: 0.6rem;">i</kbd> 
      or 
      <kbd style="font-size: 0.6rem;">span</kbd> 
      HTML Tag
    </span>
  </div>

```ts
<i class="light-icon-facebook"></i>
```


---
layout: center-image
image: '../assets/images/light-vue-landing.png'
---
  <div class="mb-4">
    <span class="text-3xl text-primary dark:text-primary-lighter" style="font-weight:500;" >Minimalist Design</span>
  </div>


---
layout: center-image
image: '../assets/images/light-icons-landing1.png'
---
  <div class="mb-4">
    <span class="text-3xl text-primary dark:text-primary-lighter" style="font-weight:500;" >Vast Selection of Light Weight Icons</span>
  </div>


---
layout: center-image
image: '../assets/images/light-icons-landing2.png'
---
  <div class="mb-4">
    <span class="text-3xl text-primary dark:text-primary-lighter" style="font-weight:500;" >Vast Selection of Light Weight Icons</span>
  </div>

  
---
layout: center-image
class: "text-center"
---
  <div class="mb-0">
    <span class="text-3xl text-primary dark:text-primary-lighter" style="font-weight:600;" >Visit Us</span>
  </div>
  <div class="mb-0">
    <a href="https://lightvue.org/" target="_blank" class="">Light Vue</a> | <a href="https://lightvue.org/getting-started/light-icons" target="_blank" class="">Light Icons</a>
  </div>

  <style>
    a {
      margin: 10px;
    }

    a:hover{
      opacity:0.7;
    }
  </style>

