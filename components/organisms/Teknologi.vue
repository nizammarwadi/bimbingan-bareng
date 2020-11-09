<template>
    <section id="teknologi" class="teknologi">
        <div class="teknologi-title">
            <h2 class="title">Teknologi yang Digunakan</h2>
            <p class="text">Bimbinganbareng menggunakan dan stack yang paling banyak digunakan di dunia kerja dan Startup,diantaranya sebagai berikut</p>
        </div>
        <div class="teknologi-images">
            <div class="vue">
                <img src="~/assets/images/vue.png" style="width:70px;" alt="not found">
            </div>
            <div class="react">
                <img src="~/assets/images/react.png" style="width:150px;" alt="not found">
                
            </div>
            <div class="node">
                <img src="~/assets/images/node.png" alt="not found">
                
            </div>
            <div class="golang">
                <img src="~/assets/images/golang.png" style="width:90px;" alt="not found">
                
            </div>
            <div class="python">
                <img src="~/assets/images/python.png" style="width:70px;" alt="not found">
                
            </div>
        </div>
    </section>
</template>

<script>
export default {

}
</script>

<style>
    .teknologi {
        margin-top: 100px;
        background-color: #F8F9FA;
        padding: 40px 0px;
        
    }
    .teknologi-title .title{
        width: 600px;
        margin: 0px auto;
        text-align: center;
        font-size: 27px;
        font-weight: 700;
        padding-bottom: 10px;
    }
    .teknologi-title .text {
        width: 600px;
        margin: 0px auto;
        text-align: center;
        font-size: 18px;
        font-weight: 450;
    }
    .teknologi-images {
        margin-top: 50px;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    

    /* mobile */
    @media(max-width: 768px) {
        
        .teknologi-title .title {
            width: 100%;
            margin: 0px 0px;
            padding: 0px 0px;
        }
        .teknologi-title .text {
            width: 100%;
            margin: 10px 0px 0px;
            padding: 0px 20px;
            font-size: 16px;
        }
        .teknologi-images {
            display: block;
            width: 100%;
            text-align: center;
        }
    }
   
        
    

 

</style>