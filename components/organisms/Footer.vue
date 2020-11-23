<template>
    <footer>
        <section id="footer" class="footer">
            <div class="container">
                <div class="row">
                    <div class="col-md-5 col-sm-6 about-us">
                        <div class="about-us-title">
                            <h5>Bimbinganbareng.id</h5>
                        </div>
                        <p>Bimbinganbareng.id adalah jenis layanan jasa membing dan mentoring kebutuhan penyelesaian projek berupa Tugas Akhir. Tugas Kampus maupun Penelitian dengan
                            tujuan memberikan bekal hardskill yang mumpuni untuk mereka agar lebih cepat dan lebih mudah dalam menyelesaikan projeknya 
                        </p>
                        
                    </div>
                    <div class="col-md-5 col-sm-6 contact-us">
                        <div class="contact-us-mediasosial">
                            <h5>Media Sosial</h5>
                            <a href="https://www.instagram.com/bimbinganbareng/"><img class="ig" src="~/assets/images/ig.png" alt="not found"></a>
                            <a href="https://www.facebook.com/nizam.marwadi/"><img class="fb" src="~/assets/images/fb.png" alt="not found"></a>
                        </div>
                        <div class="contact-us-address">
                            <h5>Alamat</h5>
                            <p>Jl. Letda Sujono No. 273, Medan Tembung <br>Medan, Sumatera Utara</p>
                        </div>
                        <div class="contact-us-call">
                            <h5>Hubungi Kami</h5>
                            <div class="call-number">
                                <a href="https://wa.me/6282362574353?text=Oops...%0AJangan%20galau%20dan%20resah%2C%20kita%20siap%20bantu%20Bro%20and%20Sist%20...%0ASelamat%20datang%20di%20Bimbinganbareng.com%0A" target="_blank"><img src="~/assets/images/call.png" alt="not found"></a>
                                <p><a href="https://wa.me/6282362574353?text=Oops...%0AJangan%20galau%20dan%20resah%2C%20kita%20siap%20bantu%20Bro%20and%20Sist%20...%0ASelamat%20datang%20di%20Bimbinganbareng.com%0A" target="_blank">0823-6257-4353</a></p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        <section class="patent">
            <p>©Copyright 2020 Bimbinganbareng.id</p>
        </section>
    </footer>
    
</template>

<script>
export default {

}
</script>

<style>
    .footer{
        background-color: #F8F9FA;
        color: #131;
        padding: 80px 0px;
    }
    .row {
        justify-content: space-between;
        align-items: flex-start;  
    }
    .about-us {
        font-size: 18px;
    }
    .contact-us{
        text-align: left;
    }
    .about-us-title h5 {
        font-size: 20px;
        font-weight: 700;
    }
    .contact-us-address p{
        font-size: 16px;
    }
    .about-us p{
        font-size: 16px;
    }
    .contact-us-mediasosial h5 {
        font-weight: bold;
    }
    .ig {
        object-fit: cover;
    }
    .fb {
        object-fit: contain;
    }
    .contact-us-address h5{
        margin-top: 20px;
        font-weight: bold;
    }
    .contact-us-call h5 {
        font-weight: bold;
        margin-top: 20px;
    }
    .call-number img {
        margin-right: 20px;
        object-fit: cover;
    }
    .call-number {
        font-weight: 700;
        margin-top: 15px;
        display: flex;
        justify-content: left;
        align-items: flex-end;
    }
   
    
    /* .about-us .about-us-title h4::after {
        content: '_____';
        display: block;
        color: #4abeed;
        font-size: 30px;
        margin: -10px 0px 15px 0px;
    }
    .contact-us .contact-us-title h4::after{
        content: '_____';
        display: block;
        color: #4abeed;
        font-size: 30px;
        margin: -10px 0px 15px 0px;
    }
    .email-us .email-us-title h4::after{
        content: '_____';
        display: block;
        color: #4abeed;
        font-size: 30px;
        margin: -10px 0px 15px 0px;
    } */
    /* .phone{
        list-style-type: none;
        
    } */
    .patent{
        /* border-top: 1px solid #bbb; */
        background-color:#E2E2E2;
        text-align: left;
    }
    .patent p{
        font-size: 16px;
        font-weight: 700;
        padding: 15px;
        margin-left: 100px;
        color: #0B090A;
    }
    @media(max-width: 578px) {
        .contact-us, .email-us{
            margin-top: 30px;
        }
        .patent p {
            width: 100%;
            margin: 0px 0px;
            padding-left:  30px;
            font-size: 12px;
        }
        .row {
            padding: 0px 20px;
        }
    }
</style>