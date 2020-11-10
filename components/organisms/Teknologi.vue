<template>
    <section id="teknologi" class="teknologi">
        <div class="teknologi-title">
            <h2 class="title">Teknologi yang Digunakan</h2>
            <p class="text">Bimbinganbareng menggunakan dan stack yang paling banyak digunakan di dunia kerja dan Startup,diantaranya sebagai berikut</p>
        </div>
        <div class="teknologi-images">
            <div class="vue" style="width: 80px">
                <img src="~/assets/images/vue.png" style="width:70px;" alt="not found">
                <p>Vue.js</p>
            </div>
            <div class="react" style="width:160px">
                <img src="~/assets/images/react.png" style="width:150px;" alt="not found">
                <p>React Js React Native</p>
                
            </div>
            <div class="node" style="width: 230px">
                <img src="~/assets/images/node.png" alt="not found">
                <p>Node.js</p>
                
            </div>
            <div class="golang" style="width: 100px">
                <img src="~/assets/images/golang.png" style="width:90px;" alt="not found">
                <p>Golang</p>
                
            </div>
            <div class="python" style="width: 100px">
                <img src="~/assets/images/python.png" style="width:70px;" alt="not found">
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
        text-align: center;
        font-weight: 700;
    }
    .vue img {
        margin: 25px 0px 30px;
    }
    .golang{
        margin: 0px 20px;
    }
    .golang img {
        margin: 10px 0px 20px;
    }
    .python img {
        margin: 20px 0px 30px;
    }
    .react img {
        margin-bottom: 15px;
    }
    .react p{
        width: 100px;
        margin: 0px auto;
    }
    .node img {
        margin-bottom: 10px;
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
    }
   
        
    

 

</style>