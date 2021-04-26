<template>
  <div class="">
    <div class="overflow-hidden" v-if="colorSub" v-on:click="colorSub = !colorSub">
      <div
        class="p-4 overflow-hidden text-center transition duration-500 ease-in-out bg-black border-b border-gray-800 cursor-pointer bg-opacity-10"
      >
        <div class="flex justify-between overflow-hidden flex-nowwrap">
          <div class="mx-auto overflow-hidden text-center">
            <div class="w-6 h-6 bg-red-500 rounded-md shadow-lg">R</div>
          </div>

          <div class="mx-auto overflow-hidden text-center">
            <div class="w-6 h-6 bg-blue-500 rounded-md shadow-lg">B</div>
          </div>

          <div class="mx-auto overflow-hidden text-center">
            <div class="w-6 h-6 bg-yellow-500 rounded-md shadow-lg">Y</div>
          </div>

          <div class="mx-auto overflow-hidden text-center">
            <div class="w-6 h-6 bg-indigo-500 rounded-md shadow-lg">I</div>
          </div>

          <div class="mx-auto overflow-hidden text-center">
            <div class="w-6 h-6 bg-green-500 rounded-md shadow-lg">G</div>
          </div>

          <div class="mx-auto overflow-hidden text-center">
            <div class="w-6 h-6 bg-purple-500 rounded-md shadow-lg">P</div>
          </div>
        </div>
      </div>
    </div>

    <div class="overflow-hidden" v-if="feelingSub" v-on:click="feelingSub = !feelingSub">
      <div
        class="p-4 overflow-hidden text-center transition duration-500 ease-in-out bg-black border-b border-gray-800 cursor-pointer bg-opacity-10"
      >
        <div class="flex flex-wrap overflow-hidden">
          <div class="mx-auto overflow-hidden text-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              height="24px"
              viewBox="0 0 24 24"
              width="24px"
              fill="#FFFFFF"
              class="self-center block text-white rounded-md shadow-lg fill-current hover:text-green-500"
            >
              <path d="M0 0h24v24H0V0z" fill="none" />
              <path
                d="M16.5 3c-1.74 0-3.41.81-4.5 2.09C10.91 3.81 9.24 3 7.5 3 4.42 3 2 5.42 2 8.5c0 3.78 3.4 6.86 8.55 11.54L12 21.35l1.45-1.32C18.6 15.36 22 12.28 22 8.5 22 5.42 19.58 3 16.5 3zm-4.4 15.55l-.1.1-.1-.1C7.14 14.24 4 11.39 4 8.5 4 6.5 5.5 5 7.5 5c1.54 0 3.04.99 3.57 2.36h1.87C13.46 5.99 14.96 5 16.5 5c2 0 3.5 1.5 3.5 3.5 0 2.89-3.14 5.74-7.9 10.05z"
              />
            </svg>
          </div>

          <div class="mx-auto overflow-hidden">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              enable-background="new 0 0 24 24"
              height="24px"
              viewBox="0 0 24 24"
              width="24px"
              fill="#FFFFFF"
              class="self-center block text-white fill-current hover:text-green-500"
            >
              <g><rect fill="none" height="24" width="24" /></g>
              <g>
                <g>
                  <path
                    d="M12,2C6.48,2,2,6.48,2,12c0,5.52,4.48,10,10,10s10-4.48,10-10 C22,6.48,17.52,2,12,2z M12,20c-4.41,0-8-3.59-8-8c0-4.41,3.59-8,8-8s8,3.59,8,8C20,16.41,16.41,20,12,20z"
                    fill-rule="evenodd"
                  />
                  <path
                    d="M13.49,11.38c0.43-1.22,0.17-2.64-0.81-3.62c-1.11-1.11-2.79-1.3-4.1-0.59 l2.35,2.35l-1.41,1.41L7.17,8.58c-0.71,1.32-0.52,2.99,0.59,4.1c0.98,0.98,2.4,1.24,3.62,0.81l3.41,3.41c0.2,0.2,0.51,0.2,0.71,0 l1.4-1.4c0.2-0.2,0.2-0.51,0-0.71L13.49,11.38z"
                    fill-rule="evenodd"
                  />
                </g>
              </g>
            </svg>
          </div>

          <div class="mx-auto overflow-hidden">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              height="24px"
              viewBox="0 0 24 24"
              width="24px"
              fill="#FFFFFF"
              class="self-center block text-white fill-current hover:text-green-500"
            >
              <path d="M0 0h24v24H0V0z" fill="none" />
              <path
                d="M19 5v2h-6V5h4M9 5v6H5V5h4m10 8v6h-6v-6h4M9 17v2H5v-2h4M21 3h-8v6h8V3zM11 3H3v10h8V3zm10 8h-8v10h8V11zm-10 4H3v6h8v-6z"
              />
            </svg>
          </div>

          <div class="mx-auto overflow-hidden">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              enable-background="new 0 0 24 24"
              height="24px"
              viewBox="0 0 24 24"
              width="24px"
              fill="#FFFFFF"
              class="self-center block text-white fill-current hover:text-green-500"
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
          </div>

          <div class="mx-auto overflow-hidden">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              enable-background="new 0 0 24 24"
              height="24px"
              viewBox="0 0 24 24"
              width="24px"
              fill="#FFFFFF"
              class="self-center block text-white fill-current hover:text-green-500"
            >
              <g><rect fill="none" height="24" width="24" /></g>
              <g>
                <g>
                  <path
                    d="M12,2C6.48,2,2,6.48,2,12c0,5.52,4.48,10,10,10s10-4.48,10-10 C22,6.48,17.52,2,12,2z M12,20c-4.41,0-8-3.59-8-8c0-4.41,3.59-8,8-8s8,3.59,8,8C20,16.41,16.41,20,12,20z"
                    fill-rule="evenodd"
                  />
                  <path
                    d="M13.49,11.38c0.43-1.22,0.17-2.64-0.81-3.62c-1.11-1.11-2.79-1.3-4.1-0.59 l2.35,2.35l-1.41,1.41L7.17,8.58c-0.71,1.32-0.52,2.99,0.59,4.1c0.98,0.98,2.4,1.24,3.62,0.81l3.41,3.41c0.2,0.2,0.51,0.2,0.71,0 l1.4-1.4c0.2-0.2,0.2-0.51,0-0.71L13.49,11.38z"
                    fill-rule="evenodd"
                  />
                </g>
              </g>
            </svg>
          </div>

          <div class="mx-auto overflow-hidden">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              height="24px"
              viewBox="0 0 24 24"
              width="24px"
              fill="#FFFFFF"
              class="self-center block text-white fill-current hover:text-green-500"
            >
              <path d="M0 0h24v24H0V0z" fill="none" />
              <path
                d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zM4 12c0-.61.08-1.21.21-1.78L8.99 15v1c0 1.1.9 2 2 2v1.93C7.06 19.43 4 16.07 4 12zm13.89 5.4c-.26-.81-1-1.4-1.9-1.4h-1v-3c0-.55-.45-1-1-1h-6v-2h2c.55 0 1-.45 1-1V7h2c1.1 0 2-.9 2-2v-.41C17.92 5.77 20 8.65 20 12c0 2.08-.81 3.98-2.11 5.4z"
              />
            </svg>
          </div>
        </div>
      </div>
    </div>

    <div class="overflow-hidden" v-if="expressionSub" v-on:click="expressionSub = !expressionSub">
      <div
        class="p-4 overflow-hidden text-center transition duration-500 ease-in-out bg-black border-b border-gray-800 cursor-pointer bg-opacity-10"
      >
        <div class="flex flex-wrap overflow-hidden">
          <div class="mx-auto overflow-hidden text-center">
            <div class="w-6 h-6 bg-red-500 rounded-md shadow-lg">R</div>
          </div>

          <div class="mx-auto overflow-hidden text-center">
            <div class="w-6 h-6 bg-blue-500 rounded-md shadow-lg">B</div>
          </div>

          <div class="mx-auto overflow-hidden text-center">
            <div class="w-6 h-6 bg-yellow-500 rounded-md shadow-lg">Y</div>
          </div>

          <div class="mx-auto overflow-hidden text-center">
            <div class="w-6 h-6 bg-indigo-500 rounded-md shadow-lg">I</div>
          </div>

          <div class="mx-auto overflow-hidden text-center">
            <div class="w-6 h-6 bg-green-500 rounded-md shadow-lg">G</div>
          </div>

          <div class="mx-auto overflow-hidden text-center">
            <div class="w-6 h-6 bg-purple-500 rounded-md shadow-lg">P</div>
          </div>
        </div>
      </div>
    </div>

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

        <div class="w-1/3 overflow-hidden" v-on:click="toggleFeelings">
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

        <div class="w-1/3 overflow-hidden description" v-on:click="toggleExpressions">
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
    return {
      colorSub: false,
      feelingSub: false,
      expressionSub: false,
      theme: "blue-theme",
      emits: ["enlargeText"],
    }
  },
  mounted() {
    console.log(this.controlsShowing)
  },
  props: ["controlsShowing"],
  methods: {
    toggleColors() {
      this.feelingSub = false
      this.expressionSub = false
      this.colorSub = !this.colorSub
      this.$emit("enlargeText", "someValue")
      console.log("pressed")
    },
    toggleFeelings() {
      this.expressionSub = false
      this.colorSub = false
      this.feelingSub = !this.feelingSub
      console.log("pressed")
    },
    toggleExpressions() {
      this.colorSub = false
      this.feelingSub = false

      this.expressionSub = !this.expressionSub
      console.log("pressed")
    },
  },
}
</script>

<style>
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s ease-out;
}

.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}

.slide-fade-from {
  transition: all 0.5s ease-out;
}

.slide-fade-enter-active {
  transition: all 0.5s ease-out;
}

.slide-fade-leave-active {
  transition: all 0.5s cubic-bezier(1, 0.9, 0.8, 1);
}

.slide-fade-enter-from,
.slide-fade-leave-to {
  transform: translateY(100px);
  opacity: 0;
}
</style>
