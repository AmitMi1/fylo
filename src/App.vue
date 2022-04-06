<template>
  <section>
   <main-header></main-header>
   <main-intro></main-intro>
   <amenity-list :amenities="amenityList"></amenity-list>
  <main-content></main-content>
  <testi-list :testimonialList="testimonialList"></testi-list>
  </section>
</template>

<script>
import mainHeader from "./components/main-header.vue"
import mainIntro from "./components/main-intro.vue"
import amenityList from "./components/amenity-list.vue"
import mainContent from "./components/main-content.vue"
import testiList from "./components/testi-list.vue"


export default {
  name: 'app-vue',
  components: {
    mainHeader,
    mainIntro,
    amenityList,
    mainContent,
    testiList
  },
  data(){
    return{
      amenityList: [
        {
          imgUrl: 'https://res.cloudinary.com/amit-mizrahi/image/upload/v1649263665/icon-access-anywhere_qdb4hv.svg',
          title: 'Access your files, anywhere',
          txt: 'The ability to use a smartphone, tablet, or computer to access your account means your files follow you everywhere.'
        },
        {
          imgUrl: 'https://res.cloudinary.com/amit-mizrahi/image/upload/v1649263797/icon-security_ofic3d.svg',
          title: 'Security you can trust',
          txt: '2-factor authentication and user-controlled encryption are just a couple of the security features we allow to help secure your files.'
        },
        {
          imgUrl: 'https://res.cloudinary.com/amit-mizrahi/image/upload/v1649263674/icon-collaboration_chjylw.svg',
          title: 'Real-time collaboration',
          txt: 'Securely share files and folders with friends, family and colleagues for live collaboration. No email attachments required.'
        },
        {
          imgUrl: 'https://res.cloudinary.com/amit-mizrahi/image/upload/v1649263665/icon-any-file_mzpfty.svg',
          title: 'Store any type of file',
          txt: `Whether you're sharing holidays photos or work documents, Fylo has you covered allowing for all file types to be securely stored and shared.`
        },
      ],
      testimonialList: [
        {
        txt: 'Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.',
       userImg: 'https://res.cloudinary.com/amit-mizrahi/image/upload/v1649263720/profile-1_hxaytz.jpg',
        fullname: 'Satish Patel',
        userTitle: 'Founder & CEO, Huddle'
        },
        {
        txt: 'Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.',
       userImg: 'https://res.cloudinary.com/amit-mizrahi/image/upload/v1649263720/profile-2_rh0kxb.jpg',
        fullname: 'Bruce McKenzie',
        userTitle: 'Founder & CEO, Huddle'
        },
        {
        txt: 'Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.',
       userImg: 'https://res.cloudinary.com/amit-mizrahi/image/upload/v1649263720/profile-3_egp1y6.jpg',
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