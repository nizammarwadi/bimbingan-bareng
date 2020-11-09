<template>
    <section class="intro">
        <div class="intro-middle-left">
            <p>Membantu bimbingan, mentoring dan penyelesaian Projek, Tugas Akhir  dan Penelitian berupa Website dan Aplikasi Mobile</p>
            <button type="submit" class="intro-middle-button">Daptar</button>
        </div>
        <div class="intro-middle-right">
            <img src="~/assets/images/intro.png" @click="toRegistrasi" alt="not found" class="image">
        </div>   
    </section>
</template>

<script>
export default {
    data() {
        return{
            buttonElement: "",
        }
    },
    mounted() {
        this.buttonElement = document.getElementById("registrasi")
    },
    methods: {
        toRegistrasi() {
            this.buttonElement.scrollIntoView({
                bahavior: "smooth",
                block: "start",
                inline: "nearest",
            })
        }
    }
}
</script>

<style>

    .intro{
        display: flex;
        justify-content: space-around;
        align-items: center;
        background-color: #A4DEF9;
        padding: 100px 100px 82px 100px;
        width: 100%;
    }
    .intro-middle-left{
        Height: 197px;
        Top: 171px;
        font-weight: 650;
        font-style: normal;
        font-size: 25px;
        line-height: 36px;
        color: white;
    }
    .intro-middle-left p{
        width: 403px;
    }
    .intro-middle-right{
        width: 377px;    
        Top: 117.77px;
    }
    .intro-middle-button{
        width: 141px;
        height: 39.05px;
        background: #A4DEF9;
        font-size: 18px;
        border: 1px solid #FFFFFF;
        box-sizing: border-box;
        color: white;
    }
    @media(max-width: 992px) {
        .intro {
            display: block;
            margin: 50px 0px 0px 0px;
            padding: 60px 0px 20px 0px;
            widows: 100%;
        }
        .intro-middle-left {
            margin-top: 40px;
            padding: 0px;
            width: 100%;
            text-align: center;
        }
        .intro-middle-left p {
            margin: 0px 0px;
            padding: 0px 0px;
            width: 100%;
        }
        .intro-middle-left .intro-middle-button {
            margin: 20px 0px 10px 0px;
        }
        .intro-middle-right {
            margin: 10px 0px 0px 0px;
            padding: 0px;
            width: 100%;
            text-align: center;
        }
        .intro-middle-right img {
            width: 100%;
            
        }
    }
</style>