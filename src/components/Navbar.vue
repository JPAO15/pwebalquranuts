<script>
import 'bootstrap/dist/css/bootstrap.css'
export default {
  name : "Navbar",
  components: {}
}
</script>
<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-dark">
    <div class="container">
      <a class="navbar-brand" style="color: white"   href="#">Al-Qur'an</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="/"><div class="anav">Home</div></a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="/juzamma"><div class="anav">Khatam</div></a>
          </li>
          <div class="dropdown">
            <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenuButton1" data-bs-toggle="dropdown" aria-expanded="false">
              Membaca Juz
            </button>
            <ul class="dropdown-menu" aria-labelledby="dropdownMenuButton1">
              <li><a class="dropdown-item" href="/juz1-5#juzsatu">Juz 1</a></li>
              <li><a class="dropdown-item" href="/juz1-5#juzdua">Juz 2</a></li>
              <li><a class="dropdown-item" href="/juz1-5#juztiga">Juz 3</a></li>
              <li><a class="dropdown-item" href="/juz1-5#juzempat">Juz 4</a></li>
              <li><a class="dropdown-item" href="/juz1-5#juzlima">Juz 5</a></li>
              <li><a class="dropdown-item" href="/juz1-5#juzenam">Juz 6</a></li>
              <li><a class="dropdown-item" href="/juz1-5#juztujuh">Juz 7</a></li>
              <li><a class="dropdown-item" href="/juz1-5#juzdelapan">Juz 8</a></li>
              <li><a class="dropdown-item" href="/juz1-5#juzsembilan">Juz 9</a></li>
              <li><a class="dropdown-item" href="/juz1-5#juzsepuluh">Juz 10</a></li>
            </ul>
          </div>
          <li class="nav-item">
            <a class="nav-link" href="/about"><div class="anav">Audio</div></a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<style scoped>
.navbar-brand{
  font-family: "Microsoft YaHei Light";
  font-weight: bold;
  font-size: 40px;
}
.nav-link:hover{
  border-bottom: 3px solid #ffffff;
}
.navbar{
  font-size: 30px;
  padding-bottom: 50px;
  background-color: #000000;
}
.anav{
  color: white;
  font-weight: bold;
}

.navbar-expand-lg .navbar-nav .dropdown-menu {
  position: absolute;
  background-color: #afafaf;
}
/* merubah warna hover */
.dropdown-item:focus, .dropdown-item:hover {
  color: #16181b;
  text-decoration: none;
  background-color: #e2e2e2;
}

.dropdown-menu .sub-menu {
  left: 100%;
  position: absolute;
  top: 0;
  visibility: hidden;
  margin-top: -1px;
}
.dropdown-menu li:hover .sub-menu {
  visibility: visible;
}
.dropdown:hover .dropdown-menu {
  display: block;
}

/* menghilangkan tanda panah kebawah (bottom arrow) */
a.menu:after, .dropdown-toggle:after {
  content: none;
}

.navbar-nav > li > a.active, .navbar-nav > li > a:focus {
  border-top: 0.1875rem solid var();
}

.navbar-nav {
  margin-right: 45rem;
}

.btn btn-secondary dropdown-toggle{
  color: black;
  font-size: 25px;
}
</style>