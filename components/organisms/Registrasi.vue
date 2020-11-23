<template>
    <section id="registrasi" class="registrasi">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-md-4">
                    <h2 class="title">Daftar Sekarang</h2>
                    <form>
                        <div class="form-group">
                            <label for="name">Nama Lengkap</label>
                            <input v-model="name" @keypress="checkValue('name')" type="text" class="form-control" id="name" placeholder="Contoh: Muda Juanri">
                            <small id="error-name" class="form-text text-muted" style="color: red !important" v-if="errorName">{{ errorName }}</small>

                        </div>
                        <div class="form-group">
                            <label for="email">Email</label>
                            <input v-model="email" @keypress="checkValue('email')" type="email" class="form-control" id="email" placeholder="Contoh: mudajuan@mail.com">
                            <small id="error-email" class="form-text text-muted" style="color: red !important" v-if="errorEmail">{{errorEmail}}</small>

                        </div>
                        <div class="form-group">    
                            <label for="phone">Ponsel (Whatsapp)</label>
                            <input v-model="phone" @keypress="checkValue('phone')" type="number" class="form-control" id="phone" placeholder="Contoh: 0822 2123 5445">
                            <small id="error-phone" class="form-text text-muted" style="color: red !important" v-if="errorPhone">{{errorPhone}}</small>

                        </div>
                        <div class="form-group">
                            <label for="project">Judul Projek</label>
                            <input v-model="project" @keypress="checkValue('project')" type="text" class="form-control" id="project" placeholder="Contoh: Website portal berita kampus">
                            <small id="error-project" class="form-text text-muted" style="color: red !important" v-if="errorProject">{{errorProject}}</small>

                        </div>
                        <div class="form-group">
                            <label for="message">Deskripsi Tentang Projek</label>
                            <textarea v-model="message" @keypress="checkValue('message')" name="message" rows="5" id="message" class="form-control textarea" placeholder="Contoh: Jadi saya ingin membuat projek tugas akhir berupa web berita portal kampus"></textarea>
                            <small id="error-message" class="form-text text-muted" style="color: red !important" v-if="errorMessage">{{errorMessage}}</small>

                        </div>
                        <div class="form-group flex-auto">
                            <button type="submit" class="btn btn-info" data-toggle="modal" data-target="#exampleModal" @click.prevent="clickRegister">Daptar</button>
                        </div>
                        <div v-if="sendData">
                           <Modal/>
                        </div>
                    </form>
                </div>
                <div class="col-md-6">
                    
                        <div class="card-body text-center">
                             <img  class="reg-image" src="~/assets/images/registration.png"  alt="not found">
                        </div>
                   
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import axios from 'axios'
import Modal from "~/components/mollecules/Modal.vue"
export default {
    components: {
        Modal: Modal,
    },
    data() {
        return {
            sendData: false,
            name: '',
            email: '',
            phone: '',
            project: '',
            message: '',
            errorName: '',
            errorEmail: '',
            errorPhone: '',
            errorProject: '',
            errorMessage: '',
        }
    },
    mounted() {
        
    },
    methods: {
        clickRegister() {
            this.validataInput()
            let payload = {
                fullname:this.name,
                email: this.email,
                whatsapp: this.phone,
                project_title: this.project,
                project_description: this.message
            }
            axios.post('https://bimbinganbareng-api.herokuapp.com/',payload)
            .then(res=>{
                console.log('kalau berhasil');
                console.log(res);
                this.sendData = true  
                
            })
            .catch(err=>{
                console.log('kalau error');
                console.log(err);
            })
        },
        validataInput() {
            if (this.name == '') {
                this.errorName = 'Nama tidak boleh kosong'
            }
            if (this.email == '') {
                this.errorEmail = 'email tidak boleh kosong'
            }
            if (this.phone == '') {
                this.errorPhone = 'tidak boleh kosong'
            }
            if (this.project == '' ) {
                this.errorProject = 'tidak boleh kosong'
            }
            if (this.message == '') {
                this.errorMessage = 'tidak boleh kosong'
            }
        },
        checkValue(param) {
            if (param == 'name') {
                this.errorName = ''
            }
            if (param == 'email') {
                this.errorEmail = ''
            }
            if (param == 'phone') {
                this.errorPhone = ''
            }
            if (param == 'project') {
                this.errorProject = ''
            }
            if (param == 'message') {
                this.errorMessage = ''
            }
        },
    }
}
</script>

<style>
    .registrasi {
        padding: 80px;
    }
    .title {
        font-size: 32px;
        font-weight: 700;
        margin-bottom: 25px;
    }
    .form-control{
        font-size: 16px;
    }
    .textarea{
        padding: 5px px 5p 0px;
    }
    label{
        font-size: 18px;
        font-weight: 400;
    }
    .reg-image{
       width: 450px;
    }
    .row {
        align-items: center;
    }
    @media (max-width: 768px) {
        .registrasi {
            margin-top: 50px;
            padding: 0px 20px;
        }
        .card-body  {
            width: 100%;
            padding: 0px 0px;
            margin: 0px 0px;
        }
        .col-md-4 {
            width: 100%;
            padding: 0px 20px;
            margin: 0px 0px;
        }
        .col-me-6 {
            width: 100% !important;
            margin: 0px 0px;
            padding: 0px 0px;
        }
    }
    @media(max-width: 860px) {
         .reg-image{
            width: 100%;
            margin: 0px 0px;
            padding: 0px 0px;
        }
    }
       

</style>