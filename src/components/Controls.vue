<template>
  <div class="">
    <div class="mx-auto bg-gray-800 bg-opacity-20">
      <div class="flex flex-wrap overflow-hidden justify-be" v-show="menuShow">
        <div class="w-1/3 overflow-hidden" v-on:click="toggleMenu">
          <div class="p-2 overflow-hidden text-center bg-black">
            <div class="flex flex-col mx-auto sm:p-6">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                enable-background="new 0 0 24 24"
                height="24px"
                viewBox="0 0 24 24"
                width="24px"
                fill="#FFFFFF"
                class="self-center block p-1"
              >
                <g><rect fill="none" height="24" width="24" /></g>
                <g>
                  <g />
                  <g>
                    <circle cx="15.5" cy="9.5" r="1.5" />
                    <circle cx="8.5" cy="9.5" r="1.5" />
                    <path d="M12,18c2.28,0,4.22-1.66,5-4H7C7.78,16.34,9.72,18,12,18z" />
                    <path
                      d="M11.99,2C6.47,2,2,6.48,2,12c0,5.52,4.47,10,9.99,10C17.52,22,22,17.52,22,12C22,6.48,17.52,2,11.99,2z M12,20 c-4.42,0-8-3.58-8-8c0-4.42,3.58-8,8-8s8,3.58,8,8C20,16.42,16.42,20,12,20z"
                    />
                  </g>
                </g>
              </svg>
              <span class="text-xs text-gray-200">Feeling</span>
            </div>
          </div>
        </div>

        <div class="w-1/3 overflow-hidden">
          <div class="p-2 overflow-hidden text-center bg-black">
            <div class="flex flex-col mx-auto sm:p-6">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                enable-background="new 0 0 24 24"
                height="24px"
                viewBox="0 0 24 24"
                width="24px"
                fill="#FFFFFF"
                class="self-center block p-1"
              >
                <g><rect fill="none" height="24" width="24" /></g>
                <g>
                  <g />
                  <g>
                    <circle cx="15.5" cy="9.5" r="1.5" />
                    <circle cx="8.5" cy="9.5" r="1.5" />
                    <path d="M12,18c2.28,0,4.22-1.66,5-4H7C7.78,16.34,9.72,18,12,18z" />
                    <path
                      d="M11.99,2C6.47,2,2,6.48,2,12c0,5.52,4.47,10,9.99,10C17.52,22,22,17.52,22,12C22,6.48,17.52,2,11.99,2z M12,20 c-4.42,0-8-3.58-8-8c0-4.42,3.58-8,8-8s8,3.58,8,8C20,16.42,16.42,20,12,20z"
                    />
                  </g>
                </g>
              </svg>
              <span class="text-xs text-gray-200">Feeling</span>
            </div>
          </div>
        </div>

        <div class="w-1/3 overflow-hidden">
          <div class="p-2 overflow-hidden text-center bg-black">
            <div class="flex flex-col mx-auto sm:p-6">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                enable-background="new 0 0 24 24"
                height="24px"
                viewBox="0 0 24 24"
                width="24px"
                fill="#FFFFFF"
                class="self-center block p-1"
              >
                <g><rect fill="none" height="24" width="24" /></g>
                <g>
                  <g />
                  <g>
                    <circle cx="15.5" cy="9.5" r="1.5" />
                    <circle cx="8.5" cy="9.5" r="1.5" />
                    <path d="M12,18c2.28,0,4.22-1.66,5-4H7C7.78,16.34,9.72,18,12,18z" />
                    <path
                      d="M11.99,2C6.47,2,2,6.48,2,12c0,5.52,4.47,10,9.99,10C17.52,22,22,17.52,22,12C22,6.48,17.52,2,11.99,2z M12,20 c-4.42,0-8-3.58-8-8c0-4.42,3.58-8,8-8s8,3.58,8,8C20,16.42,16.42,20,12,20z"
                    />
                  </g>
                </g>
              </svg>
              <span class="text-xs text-gray-200">Feeling</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      menuShow: true,
    }
  },
  mounted() {
    console.log(this.menuShow)
  },

  methods: {
    toggleMenu() {
      this.menuShow = !this.menuShow
    },
  },
}
</script>

<style lang="scss" scoped></style>
