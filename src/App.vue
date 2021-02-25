<template>
<div
class="h-screen flex flex-row justify-center items-center space-x-8 text-center"
>
<card v-for="(l, k) of list" :key="k" :value="l"/>
</div>
 </template>

 <script>
     import card from "./components/card.vue";
 export default {
     components:{card},
     data(){
         return{
list:[
{
    texthover:'hover:text-white',
    link: 'https://www.google.com',
    image:'https://cdn.onlinewebfonts.com/svg/img_24577.png',
name: 'youtube',
descripcion: 'YouTube literalmente traduce al español como ‹tú tubo› . You ‹tú, usted› representa que el contenido es generado por el usuario y no por el sitio en sí, de ahí su eslogan "difunda tú mismo',
},
{
    link: 'https://www.google.com',
    color:'bg-blue-900',
    texthover:'hover:text-green-200',
    image:'https://www.logo.wine/a/logo/Microsoft_Office/Microsoft_Office-Logo.wine.svg',
name: 'office',
descripcion: 'una habitación, un conjunto de habitaciones o un edificio utilizado como lugar para trabajos comerciales, profesionales o burocráticos',
},
{
    link: 'https://www.google.com',
    color:'bg-green-400',
    texthover:'hover:text-white',
    image:'https://www.logo.wine/a/logo/Star_Wars/Star_Wars-Logo.wine.svg',
name: 'star wars',
descripcion: 'La trilogía de Star Wars: resumen completo. Estás aquí: La primera de la serie de tres partes, Star Wars, es la historia de una banda de héroes que se unen por el bien del universo y el dinero . La historia comienza cuando la Princesa Leia es rehén del Imperio Galáctico para aplastar la rebelión contra ellos.',
},
],
         };
     },
 };
 </script>
