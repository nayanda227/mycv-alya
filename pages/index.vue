<template>
  <body>
  <div class="container-fluid">
    <!-- Baris pertama: About Me dan Education -->
    <div class="row mb-4">
      <div class="col-md-5">
        <section id="about" class="box-section blue-box">
          <h2 class="text-center mb-4">About Me</h2>
          <p>Hi, I'm Nadia! I'm currently exploring the exciting world of web development. 
            Although I'm still in the learning phase, 
            I am passionate about building websites and am eager to expand my knowledge and skills. 
            My goal is to continually grow as a developer and bring creative and functional ideas to life. 
            I'm excited about the journey ahead and always open to new learning opportunities!</p>
        </section>
      </div>
      <div class="col-md-5">
        <section id="education" class="box-section blue-box">
          <h2 class="text-center mb-4">Education</h2>
          <ul class="list-unstyled">
            <li>
              <h5>Gelar atau Sertifikasi</h5>
              <p>Singosari Senior Highschool - 2020</p>
              <p>Deskripsi singkat tentang apa yang dipelajari atau dicapai.</p>
            </li>
          </ul>
          <ul class="list-unstyled">
            <li>
              <h5>Gelar atau Sertifikasi</h5>
              <p>Universitas Brawijaya - 2023</p>
              <p>Deskripsi singkat tentang apa yang dipelajari atau dicapai.</p>
            </li>
          </ul>
        </section>
      </div>
    </div>

    <!-- Baris kedua: Skill -->
    <div class="row mb-4 justify-content-center">
      <div class="col-md-5">
        <section id="skills" class="box-section blue-box">
          <h2 class="text-center mb-4">Skills</h2>
          <div class="skill">
            <h5>JavaScript</h5>
            <div class="progress">
              <div class="progress-bar" role="progressbar" style="width: 50%;" aria-valuenow="50" aria-valuemin="0" aria-valuemax="100">80%</div>
            </div>
          </div>
          <div class="skill">
            <h5>HTML & CSS</h5>
            <div class="progress">
              <div class="progress-bar" role="progressbar" style="width: 80%;" aria-valuenow="80" aria-valuemin="0" aria-valuemax="100">90%</div>
            </div>
          </div>
          <div class="skill">
            <h5>Vue.js</h5>
            <div class="progress">
              <div class="progress-bar" role="progressbar" style="width: 75%;" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100">75%</div>
            </div>
          </div>
        </section>
      </div>
    </div>
  </div>
  <!-- Footer -->
  <footer class="footer py-4 mt-auto">
      <div class="container text-center">
        <p>Follow me on:</p>
        <a href="https://github.com/nayanda227" target="_blank">Github</a> |
        <a href="https://linkedin.com/in/NadiaAlyaParamitha" target="_blank">LinkedIn</a>
        <p>Contact: <a href="mailto:nalya2911@gmail.com">nalya2911@gmail.com</a></p>
      </div>
    </footer>
</body>
</template>

<script>
export default {
  name: 'HomePage',
};
</script>

<style>
body {
  background-color: #ffc0cb; /* Background Pink Soft */
  min-height: 100vh; /* Pastikan background menutupi seluruh halaman */
  margin: 0;
  padding: 0;
}

.box-section {
  background-color: rgba(173, 216, 230, 0.5); /* Transparan Biru */
  border: 2px solid rgba(0, 0, 0, 0.1);
  border-radius: 1rem;
  padding: 2rem;
  margin-bottom: 2rem;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  min-height: 200px; /* Ukuran box seragam */
}

.blue-box {
  background-color: rgba(173, 216, 230, 0.5); /* Transparan Biru */
}

.row {
  justify-content: center;
  margin-top: 20px;
}

.progress {
  background-color: rgba(0, 0, 0, 0.1); /* Progress bar background */
  border-radius: 1rem;
  height: 20px;
}

.progress-bar {
  background-color: #007bff; /* Warna progress bar */
  border-radius: 1rem;
  text-align: center;
  line-height: 20px;
  color: white;
}

.footer {
  background-color: rgba(173, 216, 230, 0.7); /* Soft Blue Footer */
  color: #6c757d;
  margin-top: 50px;
  padding: 20px;
  border-top: 2px solid rgba(0, 123, 255, 0.5);
}

.footer a {
  color: #007bff;
  text-decoration: none;
}

.footer a:hover {
  color: #0056b3;
}
</style>
