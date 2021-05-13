---
theme: none
layout: intro
image: 'https://source.unsplash.com/collection/94734566/1920x1080'
---

  <div class="absolute pt-6 left-12">
    <span @click="next" class="py-1 rounded cursor-pointer hover:bg-white hover:bg-opacity-10 flex justify-center items-center">
      Press Space for next page  <light-icon icon="arrow-narrow-right" size="24px"/> 
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
imageHeader: '../assets/images/light-icon-logo.svg'
---
  <display-tag >
    <span>
     Layout: <span class="text-primary text-opacity-80 dark:text-opacity-60"> image-header-intro </span>
    </span>
  </display-tag>

  <div class="leading-snug text-black dark:text-white text-opacity-60 dark:text-opacity-60 mt-4">
    The Emerging light weight icon library for Vue 3.x & Vue 2.x
  </div> 
  <div class="absolute pt-6 left-12">
    <span @click="next" class="py-1 p-2 rounded cursor-pointer hover:bg-white hover:bg-opacity-10 flex justify-center items-center">
      Press Space for next page  <light-icon icon="arrow-narrow-right" size="24px"/> 
    </span>
  </div>


---
layout: image-header-intro
imageHeader: '../assets/images/light-icon-logo.svg'
imageRight: '../assets/images/light-vue-landing.svg'
---
  <display-tag >
    <span>
     Layout: <span class=" text-primary text-opacity-80 dark:text-opacity-60"> image-header-intro </span>
    </span>
  </display-tag>

  <div class="leading-snug text-black dark:text-white text-opacity-60 dark:text-opacity-60 mt-4">
    The Emerging light weight icon library for Vue 3.x & Vue 2.x
  </div>




---
layout: image-left
image: '../assets/images/light-icons-landing.svg'
equal: true
---
  <display-tag>
    <span>
     Layout: <span class=" text-primary text-opacity-80 dark:text-opacity-60"> image-left </span>
    </span>
  </display-tag>
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
  <display-tag >
    <span>
     Layout: <span class="text-primary text-opacity-80 dark:text-opacity-60"> dynamic-image </span>
    </span>
  </display-tag>

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
layout: dynamic-image 
image: 'https://source.unsplash.com/collection/94734566/1920x1080'
equal: false
left: false
---
  <display-tag >
    <span>
     Layout: <span class=" text-primary text-opacity-80 dark:text-opacity-60"> dynamic-image </span>
    </span>
  </display-tag>

  <div class="text-black dark:text-white text-opacity-60 dark:text-opacity-60 pt-2 font-sm">
    <span class="text-sm">
      Image at right
    </span>
  </div>
  <div class="text-primary dark:text-primary-lighter pb-2 pt-4">
    <span class="">
      Theme Configuration
    </span>
  </div>


```ts
layout: dynamic-image //Layout Name
image: 'https://source.unsplash.com/collection/94734566/1920x1080'
equal: false
left: false
```




---
layout: dynamic-image 
image: 'https://source.unsplash.com/collection/94734566/1920x1080'
equal: false
left: true
---
  <display-tag >
    <span>
     Layout: <span class=" text-primary text-opacity-80 dark:text-opacity-60"> dynamic-image </span>
    </span>
  </display-tag>

  <div class="text-black dark:text-white text-opacity-60 dark:text-opacity-60 pt-2 font-sm">
      <span class="text-sm">
        Image at left
      </span>
  </div>
  <div class="text-primary dark:text-primary-lighter pb-2 pt-2">
    <span class="">
      Theme Configuration
    </span>
  </div>

```ts
layout: dynamic-image //Layout Name
image: 'https://source.unsplash.com/collection/94734566/1920x1080'
equal: false
left: true
```




---
layout: dynamic-image 
image: 'https://source.unsplash.com/collection/94734566/1920x1080'
equal: true
left: false
---
  <display-tag >
    <span>
     Layout: <span class=" text-primary text-opacity-80 dark:text-opacity-60"> dynamic-image </span>
    </span>
  </display-tag>

  <div class="text-black dark:text-white text-opacity-60 dark:text-opacity-60 pt-2 font-sm">
      <span class="text-sm">
        Equal Width
      </span>
  </div>
  <div class="text-primary dark:text-primary-lighter pb-2 pt-2">
    <span class="">
      Theme Configuration
    </span>
  </div>

```ts
layout: dynamic-image //Layout Name
image: 'https://source.unsplash.com/collection/94734566/1920x1080'
equal: true
left: false
```




---
layout: dynamic-image 
image: 'https://source.unsplash.com/collection/94734566/1920x1080'
upperImage: 'https://source.unsplash.com/collection/94734566/1920x1080'
equal: true
left: false
---
  <display-tag >
    <span>
     Layout: <span class=" text-primary text-opacity-80 dark:text-opacity-60"> dynamic-image </span>
    </span>
  </display-tag>

  <div class="text-black dark:text-white text-opacity-60 dark:text-opacity-60 pt-2 font-sm">
      <span class="text-sm">
        Floating image
      </span>
  </div>
  <div class="text-primary dark:text-primary-lighter pb-2 pt-2">
    <span class="">
      Theme Configuration
    </span>
  </div>

```ts
layout: dynamic-image //Layout Name
image: 'https://source.unsplash.com/collection/94734566/1920x1080'
upperImage: 'https://source.unsplash.com/collection/94734566/1920x1080'
equal: true
left: false
```




---
layout: center-image
image: '../assets/images/light-icons-landing2.png'
---
  <display-tag >
    <span>
     Layout: <span class=" text-primary text-opacity-80 dark:text-opacity-60"> center-image </span>
    </span>
  </display-tag>

  <div class="mb-4">
    <span class="text-3xl text-primary dark:text-primary-lighter" style="font-weight:500;" >Vast Selection of Light Weight Icons</span>
  </div>




---
layout: dynamic-image
image: 'https://source.unsplash.com/collection/94734566/1920x1080'
equal: false
left: false
---
  <display-tag >
    <span>
     Layout: <span class=" text-primary text-opacity-80 dark:text-opacity-60"> dynamic-image </span>
    </span>
  </display-tag>

  <div class="text-primary dark:text-primary-lighter ">
    <span class="text-xl">
     Easy to use Syntax:
    </span>
  </div>
  
  <div class="flex items-end justify-between pb-2 pt-5">
    <div class="">
      <i class="light-icon-brand-facebook" style="font-size:24px;" ></i>
    </div>
    <span class="text-xs opacity-60">
      Universal
    </span>
  </div>

  ```ts
  // Universal
  <i class="light-icon-brand-facebook"></i> 
  ```


  <div class="flex items-end justify-between pb-2 pt-5">
    <div class="">
      <light-icon icon="brand-facebook" size="24px" />
    </div>
    <span class="text-xs opacity-60">
      Inbuilt in theme
    </span>
  </div>

  ```ts
  // Inbuilt component in theme
  <light-icon icon="brand-facebook" size="24px" />
  ```


  <div class="flex items-end justify-between pb-2 pt-5">
    <div class="">
      <icon-wrapper>
        <light-icon icon="brand-facebook" size="24px" />
      </icon-wrapper>
    </div>
    <span class="text-xs opacity-60 ">
      Inbuilt in theme
    </span>
  </div>

  ```ts
  // Inbuilt wrapper-component in theme
  <icon-wrapper>
    <light-icon icon="brand-facebook" size="24px" />
  </icon-wrapper>
  ```




---
layout: center-image
---
  <display-tag>
    <span>
     Layout: <span class=" text-primary "> center-image </span>
    </span>
  </display-tag>

  <div class="mb-0">
    <span class="text-3xl text-primary dark:text-primary-lighter" style="font-weight:600;text-transform: uppercase;" >Explore More</span>
  </div>
  <div class="mb-0">
    <a href="https://icons.lightvue.org/" target="_blank" class="">Documentation</a> |
    <a href="https://github.com/lightvue/light-icons" target="_blank" class="">Contribute</a>
  </div>

  <style>
    a {
      margin: 10px;
    }

    a:hover{
      opacity:0.7;
    }
  </style>

