### JAVASCRIPT
Javascript adalah bahasa pemrograman yang awalnya dirancang untuk berjalan di atas browser. Namun, seiring perkembangan zaman, javascript tidak hanya berjalan di atas browser saja. Javascript juga dapat digunakan pada sisi Server, Game, IoT, Desktop, dsb.

Nama resmi JavaScript adalah ECMAScript. ECMAScript dikembangkan oleh ECMA Organization. ECMA-262 adalah standar resmi JavaScript. Diciptakan oleh Brendan Eich. Muncul pertama kali di semua browser Netscape dan Microsoft pada tahun 1996. Disetujui sebagai standar internasional pada tahun 1998.

JavaScript digunakan untuk memprogram perilaku halaman web, diantaranya adalah:

- Dapat Mengubah Konten HTML
- Dapat Mengubah Nilai Atribut HTML
- Dapat Mengubah Gaya HTML (CSS)
- Dapat Menyembunyikan Elemen HTML
- Dapat Menampilkan Elemen HTML
### PRAKTIKUM 5 
1. Persiapan membuat dokumen HTML dengan nama file lab5_javascript.html seperti berikut.

```HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Mengenal JavaScript</title>
</head>
<body>
    <h1>Pengenalan JavaScript</h1>
    <h3>Contoh document.write dan console.log</h3>
    <script>
        document.write("Hello World");
        console.log("Hello World");
    </script>
</body>
</html>
```

- Output
![img.1](gambar/gambar%201.png)

2. Pemakaian Alert sebagai property window.

```HTML
<html>
<head>
<title>alert box</title>
</head>
<body>
<script language = "javaScript">
<!--
window.alert("ini merupakan pesan untuk anda");
//-->
</script>
</body>
</html>
```

- Output
![img.1](gambar/gambar%202.png)

3. Pemakaian method dalam objek

```HTML
<html>
<head>
<title>skrip javascript</title>
</head>
<body>
percobaan memakai javascript:<br>
<script language = "javascript">
<!--
document.write("selamat mencoba javascript<br>");
document.write("semoga sukses!");
//-->
</script>
</body>
</html>
```

- output 
![img.1](gambar/gambar%203.png)

4. Pemakaian Prompt

```HTML
<html>
<head>
<title>pemasukan data</title>
</head>
<body>
<script languange = "javascript">
<!--
var nama = prompt("siapa nama anda?","masukkan nama anda");
document.write("hai, " + nama);
//-->
</script>
</body>
</html>
```

- Output
![img.1](gambar/gambar%204.png)
- Masukan nama anda
![img.1](gambar/gambar%205.png)

5. Pembuatan fungsi dan cara pemanggilannya
```HTML
<html>
<head>
    <title>contoh program javascript</title>
    <script language="javascript">
    function pesan(){
        alert ("memanggil javascript lewat body onload")
    }
    </script>
</head>
<body onload=pesan()>
</body>
</html>
```

-Output
![img.1](gambar/gambar%206.png)

6. Operasi dasar aritmatika

```HTML
<html>
<head>
    <title>contoh program javascript</title>

    <script language="javascript">
    function test (val1,val2)
    {
        document.write("<br>"+"perkalian : val1*val2 "+"<br>")
        document.write(val1*val2)
        document.write("<br>"+"pembagian : val1/val2 "+"<br>")
        document.write(val1/val2)
        document.write("<br>"+"penjumlahan : val1+val2 "+"<br>")
        document.write(val1+val2)
        document.write("<br>"+"pengurangan : val1-val2 "+"<br>")
        document.write(val1-val2)
        document.write("<br>"+"modulus : val1%val2 "+"<br>")
        document.write(val1%val2)
    }
    </script>
</head>
<body>
    <input type="button" name="button1" value="arithmetic" onclick=test(9,4)>
</body>
</html>
```

- Output
![img.1](gambar/gambar%207.png)
![img.1](gambar/gambar%208.png)

7. Seleksi kondisi(if,else)

```HTML
<html>
<head>
    <title>contoh if-else</title>
</head>
<body>
    <script language="javascript">
    <!--
        var nilai = prompt("nilai (0-100): ", 0);
        var hasil = "";
        if (nilai >= 60)
        hasil = "lulus";
        else
        hasil = "tidak lulus";
        document.write("hasil: " + hasil);
    //-->
    </script>
</body>
</html>
```

- Output
![img.1](gambar/gambar%209.png)
![img.1](gambar/gambar%2010.png)

8. Penggunaan operator switch untuk seleksi kondisi

```HTML
<html>
<head>
    <title>contoh program javascript</title>

    <script language = "javascript">
    function test ()
        {
            val1 = window.prompt("input nilai (1-5)")
            switch (val1)
            {
                case "1" : 
                    document.write("bilangan satu")
                    break
                case "2" : 
                    document.write("bilangan dua")
                    break
                case "3" : 
                    document.write("bilangan tiga")
                    break
                case "4" : 
                    document.write("bilangan empat")
                    break
                case "5" : 
                    document.write("bilangan lima")
                    break
                default : 
                    document.write("bilangan lainnya")
            }
        }
    </script>
</head>
<body>
    <input type="button" name="button1" value="switch" onclick=test()>
</body>
</html>
```

- Output
![img.1](gambar/gambar%2011.png)
![img.1](gambar/gambar%2012.png)
![img.1](gambar/gambar%2013.png)

9. form Input

```HTML
<html>
<head>
    <script language="javascript">
        function test () {
            var val1 = document.kirim.T1.value
            if (val1%2==0)
                document.kirim.T2.value = "bilangan genap"
            else   
                document.kirim.T2.value = "bilangan ganjil"
        }
    </script>
</head>
<body>
    <form method="POST" name="kirim">
        <p>BIL <input type="text" name="T1" size="20">
        MERUPAKAN BIL <input type="text" name="T2" size="20"></p>
        <p><input type="button" name="B1" value="TEBAK" onclick=test()></p>
    </form>
</body>
</html>
```

- Output
![img.1](gambar/gambar%2014.png)
![img.1](gambar/gambar%2015.png)

10. form Button

```HTML
<html>
<head>
    <title>objek document</title>
</head>
<body>
    <script language = "javascript">
    <!--
        function ubahWarnaLB(warna) {
            document.bgColor = warna;
        }
        function ubahWarnaLD(warna) {
            document.fgColor = warna;
        }
    //-->
    </script>

    <h1>tes</h1>
    <form>
        <input type="button" value="Latar Belakang Hijau" onclick="ubahWarnaLB('GREEN')">
        <input type="button" value="Latar Belakang Putih" onclick="ubahWarnaLB('WHITE')">
        <input type="button" value="Teks Kuning" onclick="ubahWarnaLD('YELLOW')">
        <input type="button" value="Teks Biru" onclick="ubahWarnaLD('BLUE')">
    </form>
    <script language = "javascript">
        <!--
        document.write("Dimodivikasi terakhir pada " + document.lastModified);
        //-->
    </script>
</body>
</html>
```

- Output
![img.1](gambar/gambar%2016.png)
![img.1](gambar/gambar%2017.png)

11. Pilihan menggunakan checkBox dengan perhitungan otomatis

```HTML
<!--
file: daftarmeu.html
//-->
<html>
<head>
    <title>Daftar Menu</title>
    <script>
        function hitung(ele) {
            var total = document.getElementById('total').value;
            total = total ? parseInt(total) : 0;
            var harga = 0;

            if (ele.checked) {
                harga = ele.getAttribute('value'); // Mengambil nilai dari atribut 'value'
                total += parseInt(harga);
            } else {
                harga = ele.getAttribute('value'); // Mengambil nilai dari atribut 'value'
                if (total > 0) 
                    total -= parseInt(harga);  
            }

            document.getElementById('total').value = total;
        }
    </script>
</head>
<body>
    <h1>Daftar Menu</h1>

    <label><input type="checkbox" value="5000" id="menu1" onclick="hitung(this);"> Ayam Goreng Rp. 5.000</label><br />
    <label><input type="checkbox" value="500" id="menu2" onclick="hitung(this);"> Tempe Goreng Rp. 500</label><br />
    <label><input type="checkbox" value="2500" id="menu3" onclick="hitung(this);"> Telur Dadar Rp. 2.500</label><hr />
    <strong>Total Bayar: Rp. <input id="total" type="text" ></strong>
</body>
</html>
```

- Output
![img.1](gambar/gambar%2018.png)
![img.1](gambar/gambar%2019.png)

### PERTANYAAN DAN TUGAS
1. Buat script untuk melakukan validasi pada isian form.
<!DOCTYPE html>
<html>
<head>
  <title>Validasi Form</title>
  <style>
    .error {
      color: red;
    }
    
    body {
      font-family: Arial, sans-serif;
      background-color: #b3ebfc;
      text-align: center;
    }

    .container {
      max-width: 100px;
      margin: 0 auto;
      background-color: #fff;
      padding: 50px;
      border-radius: 5px;
      box-shadow: 0 2px 5px #ccc;
    }

    h2 {
      color: #333;
    }

    label {
      display: block;
      margin-bottom: 5px;
      color: #333;
    }

    input[type="text"], textarea {
      width: 70%;
      padding: 10px;
      margin-bottom: 10px;
      border: 1px solid #ccc;
      border-radius: 4px;
    }

    .error {
      color: red;
      font-size: 14px;
    }

    input[type="submit"] {
      background-color: #ffffff;
      color: #070707;
      padding: 10px 20px;
      border: none;
      border-radius: 4px;
      cursor: pointer;
    }

    input[type="submit"]:hover {
      background-color: #ffffff;
    }
  </style>
</head>
<body>
  <h2>Formulir Validasi</h2>
  <form id="myForm" action="proses.php" method="post">
    <label for="nama">Nama:</label>
    <input type="text" id="nama" name="nama">
    <span class="error" id="namaError"></span><br><br>

    <label for="email">Email:</label>
    <input type="text" id="email" name="email">
    <span class="error" id="emailError"></span><br><br>

    <label for="pesan">Pesan:</label>
    <textarea id="pesan" name="pesan" rows="4" cols="50"></textarea>
    <span class="error" id="pesanError"></span><br><br>

    <input type="submit" value="Submit">
  </form>

  <script>
    // Fungsi untuk memvalidasi form
    function validateForm() {
      let nama = document.getElementById("nama").value;
      let email = document.getElementById("email").value;
      let pesan = document.getElementById("pesan").value;

      let namaError = document.getElementById("namaError");
      let emailError = document.getElementById("emailError");
      let pesanError = document.getElementById("pesanError");

      let valid = true;

      // Validasi Nama
      if (nama === "") {
        namaError.textContent = "Nama harus diisi";
        valid = false;
      } else {
        namaError.textContent = "";
      }

      // Validasi Email
      if (email === "") {
        emailError.textContent = "Email harus diisi";
        valid = false;
      } else {
        emailError.textContent = "";
      }

      // Validasi Pesan
      if (pesan === "") {
        pesanError.textContent = "Pesan harus diisi";
        valid = false;
      } else {
        pesanError.textContent = "";
      }

      return valid;
    }

    // Event listener untuk mengirim form setelah validasi
    document.getElementById("myForm").addEventListener("submit", function(event) {
      if (!validateForm()) {
        event.preventDefault(); // Menghentikan pengiriman form jika validasi gagal
      }
    });
  </script>
</body>
</html>

- Output
![img.1](gambar/gambar%2020.png)
### SELESAI