<template>
    <section id="registrasi" class="registrasi">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-md-4">
                    <h2 class="title">Daptar Sekarang</h2>
                    <form>
                        <div class="form-group">
                            <label for="name">Nama Lengkap</label>
                            <input @keypress="checkValueName" type="text" class="form-control" id="name" placeholder="Contoh: Muda Juanri">
                            <small id="error-name" class="form-text text-muted" style="color: red !important"></small>

                        </div>
                        <div class="form-group">
                            <label for="email">Email</label>
                            <input @keypress="checkValueEmail" type="email" class="form-control" id="email" placeholder="Contoh: mudajuan@mail.com">
                            <small id="error-email" class="form-text text-muted" style="color: red !important"></small>

                        </div>
                        <div class="form-group">
                            <label for="phone">Ponsel(Whatsaap)</label>
                            <input @keypress="checkValuePhone" type="number" class="form-control" id="phone" placeholder="Contoh: 0822 2123 5445">
                            <small id="error-phone" class="form-text text-muted" style="color: red !important"></small>

                        </div>
                        <div class="form-group">
                            <label for="project">Judul Projek</label>
                            <input @keypress ="checkValueProject" type="text" class="form-control" id="project" placeholder="Contoh: Website portal berita kampus">
                            <small id="error-project" class="form-text text-muted" style="color: red"></small>

                        </div>
                        <div class="form-group">
                            <label for="mesaage">Deskripsi Tentang Projek</label>
                            <textarea @keypress="checkValueMessage" name="message" rows="5" id="message" class="form-control textarea" placeholder="Contoh: Jadi saya ingin membuat projek tugas akhir berupa web berita portal kampus"></textarea>
                            <small id="error-message" class="form-text text-muted" style="color: red !important"></small>

                        </div>
                        <div class="form-group flex-auto">
                            <button type="submit" class="btn btn-info" @click="validataInput">Daptar</button>
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
export default {
    data() {
        return {
            name: '',
            email: '',
            phone: '',
            project: '',
            message: '',
            errorElementName: '',
            errorElementEmail: '',
            errorElementPhone: '',
            errorElementProject: '',
            errorElementMessage: '',
        }
    },
    mounted() {
        this.name = document.getElementById('name')
        this.email = document.getElementById('email')
        this.phone = document.getElementById('phone')
        this.project = document.getElementById('project')
        this.message = document.getElementById('message')
        this.errorElementName = document.getElementById('error-name')
        this.errorElementEmail = document.getElementById('error-email')
        this.errorElementPhone = document.getElementById('error-phone')
        this.errorElementProject = document.getElementById('error-project')
        this.errorElementMessage = document.getElementById('error-message')
    },
    methods: {
        validataInput() {
            if(name.value == '') {
                errorElementName.innerHTML = 'nama tidak boleh kosong'
            }
            if(email.value == '') {
                errorElementEmail.innerHTML = 'email tidak boleh kosong'
            }
            if(phone.value == '') {
                errorElementPhone.innerHTML = 'wajib di isi'
            }
            if(project.value == '') {
                errorElementProject.innerHTML = 'wajib di isi'
            }
            if(message.value == '') {
                errorElementMessage.innerHTML = 'wajib di isi'
            }
            if(name.value !='' && email.value !='' && phone.value !='' && project.value !='' && message.value !='') {
                alert(`${name.value}, ${email.value}, ${phone.value}, ${project.value}, ${message.value} di kirim`)
            }
        },
        checkValueName() {
            if (name.value !='') {
                errorElementName.innerHTML =''
            }
        },
        checkValueEmail() {
            if (email.value !='') {
                errorElementEmail.innerHTML =''
            }
        }, 
        checkValuePhone() {
            if (phone.value !='') {
                errorElementPhone.innerHTML = ''
           }
        },
        checkValueProject() {
            if (project.value !='') {
                errorElementProject.innerHTML =''
            }
        },
        checkValueMessage() {
            if (message.value !='') {
                errorElementMessage.innerHTML =''
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