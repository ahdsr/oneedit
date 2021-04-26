<template>
  <div class="flex flex-wrap overflow-hidden bg-center bg-no-repeat bg-cover bg-hero-pattern">
    <div class="fixed top-0 w-full overflow-hidden bg-transparent">
      <transition name="fade">
        <Navigation v-if="navigationShowing" />
      </transition>
    </div>

    <div class="w-full h-screen" v-on:click="clickEdit">
      <Editor />

      <Tiptap />
      <PreviewPub v-if="previewShowing" />
    </div>

    <div class="fixed bottom-0 w-full overflow-hidden">
      <transition name="slide-fade">
        <Controls v-if="controlsShowing" :controlsShowing="controlsShowing" />
      </transition>
    </div>
  </div>
</template>

<script>
import Navigation from "./components/Navigation.vue"
import Editor from "./components/Editor.vue"
import Controls from "./components/Controls.vue"
import Tiptap from "./components/Tiptap.vue"
import PreviewPub from "./components/PreviewPub.vue"

export default {
  name: "App",
  components: {
    Navigation,
    Editor,
    Controls,
    Tiptap,
    PreviewPub,
  },
  data() {
    return {
      // isEditing: true,
      controlsShowing: true,
      previewShowing: true,
      navigationShowing: false,
    }
  },
  mounted() {
    this.controlsShowing = !this.controlsShowing

    console.log(this.controlsShowing)
  },

  methods: {
    clickEdit() {
      this.controlsShowing = !this.controlsShowing
      this.previewShowing = !this.previewShowing
      this.navigationShowing = !this.navigationShowing
      console.log(this.controlsShowing)
    },
  },
}

// This starter template is using Vue 3 experimental <script setup> SFCs
// Check out https://github.com/vuejs/rfcs/blob/script-setup-2/active-rfcs/0000-script-setup.md
</script>

<style>
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s ease;
}

.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}

.slide-fade-enter-active {
  transition: all 0.4s ease-out;
}

.slide-fade-leave-active {
  transition: all 0.4s cubic-bezier(1, 0.5, 0.4, 1);
}

.slide-fade-enter-from,
.slide-fade-leave-to {
  transform: translateY(100px);
  opacity: 0;
}
</style>
