<template>
<main
		class="mx-auto bg-gradient-to-r from-primary-800 via-primary-900 to-primary-800 ... lg:max-w-8xl px-5 lg:px-0 pt-14 lg:pt-12 aboutbg">
		<h1 class="capitalize font-semibold text-[38px] lg:text-7xl text-center leading-snug text-white">			
			
			<span class="font-extrabold bg-clip-text text-primary-50 uppercase">About</span>
		</h1>
		
		<div class="text-center p-10 flex items-center justify-center space-x-4">
			<NuxtLink to="#" @click="useNuxtApp().$bus.$emit('evtShowContactSales')"
				class="px-5 py-2 text-sm  ring-2 ring-primary-500 hover:bg-primary-700 ring-inset text-white rounded-full transition-all duration-300">
				Contact us</NuxtLink>
			<!--<div class="relative group">
				<div
					class="absolute -inset-0.5 bg-gradient-to-r from-secondary-600 to-primary-600 rounded-lg blur opacity-75 group-hover:opacity-100 transition duration-1000 group-hover:duration-200 animate-tilt">
				</div>
				<button @click="useNuxtApp().$bus.$emit('evtShowContactSales')"
					class="relative px-7 py-4 bg-black rounded-lg leading-none flex items-center divide-x divide-gray-600">
					<span class="flex items-center space-x-5">
						<span class="pr-6 font-medium text-white">Contact us</span>
					</span>
				</button>
			</div>

			<NuxtLink
				to="#"
				class="text-sm group overflow-hidden relative bg-gray-50 ring-1 hover:ring-transparent ring-gray-300 rounded-full transition-all duration-300"
			>
				<div
					class="absolute h-full w-0 group-hover:w-full transition-all duration-500 bg-primary-700"
				></div>
				<span
					class="block px-6 py-3 transition-all duration-500 group-hover:text-white relative"
					>Take Tour</span
				>
			</NuxtLink>-->
		</div>
	</main>
  <div class="max-w-7xl mx-auto mt-16 my-16 lg:grid lg:grid-cols-2 md:flex md:flex-col">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
     <img src="https://res.cloudinary.com/lamcom/image/upload/v1670772073/santhibakery/home/Web_Photo_Editor_1_plkgqq.jpg">
     <div class="box-content bg-primary-900 mt-2 w-full h-25 rounded-lg">
     <p class="text-center p-10 text-white font-semibold text-xl ">We Bake to your taste</p>
     </div>
      </div>
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="lg:text-center md:text-center">
        <h2 class="text-base text-primary-700 font-semibold tracking-wide uppercase">About Us</h2>
        <p class="mt-2 text-3xl leading-8 font-extrabold tracking-tight text-gray-900 sm:text-4xl">
         OUR MOTTO
        </p>
        <!-- <p class="mt-4 max-w-2xl text-xl text-gray-500 lg:mx-auto md:mx-auto">
          LAM House symbolises Brilliance, Reliability and Integrity
        </p> -->
      </div>

      <div class="mt-10">
        <dl class="space-y-10 md:space-y-0 md:grid md:gap-y-10">
          <div v-for="about in about" :key="about.name" class="relative">
            <dt>
              <div class="absolute flex items-center justify-center h-12 w-12 rounded-md bg-primary-900 text-white">
                <component :is="about.icon" class="h-6 w-6" aria-hidden="true" />
              </div>
              <p class="ml-16 text-lg leading-6 font-medium text-gray-900">{{ about.name }}</p>
            </dt>            
          </div>
        </dl>
      </div>      
    </div>
  </div>

  <!-- <div class="max-w-7xl mx-auto mt-16 my-16 lg:grid">
     <div class="max-w-7xl px-4 sm:px-6 lg:px-8">
      <div class="lg:text-left md:text-left">
        <h2 class="text-base text-indigo-600 font-semibold tracking-wide uppercase">About Us</h2>
        <p class="mt-2 text-3xl leading-8 font-extrabold tracking-tight text-gray-900 sm:text-4xl">
         The Name and Legacy
        </p>        
      </div>
   </div>
     <div class="mt-10 max-w-7xl">
        <dl class="space-y-10 md:space-y-0 md:grid md:gap-y-10">
          <div v-for="legacy in legacy" :key="legacy.name" class="relative">
            <dt>
              <div class="absolute flex items-center justify-center h-12 w-12 rounded-md bg-indigo-500 text-white">
                <component :is="legacy.icon" class="h-6 w-6" aria-hidden="true" />
              </div>
              <p class="ml-16 text-lg leading-6 font-medium text-gray-900">{{ legacy.name }}</p>
            </dt>            
          </div>
        </dl>
      </div> 
   </div> -->

   
  
  
</template>

<script>
import { AnnotationIcon, GlobeAltIcon, LightningBoltIcon, ScaleIcon, ArrowCircleRightIcon } from '@heroicons/vue/outline/index.js'
definePageMeta({
  //colorMode: 'system',
  layout: "main",
})
const about = [
  {
    name: 'We Strive to bring out tasty and palatable bakery items which include cakes,buns,puffs,etc.,to the entire satisfaction of our customers.',    
    icon: ArrowCircleRightIcon,
  },
  {
    name: "SANTHI BAKERY plans to create innovations and professional expertise to meet the customer's immediate and future requirements.Our food mall is A/C and NON A/C, providing 100% vegetarian food items.",    
    icon: ArrowCircleRightIcon,
  },
  {
    name: "We value our customer's patronage for the most clean, hygiene and economical quality products to suite every family's taste. Consistency in the products is our speciality.",    
    icon: ArrowCircleRightIcon,
  },
  {
    name: "We also arrange kitty parties, Birthday, Anniversary and other events to the customer's fullest satisfaction. We also use the latest equipments and technology in the production of our bakery and food items.",   
    icon: ArrowCircleRightIcon,
  },
  {
    name: "Customers satisfaction is our main motto. Please contact us at 9965838485.We remain always at your service.",   
    icon: ArrowCircleRightIcon,
  },
]

// // const legacy = [
// //   {
// //     name: 'The name LAM House is inspired by and dedicated to my parents and family. LAM is an acronym for Life, Art and Multimedia.',    
// //     icon: ArrowCircleRightIcon,
// //   },
// //   {
// //     name: 'Mr. Muthuraman A. as the proprietor of this company brings along with him over 20 years of experience in the fields of animation and graphic design. From managerial roles, to HR roles to administrative details to the financial aspects of a graphic designing and software development firm. In the past years he has grown and groomed our team to reflect these qualities of integrity and dedication in their work.',    
// //     icon: ArrowCircleRightIcon,
// //   },  
// ]
export default {
  setup() {
    return {
      about,
      // legacy,     
    }   
  },
 
}
</script>
<style scoped src="@/assets/css/newstyle.css"></style>
