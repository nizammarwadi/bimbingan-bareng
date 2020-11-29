<template>
    <section id="teknologi" class="teknologi">
        <div class="teknologi-title">
            <h2 class="title">Teknologi yang Digunakan</h2>
            <p class="text">Bimbinganbareng menggunakan teknologi dan stack yang paling banyak digunakan di dunia kerja dan Startup,diantaranya sebagai berikut</p>
        </div>
        <div class="teknologi-images">
            <div class="vue">
                <img src="~/assets/images/vue.png" alt="not found">
                <p>Vue Js</p>
            </div>
            <div class="react">
                <img src="~/assets/images/react.png" alt="not found">
                <p>React Js React Native</p>
                
            </div>
            <div class="node">
                <img src="~/assets/images/node.png" alt="not found">
                <p>Node Js</p>
                
            </div>
            <div class="golang">
                <img src="~/assets/images/golang.png" alt="not found">
                <p>Golang</p>
                
            </div>
            <div class="python">
                <img src="~/assets/images/python.png" alt="not found">
                <p>Phyton</p>
                
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
        padding: 70px 0px 40px 0px;
        
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
        text-align: center;
        font-weight: 700;
    }
    .vue img {
        margin: 25px 0px 30px;
        width:70px;
    }
    .vue {
        width: 80px;
    }
    .node {
        width: 230px;
    }
    .react {
        width: 160px;
    }
    .golang{
        margin: 0px 20px;
        width: 100px;
    }
    .python{
        width: 100px;
    }
    .golang img {
        margin: 10px 0px 20px;
        width:90px;
    }
    .python img {
        margin: 20px 0px 30px;
        width:70px;
    }
    .react img {
        margin-bottom: 15px;
        width:150px
    }
    .react p{
        width: 100px;
        margin: 0px auto;
    }
    .node img {
        margin-bottom: 10px;
    }
    @media (max-width: 768px) {
        .teknologi {
            margin: 0px 0px;
        }
        .teknologi-title .text {
            width: 100%;
            margin: 0px 0px;
            padding: 0px 20px;
            font-size: 16px;
        }
        .teknologi-title .title {
            width: 100%;
            margin: 0px 0px 10px 0px;
            padding: 0px 0px;
        }
        .teknologi-images {
            width: 100%;
            margin: 0px 0px;
            padding: 30px 10px;
        }
        .vue {
            width: 100%;
            margin: 0px 0px 0px;
            padding: 0px 0px;
        }
        .react {
            width: 100%;
            margin: 0px 0px;
            padding: 0px 0px;
        }
        .node {
            width: 100%;
            margin: 0px 0px;
            padding: 0px 0px;
        }
        .golang {
            width: 100%;
            margin: 0px 0px;
            padding: 0px 0px;
        }
        .python {
            width: 100%;
            margin: 0px 0px;
            padding: 0px 0px;
        }
        .vue img {
            width: 40px;
            margin: 23px auto 19px;
            padding: 0px 0px;
        }
        .react img {
            width: 110px;
            margin: 0px auto 3px;
            padding: 0px 0px;
        }
        .node img {
            width: 70px;
            margin: 20px auto 23px;
            padding: 0px 0px;
        }
        .golang img {
            width: 50px;
            margin: 18px auto 10px;
            padding: 0px 0px;
        }
        .python img {
            width: 45px;
            margin: 20px auto 15px;
            padding: 0px 0px;
        }
        .teknologi-images p {
            font-size: 11px;
        }
    }
    

    /* untuk ukuran vertical */
    /* @media(max-width: 768px) {
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
        .vue {
            width: 100%;
            margin: 0px auto;
        }
        .react {
            width: 100%;
            margin: 0px auto;
        }
        .node {
            width: 100%;
            margin: 0px auto;
        }
        .golang {
            width: 100%;
            margin: 0px auto;
        }
        .python {
            width: 100%;
            margin: 0px auto;
        }
    } */
   
        
    

 

</style>