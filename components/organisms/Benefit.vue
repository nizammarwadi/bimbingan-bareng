<template>
    <section id="benefit" class="benefit">
        <div class="first-benefit">
            <div class="first-benefit-content">
                <div class="first-benefit-left">
                    <img src="~/assets/images/graduation.png" alt="not found">
                </div>
                <div class="first-benefit-right">
                    <h2>Lebih Mudah Menyelesaikan Tugas Akhir</h2>      
                    <p>Sebagai mentor dan pembimbing, Bimbinganbareng membantu kamu dari sisi teknikal dalam menyelesaikan projek kamu</p>
                </div>
            </div>
        </div>
        <div class="second-benefit">
            <div class="second-benefit-content">
                <div class="second-benefit-left">
                    <img src="~/assets/images/coding.png" alt="not found">
                </div>
                <div class="second-benefit-right">
                    <h2>Hardskill Sofware Development Website dan Aplikasi Mobile</h2>      
                    <p>Dengan Menggunakan Layanan Bimbinganbareng, selain kamu dibantu menyelesaikan projek, kamu akan dimentoring tentang proses development sebuah Website ataupun Aplikasi Mobile</p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {

}
</script>

<style>
    /* fist-benefit */
    .benefit {
        margin-top: 30px;
        padding-top: 70px;
    }
    .first-benefit-content {
        background-color: #F8F9FA;
        width: 90%;
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 40px 0px;
    }
    .first-benefit-left {
        margin-left: 200px;
    }
    .first-benefit-right {
        width: 500px;
        padding: 10px 20px 10px 40px;
    }
    .first-benefit-right h2 {
        font-weight: 700;
        font-size: 27px;
    }
    .first-benefit-right p {
        margin-top: 15px;
        font-size: 18px;
        font-weight: 400;
        width: 380px;
    }

    /* second-benefit */
    .second-benefit-content {
        background-color: #F8F9FA;
        margin-top: 60px;
        width: 90%;
        margin-left: 10%;
        display: flex;
        align-items: center;
        justify-content: space-around;
        padding: 40px 0px;
    }
    .second-benefit-right {
        width: 550px;
        padding: 10px 80px 10px 30px;    
    }
    .second-benefit-right h2 {
        font-weight: 700;
        font-size: 27px;
    }
    .second-benefit-right p {
        margin-top: 15px;
        font-size: 18px;
        font-weight: 400;
    }

    @media(max-width: 992px) {
        .benefit {
            width: 100%;
            margin-top: 30px;
            padding: 70px 20px;
            background-color: #f8f9fa;
        }
        .first-benefit {
            width: 100%;
            margin: 0px 0px;
            padding: 0px 0px;
        }
        .first-benefit-content {
            display: block;
            width: 100%;
            margin: 0px 0px;
            padding: 0px 0px;
        }
        .first-benefit-left {
            width: 80%;
            margin: 0px auto;
            padding: 0px 0px;
        }
        .first-benefit-left img {
            width: 100%;
            margin: 0px 0px;
            padding: 0px 0px;
            text-align: center;
        }
        .first-benefit-right {
            width: 100%;
            padding: 40px 20px 0px;
        }
        .first-benefit-right p {
            width: 100%;
            margin: 0px 0px;
            padding: 0px 0px;
        }
        
        /* @media second-benefit */
         .second-benefit {
            width: 100%;
            margin: 0px 0px;
            padding: 0px 0px;
        }
        .second-benefit-content {
            display: block;
            width: 100%;
            margin: 0px 0px;
            padding: 0px 0px;
        }
        .second-benefit-left {
            width: 100%;
            margin: 0px 0px;
            padding: 0px 0px;
        }
        .second-benefit-left img {
            width: 100%;
            margin: 0px 0px;
            padding: 0px 0px;
            text-align: center;
        }
        .second-benefit-right {
            width: 100%;
            margin: 0px 0px;
            padding: 0px 20px;
        }
    
    }
    

</style>