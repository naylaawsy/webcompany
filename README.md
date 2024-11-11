# webcompany
Membuat profil peusahaan sederhana menggunakan HTML dan CSS
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Company Profile</title>
    <link rel="stylesheet" href="style.css">
    <script src="https://unpkg.com/@phosphor-icons/web"></script>
    
</head>
<body>
<header>
    <nav class="wrapper">
        <div class="brand">
            <div class="name">I2YK</div>
            <div class="name2">Company.</div>
        </div>
        <div id="menu-icon" class="menu-icon">
            <i class="ph ph-list"></i>
        </div>
        <ul id ="menu-list" class="hidden">
            <li><a class="active" href="#home">Home</a></li>    
            <li><a href="#about">About Us</a></li> 
            <li><a href="#pesanan">Portofolio</a></li> 
            <li><a href="#contact">Contact Us</a></li>
        </ul> 
    </nav>
    <script src="/script.js"></script>
</header>

<!-- HOME -->
<div class="container" id="home">
    <div class="brand2">
        <div class="nama">WELCOME TO</div>
        <div class="nama2">I2YK COMPANY</div>
    </div>
    <p>I2YK Company adalah sebuah perusahaan baru yang memiliki tiga karyawan berbakat dibidang Teknologi Informasi. Berikut tiga profil karyawan di Company kami.</p>
    <div class="gallery">
        <a href="#Lola">
            <img src="lala.jpeg" alt="Lola Ardila">
        </a>
        <a href="#Hilma">
            <img src="ima.jpeg" alt="Hilma Hayati">
        </a>
        <a href="#Nayla">
            <img src="naya.jpeg" alt="Nayla Awalia Syafitri">
        </a>
    </div>
</div>
<!-- HOME SELESAI -->

<!-- ABOUT US -->
<div class="container" id="about">
    <h2>Tentang Kami</h2>
    <div class="about">
        <div class="profile" id="Lola">
            <a href="#Lala">
                 <img src="lala.jpeg" alt="Foto Anggota 1">
            </a>
            <h3>Lola Ardila</h3>
            <p>Saya Lola Ardilla, mahasiswi aktif di Universitas Djuanda Bogor, dengan mempunyai keahlian dalam mengoperasikan Microsoft Office. Keterampilan ini membantu saya dalam membuat dokumen secara profesional, menganalisis data, dan menyusun presentasi yang menarik.</p>
        </div>
        <div class="profile" id="Hilma">
            <a href="#ima">
                 <img src="ima.jpeg" alt="Foto Anggota 2">
            </a>
            <h3>Hilma Hayati</h3>
            <p>Hallo, nama saya Hilma Hayati. Saya adalah seorang Mahasiswa aktif di Fakultas Ilmu Komputer Universitas Djuanda Bogor. Saya memiliki ketertarikan pada dunia seni, khususnya menggambar. Melalui seni saya tertarik pada bidang desain seperti desain poster dan ilusi digital.</p>
        </div>
        <div class="profile" id="Nayla">
            <a href="#nana">
            <img src="naya.jpeg" alt="Foto Anggota 3">
            </a>
            <h3>Nayla Awalia Syafitri</h3>
            <p>Saya adalah mahasiswi yang sedang menempuh pendidikan S1 di Program Studi Ilmu Komputer, Universitas Djuanda, Bogor. Saya unggul dalam mengoperasikan Microsoft Excel dan juga bisa membuat pengumpulan data menggunakan MySql di ComandPromt. 
            </p>
        </div>
    </div>
</div>
<!-- ABOUT US SELESAI -->

<!-- PORTOFOLIO  -->
<div class="container" id="pesanan">
    <h2>Portofolio</h2>
<div class = "font">
    <p>Portofolio ini menampilkan beragam proyek pengembangan web dan aplikasi, database, maupun sebuah desain yang lahir dari kreativitas dan inovasi dari karyawan kami. Portofolio ini adalah bukti nyata dari keahlian kami dalam mengelola database, pengembangan web dan aplikasi serta merancang sebuah desain ilusi digital.</p>
    <div class="about">
       <div class="profile" id="Lala">
           <img src="gtw.jpeg" alt="Foto Anggota 1">
           <h3>Lola Ardila</h3>
       </div>
       <div class="profile" id="ima">
           <img src="sun flower.jpeg" alt="Foto Anggota 2">
           <h3>Hilma Hayati</h3>
       </div>
       <div class="profile" id="nana">
           <img src="mysql.jpeg" alt="Foto Anggota 3">
           <h3>Nayla Awalia Syafitri</h3>
       </div>
       </div>
   </div>
</div>
<!-- PORTOFOLIO SELESAI  -->

<!-- CONTACT US  -->
<div class="container" id="contact">
    <h2>Contact Us</h2>
    <form action="#" method="post">
        <label for="name">Nama:</label>
        <input type="text" id="name" name="name" required>

        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required>

        <label for="message">Pesan:</label>
        <textarea id="message" name="message" rows="5" required></textarea>

        <button type="submit">Kirim</button>
    </form>
</div>
<!-- CONTACK US SELESAI  -->

<!-- FOOTER  -->
<footer>
     <p> created by Kelompok 3 | copyright &copy;2024 Semua hak dilindungi.</p>
     <div class="font">
     <p> Lola Ardila - I.2310130</p>
     <p>Hilma Hayati - I.2310270</p>
     <p>Nayla Awalia Syafitri - I.2310537</p>
     </div>
</footer>
<!-- FOOTER END -->

</body>
</html>

const menuicon = document.getElementById("menu-icon");
const menulist = document.getElementById("menu-list");

menuicon.addEventListener("click", () => {
    menulist.classlist.toggle('hidden');
})

body {
    margin: 0;
    padding:0;
    font-family: "Roboto" , sans-serif;
}

/* Header */
.wrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;
    font-size: 20px;
    padding: 15px;
    width: 100%;
    height: 80px;
    background-color: #216598;
    box-shadow: 0 7px 15px 0 rgba(0, 0,0, 0,5);
    position: sticky;
    top: 0;
    z-index: 1000;
}

.brand {
    display: flex;
    flex-direction: row;
    font-size: 1.5em;
    padding: 15px;
    text-transform: capitalize;
}

.name {
    color: white;
    font-weight: 700;
    font-weight: bold;
}

.name2 {
    color: coral;
    font-weight: 400;
    padding-left: 0 5px;
    font-weight: bold;
}

nav ul{
    display: flex;
    justify-content: center;
    align-items: center;
}

nav ul li {
    list-style-type: none;
    padding: 15px;
} 

nav ul li a {
    color: white;
    font-size: 15px;
    text-decoration: none;
    text-transform: uppercase;
}

a.active,a:hover {
    background-color: #555;
    border-radius: 5px;
}

.menu-icon{
    /* background-color: tomato; */
    font-size: 28px;
    display: none;
    align-items: center;
}

@media only screen and (max-width: 768px) {
    nav{
        flex-wrap: wrap;
    }

    nav ul {
        flex-direction: column;
        width:100%;
    }

    nav ul.hidden{
        display: none;
    }

    .menu-icon {
        display: flex;
         align-items: center;
        cursor: pointer; /* Tangan saat hover */
    }
}

/* Home */
#home {
    background-image: url('yaya.jpeg');
    background-size: cover;
    background-position: center;
    width: 100%;
    color: rgb(11, 0, 0);
    text-align: center;
    padding: 100px 20px; /* Tambahkan padding untuk memberi ruang */
}

.brand2 {
    display: flex;
    justify-content: center;
    font-size: 1.5em;
    padding: 15px;
    text-transform: capitalize;
    text-align: center;
}

.nama {
    color: rgb(9, 9, 9);
    font-weight: 700;
}

.nama2 {
    color: coral;
    font-weight: 400;
    padding-left: 4px;
}

.gallery {
    display: flex;
    width: 100%;
    justify-content: center;
    gap: 20px;
    margin-top: 20px; 
}

.gallery img {
    width: 200px;
    height: auto;
    border-radius: 10px; /* Membuat sudut gambar melengkung */
}

/* About Us */
#about {
    background-color: #FFFF;
    color: #0c0c0ce9;
    width: 100%;
    padding: 20px;
    font-size: 1.5em;
    text-align: center;
}


.about {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
    font-size: medium;
    font-weight: none;
}

.profile {
    text-align: center;
    margin: 10px;
    padding: 20px;
    border: 1px solid #ccc; /* Tambahkan border untuk kotak */
    border-radius: 10px; /* Sudut kotak melengkung */
    background-color: rgb(165, 211, 242); 
    width: 300px; /* Lebar kotak */
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1); /* Bayangan untuk efek kedalaman */
}

.profile img {
    width: 100%;
    border-radius: 10px; /* Sudut gambar melengkung */
}

/* Portofolio */
#pesanan {
    background-color: #ffff; 
    color: #090909e9;
    width: 100%;
    font-size: 1.5em;
    text-align: center;
}

.font {
    font-size: medium; 
    line-height: none; 
}

.about {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
    font-size: medium;
}

/* Contact Us */
#contact {
    background-color:#cce1ef;
    color: #040000e9;
    width: 100%;
    padding: 20px;
    font-size: 1.5em;
    text-align: center;
}
form {
    display: flex;
    flex-direction: column;
    gap: 10px;
    font-size: medium;
    font-weight: none;
    text-align: left;
}

label {
    font-weight: bold;
}

input, textarea {
    padding: 10px;
    border: 1px solid #020202;
    border-radius: 5px;
}

button {
    background-color: #4CAF50;
    color: white;
    padding: 10px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

button:hover {
    background-color: #abd6f2;
}



/* Footer */
footer {
    display: flex;
    flex-direction: column;
    width: 100%;
    text-align: center;
    font-size: small;
    padding: 10px 0;
    background-color: #4e4c4c;
    color: white;
}

.font {
    text-align: center;
    font-size: smaller;
    padding: 0;
    margin: 0;
    color: #ffff;
}


