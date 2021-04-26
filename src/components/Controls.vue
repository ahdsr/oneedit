<template>
  <div class="">
    <transition name="fade">
      <div class="overflow-hidden" v-if="colorSub" v-on:click="colorSub = !colorSub">
        <div
          class="p-4 overflow-hidden text-center transition duration-500 ease-in-out bg-black cursor-pointer hover:bg-opacity-20 hover:bg-white"
        >
          <div class="flex flex-wrap overflow-hidden">
            <div class="w-1/6 overflow-hidden">
              <div class="w-full h-10 bg-red-500">Red</div>
            </div>

            <div class="w-1/6 overflow-hidden">
              <div class="w-full h-10 bg-blue-500">Red</div>
            </div>

            <div class="w-1/6 overflow-hidden">
              <div class="w-full h-10 bg-yellow-500">Red</div>
            </div>

            <div class="w-1/6 overflow-hidden">
              <div class="w-full h-10 bg-indigo-500">Red</div>
            </div>

            <div class="w-1/6 overflow-hidden">
              <div class="w-full h-10 bg-green-500">Red</div>
            </div>

            <div class="w-1/6 overflow-hidden">
              <div class="w-full h-10 bg-purple-500">Red</div>
            </div>
          </div>
        </div>
      </div>
    </transition>
    <div class="mx-auto bg-gray-800 bg-opacity-20">
      <div class="flex flex-wrap justify-between overflow-hidden">
        <div class="w-1/3 overflow-hidden" v-on:click="toggleColors">
          <div
            class="p-2 overflow-hidden text-center transition duration-500 ease-in-out bg-black cursor-pointer hover:bg-opacity-20"
          >
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
                  <g>
                    <g>
                      <g>
                        <path
                          d="M12,22C6.49,22,2,17.51,2,12S6.49,2,12,2s10,4.04,10,9c0,3.31-2.69,6-6,6h-1.77c-0.28,0-0.5,0.22-0.5,0.5 c0,0.12,0.05,0.23,0.13,0.33c0.41,0.47,0.64,1.06,0.64,1.67C14.5,20.88,13.38,22,12,22z M12,4c-4.41,0-8,3.59-8,8s3.59,8,8,8 c0.28,0,0.5-0.22,0.5-0.5c0-0.16-0.08-0.28-0.14-0.35c-0.41-0.46-0.63-1.05-0.63-1.65c0-1.38,1.12-2.5,2.5-2.5H16 c2.21,0,4-1.79,4-4C20,7.14,16.41,4,12,4z"
                        />
                        <circle cx="6.5" cy="11.5" r="1.5" />
                        <circle cx="9.5" cy="7.5" r="1.5" />
                        <circle cx="14.5" cy="7.5" r="1.5" />
                        <circle cx="17.5" cy="11.5" r="1.5" />
                      </g>
                    </g>
                  </g>
                </g>
              </svg>
              <span class="text-xs text-gray-200">Color</span>
            </div>
          </div>
        </div>

        <div class="w-1/3 overflow-hidden">
          <div
            class="p-2 overflow-hidden text-center transition duration-500 ease-in-out bg-black cursor-pointer hover:bg-opacity-20"
          >
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
          <div
            class="p-2 overflow-hidden text-center transition duration-500 ease-in-out bg-black cursor-pointer hover:bg-opacity-20"
          >
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
                <g><rect fill="none" height="24" width="24" y="0" /></g>
                <g>
                  <path
                    d="M19.48,12.35c-1.57-4.08-7.16-4.3-5.81-10.23c0.1-0.44-0.37-0.78-0.75-0.55C9.29,3.71,6.68,8,8.87,13.62 c0.18,0.46-0.36,0.89-0.75,0.59c-1.81-1.37-2-3.34-1.84-4.75c0.06-0.52-0.62-0.77-0.91-0.34C4.69,10.16,4,11.84,4,14.37 c0.38,5.6,5.11,7.32,6.81,7.54c2.43,0.31,5.06-0.14,6.95-1.87C19.84,18.11,20.6,15.03,19.48,12.35z M10.2,17.38 c1.44-0.35,2.18-1.39,2.38-2.31c0.33-1.43-0.96-2.83-0.09-5.09c0.33,1.87,3.27,3.04,3.27,5.08C15.84,17.59,13.1,19.76,10.2,17.38z"
                  />
                </g>
              </svg>
              <span class="text-xs text-gray-200">Expression</span>
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
    return {colorSub: false}
  },
  mounted() {
    console.log(this.controlsShowing)
  },
  props: ["controlsShowing"],
  methods: {
    toggleColors() {
      this.colorSub = !this.colorSub
      console.log("pressed")
    },
  },
}
</script>

<style>
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.2s ease-out;
}

.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}

.slide-fade-enter-active {
  transition: all 0.2s ease-out;
}

.slide-fade-leave-active {
  transition: all 0.2s cubic-bezier(1, 0.5, 0.4, 1);
}

.slide-fade-enter-from,
.slide-fade-leave-to {
  transform: translateY(100px);
  opacity: 0;
}
</style>
