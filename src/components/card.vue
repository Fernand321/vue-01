<template>
 <div
     class="bg-red-500 border-t border-b flex flex-col  w-64  border-black py-12 px-9 space-y-5 "
     :class="[value.color, value.texthover]"

     >
  <img 
  :src="value.image"
  class="w-24 h-24 "
  /> 
  <span class="text-xl font-bold uppercase">{{value.name}}</span>
  <span
   class="text-center">{{value.descripcion}}</span>
  <a :href="value.link"
  target="blank" 
  class="bg-black hover:bg-gray-400 text-white py-2 px-12 rounded-full  "
  >
  visitar sitio
  
  </a>
  </div>
</template>

<script>
export default {
    props:["value"],
};
</script>