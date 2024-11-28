<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Website Pribadi</title>
    <style>
        /* CSS Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f9;
            color: #333;
        }

        header {
            background-color: #4CAF50;
            color: white;
            text-align: center;
            padding: 20px;
        }

        nav {
            display: flex;
            justify-content: center;
            background-color: #333;
            padding: 10px 0;
        }

        nav a {
            color: white;
            text-decoration: none;
            padding: 14px 20px;
            text-align: center;
            font-weight: bold;
        }

        nav a:hover {
            background-color: #ddd;
            color: black;
        }

        .container {
            width: 80%;
            margin: 20px auto;
            padding: 20px;
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            display: none;
        }

        .container h2 {
            text-align: center;
            color: #4CAF50;
            margin-bottom: 20px;
        }

        .content {
            text-align: center;
        }

        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>

    <!-- Header -->
    <header>
        <h1>Website Pribadi Saya</h1>
        <p>Selamat datang di website pribadi saya! Temukan lebih banyak tentang saya melalui halaman berikut.</p>
    </header>

    <!-- Navigation -->
    <nav>
        <a href="#" onclick="showSection('profil')">Profil</a>
        <a href="#" onclick="showSection('hobi')">Hobi</a>
        <a href="#" onclick="showSection('cita-cita')">Cita-cita</a>
    </nav>

    <!-- Profil Section -->
    <div class="container" id="profil">
        <h2>Profil</h2>
        <div class="content">
            <p>Kenalin nama aku Andhita maura fahla, aku biasa dipanggil dhita. Aku adalah anak kedua dari dua bersaudara, dan aku juga cucu terakhir di keluarga besar. Aku kelas 12 ips 2 di SMAN 5 Cimahi.</p>
        </div>
    </div>

    <!-- Hobi Section -->
    <div class="container" id="hobi">
        <h2>Hobi</h2>
        <div class="content">
            <p>Saya memiliki beberapa hobi, yaitu:</p>
            <ul style="list-style: none;">
                <li>📸 foto alam</li>
                <li>📝 menulis cerita</li>
                <li>🎶 Mendengarkan Musik</li>
            </ul>
        </div>
    </div>

    <!-- Cita-cita Section -->
    <div class="container" id="cita-cita">
        <h2>Cita-cita</h2>
        <div class="content">
            <p>Aku bercita-cita untuk menjadi seorang penulis. Minat menulis aku muncul ketika aku SMP, saat itu ada satu guru yang sangat menginspirasi aku. Hingga aku akhirnya bisa mengetahui apa cita-cita aku sebenarnya. Aku juga berharap jika aku sudah menciptakan buku nanti bukuku akan menambah minat baca di Indonesia.</p>
        </div>
    </div>

    <!-- Footer -->
    <footer>
        <p>&copy; 2024 Website Pribadi oleh Andhita Maura Fahla</p>
    </footer>

    <script>
        function showSection(section) {
            // Sembunyikan semua bagian
            const sections = document.querySelectorAll('.container');
            sections.forEach(function (el) {
                el.style.display = 'none';
            });

            // Tampilkan bagian yang dipilih
            document.getElementById(section).style.display = 'block';
        }

        // Menampilkan Profil secara default ketika halaman dimuat
        window.onload = function() {
            showSection('profil');
        };
    </script>

</body>
</html>
