<template>
  <body>
    <div class="container-fluid">
      <!-- Bagian Experience -->
      <div class="col-md-5 mx-auto">
        <section id="experience" class="box-section pink-box">
          <h2 class="text-center mb-4">Experience</h2>
          <ul class="list-unstyled">
            <li>
              <h5>Student Council Member (OSIS)</h5>
              <p>Singosari Senior Highschool - 2020-2022</p>
              <p>Actively participated as a member of the student council, 
                organizing school events, managing student activities, and developing leadership and teamwork skills. 
                Worked collaboratively with peers to plan and execute various school programs, 
                contributing to the overall school community and enhancing student engagement.</p>
            </li>
          </ul>
        </section>
      </div>

      <!-- Bagian Portfolio -->
      <div class="col-md-5 mx-auto mt-4">
        <section id="portfolio" class="box-section green-box">
          <h2 class="text-center mb-4">Portfolio</h2>
          <div class="card">
            <img :src="projectImage" class="card-img-top" alt="Gambar Proyek">
            <div class="card-body">
              <h5 class="card-title">Apart</h5>
              <p class="card-text">Apart adalah aplikasi penyewaan apartemen yang memudahkan pengguna 
                mencari dan menyewa tempat tinggal. Dengan fitur pencarian berbasis tipe dan filter fasilitas, 
                Apart menawarkan pengalaman sewa yang cepat dan efisien.</p>
              <a href="https://github.com/nayanda227/Apart" class="btn btn-primary">Link Github Proyek</a>
            </div>
          </div>
        </section>
      </div>
    </div>
     <!-- Footer -->
     <footer class="footer py-4 mt-auto">
          <div class="container text-center">
              <p>Follow me on:</p>
              <a href="https://github.com/nayanda227" target="_blank">Github</a> |
              <a href="https://www.linkedin.com/in/nadia-alya-paramitha/" target="_blank">LinkedIn</a> |
              <a href="https://wa.me/6285742668675" target="_blank">WhatsApp</a> |
              <p>Contact: <a href="mailto:nalya2911@gmail.com">nalya2911@gmail.com</a></p>
          </div>
      </footer>
  </body>
</template>

<script>
import projectImage from '@/assets/img/Apart.png';

export default {
  name: 'HomePage',
  data() {
    return {
      projectImage,
      showForm: false
    };
  }
};
</script>

<style scoped>
/* Atur font menjadi lebih stylish */
body {
  background-color: #ffc0cb; /* Background Pink Soft */
  font-family: 'Poppins', sans-serif; /* Gunakan font yang lebih modern */
  min-height: 100vh;
  margin: 0;
  padding: 0;
}

h2 {
  font-size: 2.5rem;
  color: #333;
  font-weight: bold;
  margin-bottom: 1.5rem;
}

p {
  font-size: 1.1rem;
  color: #555;
}

.box-section {
  background-color: rgba(255, 255, 255, 0.2); /* Transparan */
  border-radius: 1rem;
  padding: 2rem;
  margin-bottom: 2rem;
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.1); /* Bayangan untuk kesan elegan */
}

/* Box khusus untuk Experience */
.pink-box {
  background-color: rgba(255, 255, 255, 0.553); /* Transparan Pink */
}

/* Box khusus untuk Portfolio */
.green-box {
  background-color: rgba(144, 238, 144, 0.3); /* Transparan Hijau */
}

.card {
  border: none;
  border-radius: 0.5rem;
}

.card-img-top {
  border-top-left-radius: 0.5rem;
  border-top-right-radius: 0.5rem;
}

.btn-primary {
  background-color: #007bff;
  border: none;
}

.btn-primary:hover {
  background-color: #0056b3;
}

/* Menambahkan margin agar tidak terlalu mepet */
.container-fluid {
  padding: 2rem;
}

.col-md-5 {
  margin-bottom: 2rem;
}

.footer {
  background-color: rgba(173, 216, 230, 0.7); /* Soft Blue Footer */
  color: #6c757d;
  padding: 20px;
  position: relative;
  width: 100%; /* Memastikan footer memanjang penuh */
  bottom: 0;
  border-top: 2px solid rgba(0, 123, 255, 0.5);
  }

  .footer a {
  color: #007bff;
  text-decoration: none;
  }

  .footer a:hover {
  color: #0056b3;
  }
  .container {
  max-width: 100%; /* Pastikan container juga memanjang penuh */
  }

</style>
