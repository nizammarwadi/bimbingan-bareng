<template>
    <section class="flowusers">
        <div class="flowusers-title">
            <h2>Flow Pelayanan User</h2>
        </div>
        <div class="flowusers-image">
            <div class="daptar" style="width: 130px; ">
                <img src="~/assets/images/daptar.png" alt="not found">
                <p>Daftar</p>
            </div>
            <div class="konsultasi" style="width: 130px; ">
                <img src="~/assets/images/konsultasi.png" alt="not found">
                <p>Konsultasi Projek</p>
            </div>
            <div class="negosiasi" style="width: 130px; ">
                <img src="~/assets/images/negosiasi.png" alt="not found">
                <p>Negosiasi</p>
            </div>
            <div class="pembayaran" style="width: 130px; ">
                <img src="~/assets/images/pembayaran.png" alt="not found">
                <p>Pembayaran</p>
            </div>
            <div class="mentoring" style="width: 130px; ">
                <img src="~/assets/images/mentoring.png" alt="not found">
                <p>Mentoring & Development</p>
            </div>
            <div class="mentoring" style="width: 130px; ">
                <img src="~/assets/images/selesai.png" alt="not found">
                <p>Selesai</p>
            </div>
            
        </div>
    </section>
</template>

<script>
export default {

}
</script>

<style>
    .flowusers {
        background-color: #A4DEF9;
        padding: 30px 0px;
        color: white;
    }
    .flowusers-title h2{
        text-align: center;
        font-size: 32px;
        font-weight: 700;
        width: 453px; 
        margin: 0px auto;
        padding: 20px 10px;
        
    }
    .flowusers-image {
        display: flex;
        justify-content: center;
        text-align: center;
        padding: 30px 0px;
               
    }

    .flowusers-image p{
        margin-top: 20px;
        font-size: 16px;
        font-weight: 700;
    }
    @media(max-width: 768px) {
        .flowusers-title h2 {
            width: 100%;
            margin: 0px 0px 20px;
            padding: 0px 0px;
        }
        .flowusers-image {
            width: 100%;
            margin: 0px 0px;
            padding: 0px 0px;
        }
        .flowusers-image img {
            width: 40px;
            margin: 0px 0px;
            padding: 0px 0px;   
        }
        .flowusers-image p {
            font-size: 10px;
            margin: 10px 0px;
        }
       
    }

</style>