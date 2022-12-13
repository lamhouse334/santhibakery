<template>
         <div class="grid grid-cols-2 gap-8 md:grid-cols-1 lg:grid-cols-4">
            <div>
                <h4 class="text-sm text-white leading-5 font-semibold tracking-wider text-white uppercase">
                    {{ menuitems.footer.sections[0].name }}
                </h4>
                <ul class="mt-4">
                    <li class="mt-4" v-for="sm in menuitems.footer.sections[0].menus" :key="sm.title">
                        <a :href="sm.link" class="text-base text-white leading-6 text-white hover:text-primary-500">
                            {{ sm.title }}
                        </a>
                    </li>
                </ul>
            </div>
            <!-- <div>
                <h4 class="text-sm leading-5 font-semibold tracking-wider text-white uppercase">
                    {{ menuitems.footer.sections[2].name }}
                </h4>
                <ul class="mt-4">
                    <li class="mt-4" v-for="sm in menuitems.footer.sections[2].menus" :key="sm.title">
                        <a :href="sm.link" class="text-base leading-6 text-white hover:text-primary-500">
                            {{ sm.title }}
                        </a>
                    </li>
                </ul>
            </div> -->
            
         </div>
         <div class="grid grid-cols-1">
          <div class="flex flex-col">
                <ContactUs />
            </div>
         </div>
         <div class="grid grid-cols-2">
           
       
                         
            <div class="mt-12 md:mt-0 md:min-w-64 lg:w-full">
                <iframe class="md:min-w-64" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3945.9731669881703!2d78.11618211513765!3d8.501985993887503!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3b039023b9f595fd%3A0x19bd9f170d10ceea!2sSanthi%20Bakery!5e0!3m2!1sen!2sin!4v1670832368745!5m2!1sen!2sin" 
                width="300" height="200" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade">
                </iframe>
            </div>
         </div>

</template>

<script>
import menuitems from "@/store/siteconfig.json";
export default {
    components: {

    },
    data() {
        return {
            menuitems
        };
    },
    methods: {

    }
}
</script>

