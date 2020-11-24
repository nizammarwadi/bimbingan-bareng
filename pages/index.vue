<template>
    <div>
      <Navbar/>
      <Intro/>
      <Service/>
      <Benefit/>
      <Teknologi/>
      <Platform/>
      <FlowUser/>
      <Registrasi/>
      <Footer/>
    </div>
</template>
<script>
import Navbar from "~/components/organisms/Navbar.vue"
import Intro from "~/components/organisms/Intro.vue"
import Service from "~/components/organisms/service.vue"
import Benefit from "~/components/organisms/Benefit.vue"
import Teknologi from "~/components/organisms/Teknologi.vue"
import Platform from "~/components/organisms/Platform.vue"
import FlowUser from "~/components/organisms/FlowUser.vue"
import Registrasi from "~/components/organisms/Registrasi.vue"
import Footer from "~/components/organisms/Footer.vue"
export default {
    components: {
      Navbar: Navbar, 
      Intro: Intro,
      Service: Service,
      Benefit: Benefit,
      Teknologi: Teknologi,
      Platform: Platform,
      FlowUser: FlowUser,
      Registrasi: Registrasi,
      Footer: Footer,
    }
}
</script>

<style>

</style>