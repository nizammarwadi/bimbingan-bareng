<template>
    <section id="service" class="service">
        <div class="service-title">
            <p class="service-title-top">Pelayanan yang diberikan</p>
            <p class="service-title-bottom">Ada beberapa kategori projek website dan aplikasi mobile yang kami layani, diantaranya sebagai berikut</p>
        </div>
        <div class="service-content">
            <div class="service-card">
                <img src="~/assets/images/vector1.png" alt="not found">
                <p>Bimbingan Projek Website atau Aplikasi Mobile untuk Tugas Akhir</p>
            </div>

        
            <div class="service-card">
                <img src="~/assets/images/vector2.png" alt="not found">
                <p>Membantu dan Mentoring Penelitian berupa Website dan Aplikasi Mobile</p>
            </div>

            <div class="service-card">
                <img src="~/assets/images/vector3.png" alt="not found">
                <p>Tugas dan Projek Kampus berupa Website dan Mobile Aplikasi</p>
            </div>
        </div>
    </section>
</template>

<script>
export default {

}
</script>

<style>
    .service{
        margin-top: 0px;
        padding: 70px 0px 0px 0px;
        margin-bottom: 50px;
    }
    .service-title .service-title-top {
        font-weight: 700;
        font-size: 27px;
        font-style: normal;
        margin-bottom: 10px;
    }
    .service-title .service-bottom {
        width: 655px;
        margin: 0px auto;
        font-size: 22px;
        font-weight: 400;
    }
    .service-card img{
        width: 76px;
        height: 53px; 
        margin-right: 15px; 
        object-fit: contain;    
        padding-top: 5px;
    }
    .service-title{
        text-align: center;
    }
    .service-content {
        margin-top: 50px;
        display: flex;
        justify-content: space-evenly;
    }
    .service-card{
        display: flex;
        box-shadow: inset 0px -3px 5px rgba(0, 0, 0, 0.25);
        border-radius: 30px;
        padding: 45px 24px;  
        line-height: 20px;
        width: 335px;
        height: 165px;
        font-size: 15px;
        font-weight: 700;  
    }
    @media(max-width: 768px) {
        .service {
            width: 100%;
            margin: 0px 0px;
            padding-top: 80px;
        }
        .service-title .service-title-top {
            margin: 0px 0px 10px 0px;
            padding: 0px 0px;
            width: 100%;
        }
        .service-title .service-title-bottom {
            width: 80%;
            margin: 0px auto;
            padding: 0px 0px;
        }
        .service-content {
            display: block;
            width: 90%;
            margin: 20px auto;
        }
        .service-card {
            width: 100%;
            margin: 10px 0px;
        }
        
       
    }
    
    



</style>