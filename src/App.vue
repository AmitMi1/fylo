<template>
  <section>
   <main-header></main-header>
   <main-intro></main-intro>
   <amenity-list :amenities="amenityList"></amenity-list>
  <main-content></main-content>
  <testi-list :testimonialList="testimonialList"></testi-list>
  <main-starter></main-starter>
  <main-footer></main-footer>
  </section>
</template>

<script>
import mainHeader from "./components/main-header.vue"
import mainIntro from "./components/main-intro.vue"
import amenityList from "./components/amenity-list.vue"
import mainContent from "./components/main-content.vue"
import testiList from "./components/testi-list.vue"
import mainFooter from "./components/main-footer.vue"
import mainStarter from "./components/main-starter.vue"


export default {
  name: 'app-vue',
  components: {
    mainHeader,
    mainIntro,
    amenityList,
    mainContent,
    testiList,
    mainFooter,
    mainStarter
  },
  data(){
    return{
      amenityList: [
        {
          imgUrl: new URL('assets/images/icon-access-anywhere.svg', import.meta.url).href,
          title: 'Access your files, anywhere',
          txt: 'The ability to use a smartphone, tablet, or computer to access your account means your files follow you everywhere.'
        },
        {
          imgUrl: new URL('assets/images/icon-security.svg', import.meta.url).href,
          title: 'Security you can trust',
          txt: '2-factor authentication and user-controlled encryption are just a couple of the security features we allow to help secure your files.'
        },
        {
          imgUrl: new URL('assets/images/icon-collaboration.svg', import.meta.url).href,
          title: 'Real-time collaboration',
          txt: 'Securely share files and folders with friends, family and colleagues for live collaboration. No email attachments required.'
        },
        {
          imgUrl: new URL('assets/images/icon-any-file.svg', import.meta.url).href,
          title: 'Store any type of file',
          txt: `Whether you're sharing holidays photos or work documents, Fylo has you covered allowing for all file types to be securely stored and shared.`
        },
      ],
      testimonialList: [
        {
        txt: 'Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.',
       userImg: new URL('assets/images/profile-1.jpg', import.meta.url).href,
        fullname: 'Satish Patel',
        userTitle: 'Founder & CEO, Huddle'
        },
        {
        txt: 'Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.',
       userImg: new URL('assets/images/profile-2.jpg', import.meta.url).href,
        fullname: 'Bruce McKenzie',
        userTitle: 'Founder & CEO, Huddle'
        },
        {
        txt: 'Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.',
       userImg: new URL('assets/images/profile-3.jpg', import.meta.url).href,
        fullname: 'Iva Boyd',
        userTitle: 'Founder & CEO, Huddle'
        },
      ]
    }
  }


}
</script>

<style>

</style>