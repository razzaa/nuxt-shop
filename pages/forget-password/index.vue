<template>
<div class="h-screen w-full bg-gray-800">
  <div class="h-screen mx-auto max-w-screen-sm">
    <div class="p-12">
      <p class="text-5xl pt-10 text-yellow-500 font-bold">
        Welcome to
        Company
      </p>
      <p class="text-xl py-3 text-gray-400 font-semibold">Reset Password to continue</p>
    </div>
    <div class="mx-12 pl-3 pt-3 pr-3 pb-8 rounded-xl shadow-sm bg-gray-900">
      <div class="p-3 mx-6 border-b border-gray-500">
        <input placeholder="Phone Number or Email" class="bg-transparent text-yellow-500 w-full focus:outline-none focus:rang" type="tel" />
      </div>
    </div>
    <div class="w-full p-12">
      <button class=" bg-yellow-500 p-3 rounded-3xl w-full h-full hover:bg-yellow-600"> Submit</button>
      <p class="mx-auto text-center mt-3 text-gray-400">Have an account?  <nuxt-link to="signin" class="text-md font-semibold">Sign in</nuxt-link> </p>
    </div>
  </div>
</div>


</template>