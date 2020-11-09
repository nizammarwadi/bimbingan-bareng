<template>
    <nav class="navbar navbar-expand-lg navbar-light fixed-top">
        <div class="container">
            <a class="navbar-brand text-white" href="#">Bimbinganbareng.com</a>
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
                        <a class="nav-link js-scroll-trigger text-white" href="#Tentang KAmi">Tentang Kami</a>
                    </li>
                        <li class="nav-item">
                        <a class="nav-link js-scroll-trigger text-white" href="#Hubungi">Hubungi</a>
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
        }
    },
    mounted() {
        this.serviceSection = document.getElementById("service")
        this.benefitSection = document.getElementById("benefit")
        this.teknologiSection = document.getElementById("teknologi")
        this.flatformSection = document.getElementById("flatform")
    },
    methods: {
        toServiceSection() {
            this.serviceSection.scrollIntoView ({
                bahavior: "smooth",
                block: "start",
                inline: "nearest",
            })
        },
        toBenefitSection() {
            this.benefitSection.scrollIntoView({
                bahavior: "smooth",
                block: "start",
                inline: "nearest",
            })
        },
        toTeknologiSection() {
            this.teknologiSection.scrollIntoView({
                bahavior: "smooth",
                block: "start",
                inline: "nearest",
            })
        },
        toFlatformSection() {
            this.flatformSection.scrollIntoView({
                bahavior: "smooth",
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