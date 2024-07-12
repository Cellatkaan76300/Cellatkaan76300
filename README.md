CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    ad VARCHAR(50) NOT NULL,
    soyad VARCHAR(50) NOT NULL,
    fiyat DECIMAL(10, 2) NOT NULL,
    telefon VARCHAR(20) NOT NULL
);
**<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kayıt Formu</title>
</head>
<body>
    <h2>Kayıt Formu</h2>
    <form action="kayit.php" method="post">
        <label for="ad">Ad:</label>
        <input type="text" id="ad" name="ad" required><br><br>

        <label for="soyad">Soyad:</label>
        <input type="text" id="soyad" name="soyad" required><br><br>

        <label for="fiyat">Fiyat:</label>
        <input type="text" id="fiyat" name="fiyat" required><br><br>

        <label for="telefon">Telefon Numarası:</label>
        <input type="text" id="telefon" name="telefon" required><br><br>

        <input type="submit" value="Kayıt Ol">
    </form>
</body>
</html>
<?php
// Veritabanı bağlantı bilgileri
$servername = "localhost";
$username = "kullanici_adi";
$password = "parola";
$dbname = "veritabani_adi";

// POST verilerini al
$ad = $_POST['ad'];
$soyad = $_POST['soyad'];
$fiyat = $_POST['fiyat'];
$telefon = $_POST['telefon'];

// Veritabanı bağlantısını oluştur
$conn = new mysqli($servername, $username, $password, $dbname);

// Bağlantıyı kontrol et
if ($conn->connect_error) {
    die("Veritabanı bağlantısı başarısız: " . $conn->connect_error);
}

// SQL komutunu hazırla ve veritabanına ekle
$sql = "INSERT INTO users (ad, soyad, fiyat, telefon) VALUES ('$ad', '$soyad', '$fiyat', '$telefon')";

if ($conn->query($sql) === TRUE) {
    echo "Kayıt başarıyla eklendi";
} else {
    echo "Hata: " . $sql . "<br>" . $conn->error;
}

// Veritabanı bağlantısını kapat
$conn->close();
?>
**- 👋 Hi, I’m @Cellatkaan76300
**- 👋 Hi, I’m @Cellatkaan76300
**- 👋 Hi, I’m @Cellatkaan76300
**- 👋 Hi, I’m @Cellatkaan76300
**- 👋 Hi, I’m @Cellatkaan76300
**- 👋 Hi, I’m @Cellatkaan76300
**- 👋 Hi, I’m @Cellatkaan76300
**- 👋 Hi, I’m @Cellatkaan76300
**- 👋 Hi, I’m @Cellatkaan76300
**- 👋 Hi, I’m @Cellatkaan76300
**- 👋 Hi, I’m @Cellatkaan76300
**- 👋 Hi, I’m @Cellatkaan76300
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Cellatkaan76300/Cellatkaan76300 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
