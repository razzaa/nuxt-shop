<template>
<div class="h-screen w-full bg-gray-800">
  <div class="h-screen mx-auto max-w-screen-sm">
    <div class="p-12">
      <p class="mx-auto text-5xl pt-10 text-yellow-500 font-bold">
        Welcome 
        Back
      </p>
      <p class="text-xl py-3 text-gray-400 font-semibold">Sign in to continue</p>
    </div>
    <div class="mx-12 pl-3 pt-3 pr-3 pb-8 rounded-xl shadow-sm bg-gray-900">
      <div class="p-3 mx-6 border-b border-gray-500">
        <input placeholder="Phone Number" class="bg-transparent text-yellow-500 w-full focus:outline-none focus:rang" type="tel" />
      </div>

      <div class="p-3 mx-6 flex border-b border-gray-500">
        <input v-bind:type="[showPassword ? 'text' : 'password']" placeholder="Password" class="bg-transparent text-yellow-500 focus:outline-none focus:rang w-full" />
        <div @click="showPassword = !showPassword" class="w-auto text-yellow-500 cursor-pointer">
            <svg v-if="showPassword" xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13.875 18.825A10.05 10.05 0 0112 19c-4.478 0-8.268-2.943-9.543-7a9.97 9.97 0 011.563-3.029m5.858.908a3 3 0 114.243 4.243M9.878 9.878l4.242 4.242M9.88 9.88l-3.29-3.29m7.532 7.532l3.29 3.29M3 3l3.59 3.59m0 0A9.953 9.953 0 0112 5c4.478 0 8.268 2.943 9.543 7a10.025 10.025 0 01-4.132 5.411m0 0L21 21" />
            </svg>
            <svg v-else xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z" />
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M2.458 12C3.732 7.943 7.523 5 12 5c4.478 0 8.268 2.943 9.542 7-1.274 4.057-5.064 7-9.542 7-4.477 0-8.268-2.943-9.542-7z" />
            </svg>
        </div>
      </div>
    </div>
    <div class="mx-12 p-3 justify-between flex">
      <div class="flex">
        <div class="relative inline-block w-12 mr-2 align-middle select-none transition duration-200 ease-in">
          <input type="checkbox" name="toggle" id="toggle" class="toggle-checkbox absolute block w-6 h-6 rounded-full bg-gray-800 border-4 appearance-none cursor-pointer" />
          <label for="toggle" class="toggle-label block overflow-hidden h-6 rounded-full bg-yellow-500 cursor-pointer"></label>
        </div>
        <label for="toggle" class="text-xs text-gray-300 mt-1">remeber me</label>
      </div>
      <div class="bg mt-1 text-xs text-gray-300">
        <nuxt-link to="/forget-password">forget password?</nuxt-link></div>
    </div>
    <div class="w-full p-12">
      <button class=" bg-yellow-500 p-3 rounded-3xl w-full h-full hover:bg-yellow-600"> Login</button>
      <p class="mx-auto text-center mt-3 text-gray-400">Don't have an account?  <nuxt-link to="signup" class="text-md font-semibold">Sign up</nuxt-link> </p>
    </div>
  </div>
</div>


</template>
<script>
export default {
    data() {
        return {
        showPassword: false
        }
    },
    methods: {

    }
}
</script>
