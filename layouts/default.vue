<template>
  <div>
    <!-- <Navbar /> -->
    <Nuxt />
  </div>
</template>

// <script>
//  import Navbar from '@/components/Navbar'
//  export default {
//   components: {
//     Navbar
//   }
//  }
// </script>

<style>
.toggle-checkbox:checked {
  @apply: right-0 border-green-400;
  right: 0;
  border-color: rgb(241, 131, 4);
}
.toggle-checkbox:checked + .toggle-label {
  @apply: bg-green-400;
  background-color: rgb(241, 131, 4);
}
/* Change the white to any color */
input:-webkit-autofill,
input:-webkit-autofill:hover, 
input:-webkit-autofill:focus, 
input:-webkit-autofill:active
{
 -webkit-box-shadow: 0 0 0 30px #111827 inset !important;
}
/*Change text in autofill textbox*/
input:-webkit-autofill
{
 -webkit-text-fill-color: #F49E0A !important;
}
</style>