<template>
  <div class="w-full max-w-screen-xl mx-auto">
    <div class="flex justify-center">
      <div class="w-full max-w-md">
        <div class="bg-white shadow-md rounded-lg px-3 py-2 mb-4">
          <div class="block text-gray-700 text-lg font-semibold py-2 px-2">
            Search
          </div>
          <div class="flex items-center bg-gray-200 rounded-md">
            <div class="pl-2">
              <svg
                class="fill-current text-gray-500 w-6 h-6"
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
              >
                <path
                  class="heroicon-ui"
                  d="M16.32 14.9l5.39 5.4a1 1 0 0 1-1.42 1.4l-5.38-5.38a8 8 0 1 1 1.41-1.41zM10 16a6 6 0 1 0 0-12 6 6 0 0 0 0 12z"
                />
              </svg>
            </div>
            <input
              id="search"
              class="w-full rounded-md bg-gray-200 text-gray-700 leading-tight focus:outline-none py-2 px-2"
              type="text"
              placeholder="Search resource"
            />
          </div>
          <div class="py-3 text-sm"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      input: ``,
      dropdownOpen: false,
    }
  },
  methods: {
    clearInput() {
      this.reset()
    },
    openDropdown() {
      this.$emit('open-dropdown')
      this.openDropdown = true
      this.$emit('opened-dropdown')
    },
  },
}
</script>
