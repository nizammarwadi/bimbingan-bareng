<template>
    <nav id="navbar" class="navbar navbar-expand-lg navbar-light fixed-top">
        <div class="container">
            <a class="navbar-brand text-white" href="https://wa.me/6282362574353?text=Oops...%0AJangan%20galau%20dan%20resah%2C%20kita%20siap%20bantu%20Bro%20and%20Sist%20...%0ASelamat%20datang%20di%20Bimbinganbareng.com%0A" target="_blank">Bimbinganbareng.com</a>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ml-auto">
                    <li class="nav-item active">
                        <a class="nav-link text-white" @click="toServiceSection">Layanan <span class="sr-only">(current)</span></a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link js-scroll-trigger text-white" @click="toBenefitSection">Keuntungan</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link js-scroll-trigger text-white" @click="toTeknologiSection">Teknologi</a>
                    </li>
                        <li class="nav-item">
                        <a class="nav-link js-scroll-trigger text-white" @click="toFlatformSection">Platform</a>
                    </li>
                        <li class="nav-item">
                        <a class="nav-link js-scroll-trigger text-white"  @click="toFooterSection">Tentang Kami</a>
                    </li>
                        <li class="nav-item">
                        <a class="nav-link js-scroll-trigger text-white" href="https://wa.me/6282362574353?text=Selamat%20Datang%20di%20Bimbinganbareng.com.%0AApa%20masalah%20bro and sist%3F%20ayo%20cerita%20....%0A" target="_blank">Hubungi</a>
                    </li>
                </ul>
            </div>
        </div>  
    </nav>
</template>

<script>
export default {
    data() {
        return {
            serviceSection: "",
            benefitSection: "",
            teknologiSection: "",
            flatformSection: "",
            footerSection: "",
        };
    },
    mounted() {
        this.serviceSection = document.getElementById("service");
        this.benefitSection = document.getElementById("benefit");
        this.teknologiSection = document.getElementById("teknologi");
        this.flatformSection = document.getElementById("flatform");
        this.footerSection = document.getElementById("footer");
    },
    methods: {
        hideMenu() {
            let menuContainer = document.getElementById("navbarNav");
            menuContainer.classList.remove("show");
        },
        toServiceSection() {
            this.serviceSection.scrollIntoView ({
                behavior: "smooth",
                block: "start",
                inline: "nearest",
            });
            this.hideMenu()
        },
        toBenefitSection() {
            this.benefitSection.scrollIntoView({
                behavior: "smooth",
                block: "start",
                inline: "nearest",
            });
            this.hideMenu()
        },
        toTeknologiSection() {
            this.teknologiSection.scrollIntoView({
                behavior: "smooth",
                block: "start",
                inline: "nearest",
            });
        },
        toFlatformSection() {
            this.flatformSection.scrollIntoView({
                behavior: "smooth",
                block: "start",
                inline: "nearest",
            });
        },
        toFooterSection() {
            this.footerSection.scrollIntoView({
                behavior: "smooth",
                block: "start",
                inline: "nearest",
            })
        }
    }
}
</script>

<style>
    .navbar {
        background-color: #A4DEF9;
        font-size: 16px;
        font-weight: 700;   
    }
    .navbar-nav {
        cursor: pointer;
    }
    
</style>