<template>
    <NavBar/>
   <HomeComponent/>
   <AboutComponent/>
   <ResumeComponent/>
   <ProjectsComponent/>
   <TestimonialsComponent/>
   <ContactComponent/>
   <FooterComponent/>
   
</template>



<script>

import NavBar from '@/components/NavBar.vue'
import HomeComponent from '@/components/HomeComponent.vue'
import AboutComponent from '@/components/AboutComponent.vue'
import ResumeComponent from '@/components/ResumeComponent.vue'
import ProjectsComponent from '@/components/ProjectsComponent.vue'
import TestimonialsComponent from '@/components/TestimonialsComponent.vue'
import ContactComponent from '@/components/ContactComponent.vue'
import FooterComponent from '@/components/FooterComponent.vue'


export default {
    components: {
        NavBar,
        HomeComponent, 
        AboutComponent, 
        ResumeComponent, 
        ProjectsComponent, 
        TestimonialsComponent, 
        ContactComponent,
        FooterComponent
    }
    
}
</script>

<style scoped>
    
</style>