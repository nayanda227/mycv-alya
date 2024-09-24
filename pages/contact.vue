<template>
  <div class="row mb-4 justify-content-center">
    <div class="col-md-6">
      <section id="contact" class="box-section small-box">
        <h2 class="text-center mb-4">Kontak Saya</h2>
        <form>
          <div class="form-group">
            <label for="name">Nama</label>
            <input type="text" class="form-control" id="name" placeholder="Nama Anda">
          </div>
          <div class="form-group">
            <label for="email">Alamat Email</label>
            <input type="email" class="form-control" id="email" placeholder="Email Anda">
          </div>
          <div class="form-group">
            <label for="message">Pesan</label>
            <textarea class="form-control" id="message" rows="3" placeholder="Pesan Anda"></textarea>
          </div>
          <div class="text-center">
            <button type="submit" class="btn btn-submit">Kirim</button>
          </div>
        </form>
      </section>
    </div>
  </div>

  <!-- Footer -->
  <footer class="footer py-4 mt-auto">
    <div class="container text-center">
      <p>Follow me on:</p>
      <a href="https://github.com/nayanda227" target="_blank">Github</a> |
      <a href="https://linkedin.com/in/NadiaAlyaParamitha" target="_blank">LinkedIn</a> |
      <a href="https://wa.me/6285742668675" target="_blank">WhatsApp</a> |
      <p>Contact: <a href="mailto:nalya2911@gmail.com">nalya2911@gmail.com</a></p>
    </div>
  </footer>
</template>

<style>
  .box-section {
    background-color: rgba(255, 255, 255, 0.8); /* Box background */
    border: 1px solid rgba(0, 0, 0, 0.1);
    border-radius: 10px;
    padding: 2rem;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    margin-bottom: 2rem;
  }

  .small-box {
    max-width: 600px;
  }

  .btn-submit {
    background-color: #007bff;
    color: white;
    border: none;
    padding: 0.5rem 2rem;
  }

  .btn-submit:hover {
    background-color: #0056b3;
  }

  .footer {
    background-color: rgba(173, 216, 230, 0.7); /* Soft Blue Footer */
    color: #6c757d;
    padding: 20px;
    width: 100%; /* Full-width footer */
    position: relative;
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
    max-width: 100%; /* Full-width container */
  }

  .row {
    margin-top: 50px; /* Adds space between layout and top of form */
  }
</style>
