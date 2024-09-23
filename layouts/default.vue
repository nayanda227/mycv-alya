<template>
  <div>
    <header class="bg-pink text-center py-5 full-height position-relative">
      <div class="container">
        <!-- Navbar -->
        <nav class="navbar navbar-expand-lg navbar-light bg-light custom-navbar">
          <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse justify-content-center" id="navbarNav">
            <ul class="navbar-nav">
              <li class="nav-item">
                <NuxtLink class="nav-link" to="/">About</NuxtLink>
              </li>
              <li class="nav-item">
                <NuxtLink class="nav-link" to="/work">Work</NuxtLink>
              </li>
              <li class="nav-item">
                <NuxtLink class="nav-link" to="/contact">Contact</NuxtLink>
              </li>
            </ul>
          </div>
        </nav>
        <!-- Bagian Profil -->
        <div class="profile-box mx-auto p-4"
             :class="{ 'book-animation': isAnimating }"> <!-- Tambah class dinamis -->
          <img src="~assets/img/alya-profil.jpg" class="profile-img" alt="Nadia Alya">
          <h1>Nadia Alya Paramitha Erwanto</h1>
          <p>Student Information Technology in Brawijaya University</p>
          <!-- Tombol Navigasi -->
          <nuxt-link  
            class="btn btn-light btn-lg mt-3" 
            @click="scrollDown">
            Next
          </nuxt-link>
        </div>
      </div>
      <!-- Love besar di pojok kanan bawah -->
      <div class="love-icon"></div>
      <!-- Strap biru di pojok kanan atas dan kiri bawah -->
      <div class="strap-top-right"></div>
      <div class="strap-bottom-left"></div>
    </header>
    <main>
      <NuxtPage />
    </main>
  </div>
</template>

<script>
export default {
  layout: 'default',
  methods: {
    // Fungsi untuk melakukan scroll ke bawah
    scrollDown() {
      window.scrollTo({
        top: window.innerHeight, // Scroll setinggi viewport saat ini
        behavior: 'smooth', // Efek scroll halus
      });
    },
  },
};
</script>

<style scoped>
html {
  scroll-behavior: smooth;
}
/* Navbar Style */
.custom-navbar {
  border: 2px solid #ccc;
  border-radius: 25px;
  margin: 20px auto;
  max-width: 30%;
  padding: 10px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  position: relative;
}

.navbar-nav {
  justify-content: center;
}

.nav-link {
  margin: 0 10px;
  position: relative;
  padding: 5px 10px;
  transition: color 0.3s ease;
}

.nav-link:hover {
  color: #007bff;
}

.nav-item.active .nav-link {
  color: #007bff;
}

.nav-link::after {
  content: "";
  position: absolute;
  width: 0;
  height: 3px;
  bottom: -5px;
  left: 0;
  background-color: #007bff;
  transition: width 0.3s ease-in-out;
}

.nav-link:hover::after,
.nav-item.active .nav-link::after {
  width: 100%; /* Border box akan memanjang penuh */
}

.box-section {
  background-color: rgba(255, 255, 255, 0.2);
  border: 2px solid rgba(0, 0, 0, 0.1);
  border-radius: 1rem;
  padding: 2rem;
  margin-bottom: 2rem;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.small-box {
  max-width: 400px;
}

.blue-box {
  background-color: rgba(173, 216, 230, 0.2);
}

/* Adding transition effect when clicking links */
.nav-link.transition-active::after {
  transition: width 0.5s ease, transform 0.3s ease;
}
/* Warna background pink */
.bg-pink {
  background-color: #ffc0cb;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
}

/* Kotak putih tempat profil */
.profile-box {
  background-color: #ffffff;
  border-radius: 15px;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
  width: 350px;
  max-width: 100%;
  transition: transform 1s ease-in-out; /* Pastikan ada transition */
  transform-origin: left center;
}

/* Gambar profil */
.profile-img {
  border-radius: 50%;
  width: 200px;
  height: 200px;
  border: 6px solid #ffffff;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
  margin-bottom: 20px;
}

/* Strap biru di pojok kanan atas */
.strap-top-right {
  position: absolute;
  top: 0;
  right: 0;
  width: 150px;
  height: 100px;
  background-color: #a6c1ee;
  clip-path: polygon(0 0, 100% 0, 100% 100%);
}

/* Strap biru di pojok kiri bawah */
.strap-bottom-left {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 150px;
  height: 100px;
  background-color: #a6c1ee;
  clip-path: polygon(0 100%, 100% 100%, 0 0);
}

/* Love icon besar di pojok kanan bawah */
.love-icon {
  position: absolute;
  bottom: 20px;
  right: 20px;
  width: 100px;
  height: 100px;
  background-color: #ff69b4;
  clip-path: polygon(50% 0%, 100% 38%, 82% 100%, 50% 82%, 18% 100%, 0% 38%);
}

/* Header teks */
header h1 {
  font-size: 2rem;
  color: #333;
  margin-top: 10px;
}

header p {
  font-size: 1.1rem;
  color: #666;
}

/* Tombol */
header .btn {
  background-color: #a6c1ee;
  color: #333;
  border: none;
  padding: 10px 25px;
  border-radius: 50px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
  transition: background-color 0.3s ease;
}

header .btn:hover {
  background-color: #9db9e9;
  color: #fff;
}

/* Responsif */
@media (max-width: 768px) {
  .profile-box {
    width: 100%;
    padding: 20px;
  }

  header h1 {
    font-size: 1.8rem;
  }

  header p {
    font-size: 1rem;
  }

  .love-icon {
    width: 80px;
    height: 80px;
  }

  .strap-top-right,
  .strap-bottom-left {
    width: 100px;
    height: 35px;
  }
}
</style>