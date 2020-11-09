<template>
<section class="benefit">
    <div class="benefit-content">
        <div class="benefit-image">
            <img src="~/assets/images/graduation.png" style="width: 373px;" alt="not found">
        </div>
        <div class="benefit-tutorial">
            <h2>Lebih Mudah Menyelesaikan Tugas Akhir</h2>      
            <p>Sebagai mentor dan pembimbing, Bimbinganbareng membantu kamu dari sisi teknikal dalam menyelesaikan projek kamu</p>
        </div>
    </div>
</section>

</template>

<script>
export default {

}
</script>

<style>
    .benefit {
        padding: 40px 0px;
        width: 85%;
        background-color: #F8F9FA;
    }
    .benefit-content {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }
    .benefit-image{
        margin-left: 120px;
    }
    .benefit-tutorial {
        width: 500px;
        padding: 0px 30px;
    }
    .benefit-tutorial h2 {
        font-weight: 700;
    }
    .benefit-tutorial p {
        margin-top: 25px;
        font-size: 19px;
        font-weight: 400;
    }
    @media(max-width: 768px) {
        .benefit-content {
            display: block;
        }
        .benefit-tutorial {
            margin-top: 50px;
            
        }
        .benefit-image {
            margin-right: 120px;
        }
    }
</style>