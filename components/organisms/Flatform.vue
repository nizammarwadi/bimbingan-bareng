<template>
    <section id="platform" class="platform">
        <div class="platform-title">
            <h2 class="title">Platform yang Didukung</h2>
            <p class="text">Ada dua platform yang didukung dan menjadi target pelayanan dari Bimbinganbareng, yaitu sebagai berikut</p>
        </div>
        <div class="website">
            <div class="website-image">
                <img src="~/assets/images/dekstop.png" style="width:350px; height: 320px;" alt="not found">
            </div>
            <div class="website-text">
                <h2 class="title">Website,<br> Dekstop Maupun Mobile</h2>
                <p class="text">Projek yang dihasilkan berupa website yang Kompatible dengan layar apapun (Dekstop, Mobile, maupun tablet)</p>
            </div>
        </div>
        <div class="mobile">
            <div class="mobile-text">
                <h2 class="title">Aplikasi Mobile,<br> Android</h2>
                <p class="text">Projek yang dihasilkan berupa aplikasi mobile yang dapat di gunakan di smartphone. Untuk saat ini masih mendukung environment<br> Android</p>
            </div>
            <div class="mobile-image">
                <img src="~/assets/images/phone.png" style="width:238px; height:458px;" alt="not found">
            </div>
        </div>
    </section>
</template>

<script>
export default {

}
</script>

<style>
    .platform {
        margin: 40px 0px;
        padding: 70px 0px 0px 0px;
    }
    .platform-title .title {
        margin: 0px auto;
        text-align: center;
        font-size: 27px;
        font-weight: 700;
        
    }
    .platform-title .text {
        font-size: 18px;
        font-weight: 450;
        margin: 0px auto;
        width: 700px;
        text-align: center;
        padding: 20px 0px;
    }
    .website {
        margin-top: 50px;
        display: flex;
        justify-content: space-evenly;
        align-items: center;
    }
    .website-text h2 {
        font-size: 27px;
        font-weight: 700;
        margin-bottom: 10px;
    }
    .website-text p {
        font-size: 17px;
        font-weight: 400;
        padding: 0px 0px;
        width: 400px;
    }
    .website-image img {
        object-fit: contain;
    }
    .mobile {
        margin-top: 100px;
        padding: 30px 0;
        display: flex;
        justify-content: space-evenly;
        align-items: center;
    }
    .mobile-image img {
        object-fit: contain;
    }
    .mobile-text h2 {
        font-size: 27px;
        font-weight: 700;
        margin-bottom: 10px;
    }
    .mobile-text p {
        font-size: 17px;
        font-weight: 400;
        padding: 0px 0px;
        width: 380px;
    }

    @media (max-width: 768px) {
        .website {
            display: block;
            width: 100%;
            margin: 0px 0px;
            padding: 0px 0px;
            text-align: center;
        }
        .website-text {
            text-align: left;
            padding: 0px 20px;
        }
        .website-text p{
            width: 100%;
        }
        .website-text .title {
            margin-bottom: 10px;
        }
        .mobile {
            display: block;
            width: 100%;
            margin: 0px 0px;
            padding: 0px 0px;
            text-align: center;
        }
         .mobile-text {
            text-align: left;
            padding: 0px 20px;
        }
        .mobile-text p {
            width: 100%;
        }
        .mobile-text .title {
            margin: 60px 0px 10px;
        }
        .platform-title .text {
            width: 100%;
            font-size: 16px;
            margin: 0px auto;
            text-align: center;
            padding: 10px 20px 0px;
        }
    }
    @media(max-width: 350px) {
        .website-image{
           width: 100%;
        }
        .website-image img{
            width: 200px!important;
        }
            
    }


</style>