<template>
    <section id="registrasi" class="registrasi">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-md-4">
                    <h2 class="title">Daptar Sekarang</h2>
                    <form>
                        <div class="form-group">
                            <label for="nama">Nama Lengkap</label>
                            <input type="text" class="form-control" id="nama" placeholder="Contoh: Muda Juanri">
                        </div>
                        <div class="form-group">
                            <label for="email">Email</label>
                            <input type="email" class="form-control" id="email" placeholder="Contoh: mudajuan@mail.com">
                        </div>
                        <div class="form-group">
                            <label for="no.telp">Ponsel(Whatsaap)</label>
                            <input type="text" class="form-control" id="no.telp" placeholder="Contoh: 0822 2123 5445">
                        </div>
                        <div class="form-group">
                            <label for="no.telp">Judul Projek</label>
                            <input type="text" class="form-control" id="no.telp" placeholder="Contoh: Website portal berita kampus">
                        </div>
                        <div class="form-group">
                            <label for="pesan">Deskripsi Tentang Projek</label>
                            <textarea name="pesan" rows="5" id="pesan" class="form-control textarea" placeholder="Contoh: Jadi saya ingin membuat projek tugas akhir berupa web berita portal kampus"></textarea>
                        </div>
                        <div class="form-group flex-auto">
                            <button type="submit" class="btn btn-info">Daptar</button>
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