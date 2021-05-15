
  <template>
  <!-- Image is at Left -->
  <div v-if="left" class="relative h-full intro grid grid-cols-12">
    <div class="absolute h-full w-full" style="z-index: -10">
      <BubbleFrame v-if="!hideFrame"/>
    </div>
    <!-- Image -->
    <div
      :class="[equal ? 'col-span-6' : 'col-span-4', 'my-auto h-full']"
      :style="{ zIndex: '-1' }"
    >
      <div
        v-if="upperImage"
        class="absolute top-1/2 transform -translate-y-1/2"
        :class="left ? 'left-[80px]' : 'right-[80px]'"
        :style="{
          boxShadow: '0px 10px 30px rgba(0,0,0,0.7)',
          zIndex: '5',
        }"
      >
        <img :src="upperImage" class="w-[450px]" alt="" loading="lazy" />
      </div>
      <div
        v-if="image"
        class="my-auto h-full"
        :style="upperImage ? { ...style, filter: 'blur(3px)' } : { ...style }"
      ></div>
    </div>
    <!-- Layout -->
    <div
      :class="[
        'slidev-layout my-auto',
        image ? 'col-span-6' : 'col-span-12',
        equal ? 'col-span-6' : 'col-span-8',
      ]"
    >
      <slot />
    </div>
  </div>

  <!-- Image is at Right -->
  <div v-else class="relative h-full intro grid grid-cols-12">
    <div class="absolute h-full w-full" style="z-index: -10">
      <backgroundBubble />
    </div>
    <!-- Layout -->
    <div
      :class="[
        'slidev-layout my-auto',
        image ? 'col-span-6' : 'col-span-12',
        equal ? 'col-span-6' : 'col-span-8',
      ]"
    >
      <slot />
    </div>
    <!-- Image -->
    <div
      :class="[equal ? 'col-span-6' : 'col-span-4', 'my-auto h-full']"
      :style="{ zIndex: '-1' }"
    >
      <div
        v-if="upperImage"
        class="absolute top-1/2 transform -translate-y-1/2"
        :class="left ? 'left-[80px]' : 'right-[80px]'"
        :style="{
          boxShadow: '0px 10px 30px rgba(0,0,0,0.7)',
          zIndex: '5',
        }"
      >
        <img :src="upperImage" class="w-[450px]" alt="" loading="lazy" />
      </div>
      <div
        v-if="image"
        class="my-auto h-full"
        :style="
          upperImage
            ? {
                ...style,
                filter: 'blur(3px)',
              }
            : { ...style }
        "
      ></div>
    </div>
  </div>
</template>

<script setup lang="ts">
// Dependencies
import { computed, defineProps } from "vue";

// Utils
import { handleBackground } from "../utils";
const props = defineProps({
  image: {
    type: String,
    required: false,
  },
  upperImage: {
    type: String,
    required: false,
  },
  equal: {
    type: Boolean,
    default: false,
    required: false,
  },
  left: {
    type: Boolean,
    default: true,
    required: false,
  },
  hideFrame: {
    type: Boolean,
    default: false,
  }
});
// const style1 = {
//   filter: "blur(3px)",
//   backgroundImage: `url(${require("upperImage")})`,
//   backgroundRepeat: "no-repeat",
//   backgroundPosition: "center",
//   backgroundSize: "cover",
// };
const style = computed(() =>
  handleBackground(props.image, props.upperImage ? true : false)
);
</script>
