<template>
  <br>
  <br>
  <br>
   <div id="app" class="background">
    <header class="header">
      <div class="header-text">
        <h1 class="header-title">Chikal Verguson</h1>
        <h2 class="header-subtitle">Mahasiswa universitas Islam Riau Fakutltas Teknik Program Studi Teknik Informatika </h2>
        
        <div class="header-gambar">
           <img src="@/assets/gambar2.jpg" alt="Gambar Hobi">
        </div>
      </div>
    </header>

    <main class="content">
      <div class="nav-links">
        <router-link to="/" class="nav-link">Home</router-link>
        <router-link to="/about" class="nav-link">About</router-link>
        <router-link to="/blog" class="nav-link">Blog</router-link>
        <router-link to="/portfolio" class="nav-link">Portfolio</router-link>
      </div>
  
      <router-view></router-view>
      <div class="isi-conten">
      <section class="about-me">
        <h2>Tentang Saya</h2>
        <p>Saya adalah mahasiswa Teknik Informatika di Universitas Islam Riau. Saya memiliki minat dalam pengembangan web dan ingin terus belajar dan berkembang dalam bidang ini.</p>
      </section>

      <section class="my-work">
        <h2>Pengalaman</h2>
        <p>Saya pernah bekerja sama bapak saya, yaitu pekerjaan mencari mobil.</p>
      </section>

      <section class="social-media">
        <h2>Media Sosial</h2>
        <ul>
          <li><a href="https://www.instagram.com/chikalvergusonn/">instagram</a></li>
          <!-- Tambahkan tautan media sosial lainnya sesuai kebutuhan -->
        </ul>
      </section>

      <section class="my-work">
        <h2>My Hobi</h2>
        <p>Saya Mempunyai Hobi Bermain game  </p>
        <img src="@/assets/gambar1.jpeg" alt="Gambar Hobi">
      </section>
    </div>
    </main>
<br>
    <footer class="footer">
      <div class="footer-text">
        <p class="footer-copyright">
          &copy; {{ new Date().getFullYear() }} - Chikal Verguson
        </p>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'App',
  components: {
  }
}
</script>

<style>
.background {
  background-image: url('@/assets/gambar3.jpg');
  background-size: cover;
  background-position: center;
}

.nav-links {
  justify-content: center;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background-color: grey;
  padding: 20px 0;  
  z-index: 1000; 
}

.nav-link {
  color: white; 
  text-decoration: none; 
  margin: 0 10px; 
  font-size: 20px;
}

.nav-link:hover {
  text-decoration: underline; 
}


.content {
  margin-top: 50px; 
}


.header {
  color: white;
  font-size: 50px;
  padding: 20px 0;
  text-align: center;
  text-shadow: 10px 10px 10px black; 
}


.header-title {
  margin: 0; 
}

.header-subtitle {
  margin-top: 5px; 
}

.header-gambar {
  margin-top: 50px;
}

.header-gambar img {
  border-radius: 50%;
  box-shadow: 10px 20px 10px black; 
  width: 300px; 
  height: 300px; 
  object-fit: cover; 
}

.footer {
  background-color: grey; 
  color: white; 
  padding: 20px 0; 
  text-align: center; 
}

.footer-link {
  color: white; 
  text-decoration: none; 
  margin-left: 5px; 
}

.footer-link:hover {
  text-decoration: underline; 
}

.isi-conten {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

.isi-conten section {
  background-color: white;
  width: 300px;
  margin: 20px;
  padding: 20px;
  border: 5px solid #000000;
  border-radius: 10px;
  background-image:rgb(0, 0, 0);
}

.isi-conten h2 {
  margin-top: 0;
}

.isi-conten p {
  margin-bottom: 0;
}


</style>


