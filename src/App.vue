<template>
  <div class="flex flex-wrap overflow-hidden bg-center bg-no-repeat bg-cover bg-hero-pattern">
    <div class="fixed top-0 w-full overflow-hidden bg-transparent">
      <Navigation />
    </div>

    <div class="w-full h-screen">
      <Editor />
      <Tiptap />
    </div>

    <div class="fixed bottom-0 w-full overflow-hidden">
      <Controls />
    </div>
  </div>
</template>

<script>
import Navigation from "./components/Navigation.vue"
import Editor from "./components/Editor.vue"
import Controls from "./components/Controls.vue"
import Tiptap from "./components/Tiptap.vue"

export default {
  name: "App",
  components: {
    Navigation,
    Editor,
    Controls,
    Tiptap,
  },
  data() {
    return {
      isEditing: false,
    }
  },
  mounted() {
    console.log("Editing On")
  },

  methods: {},
}

// This starter template is using Vue 3 experimental <script setup> SFCs
// Check out https://github.com/vuejs/rfcs/blob/script-setup-2/active-rfcs/0000-script-setup.md
</script>

<style></style>
