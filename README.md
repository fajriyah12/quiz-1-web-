#profil _ig 
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fajriyah Indriani</title>
    <style>
        body {
            font-family: Colonna MT, sans-serif;
            background-color:rgb(34, 147, 217);
            text-align: center;
            padding: 20px;
        }
        .container {
            max-width: 400px;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgb(238, 246, 246);
        }
        .profile-img {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            object-fit: cover;
        }
        .social-icons {
            margin: 10px 0;
        }
        .social-icons a {
            text-decoration: none;
            margin: 0 10px;
            font-size: 24px;
            color: black;
        }
        .button {
            display: block;
            background:rgb(27, 147, 232);
            padding: 15px;
            margin: 10px 0;
            text-decoration: none;
            color: black;
            border-radius: 5px;
            font-weight: bold;
        }
    </style>
</head>
<body>

<section id ="profil">
<div class="container">
    <img src="riri.04.jpg" alt="Profile Picture" class="profile-img">
    <h2>Fajriyah Indriani</h2>
    <p>link outfit</p>
    
    <div class="social-icons">
        <a href="#"><img src="th.jpeg" width="30"></a>
        
    </div>
    <a href = "http://localhost/jadwal_pelajaran/jadwal_pelajaran"
    <a href="#" class="button">linktr.shopee</a>
</section>

</div>

</body>
</html>

#jadwal_pelajaran
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jadwal Pelajaran - Stitch Theme</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Baloo+2&display=swap');
        
        body {
            font-family: 'Baloo 2', cursive;
            background-color: #87CEEB;
            text-align: center;
            padding: 20px;
        }
        .container {
            max-width: 500px;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
            position: relative;
        }
        .stitch-img {
            width: 120px;
            position: absolute;
            top: -60px;
            left: 50%;
            transform: translateX(-50%);
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 10px;
        }
        th, td {
            border: 2px solid #4682B4;
            padding: 10px;
            text-align: center;
        }
        th {
            background-color: #4682B4;
            color: white;
        }
        .highlight {
            background-color: #FFD700;
        }
        .button {
            display: inline-block;
            background: #4682B4;
            padding: 15px;
            margin: 15px 0;
            text-decoration: none;
            color: white;
            border-radius: 5px;
            font-size: 18px;
            font-weight: bold;
            cursor: pointer;
        }
    </style>
</head>
<body>

<div class="container">
    <img src="https://i.pinimg.com/originals/2f/6d/cd/2f6dcd1aa257ed676b527723e42eebad.png" class="stitch-img">
    <h2>Jadwal Pelajaran</h2>
    <p id="hari-ini"></p>

    <table>
        <thead>
            <tr>
                <th>Hari</th>
                <th>Jam</th>
                <th>Mata Pelajaran</th>
            </tr>
        </thead>
        <tbody>
            <tr data-hari="Senin">
                <td>Senin</td>
                <td>07:00 - 08:30</td>
                <td>pembelajaran mesin</td>
            </tr>
            <tr data-hari="Selasa">
                <td>Selasa</td>
                <td>08:30 - 10:00</td>
                <td>analisis dan desain si</td>
            </tr>
            <tr data-hari="Rabu">
                <td>Rabu</td>
                <td>10:00 - 11:30</td>
                <td>pemprograman web</td>
            </tr>
            <tr data-hari="Kamis">
                <td>Kamis</td>
                <td>13:00 - 14:30</td>
                <td>pdt</td>
            </tr>
            <tr data-hari="Jumat">
                <td>Jumat</td>
                <td>14:30 - 16:00</td>
                <td>teknologi dan aplikasi  mobile</td>
            </tr>
        </tbody>
    </table>
 
</div>

<script>
    function highlightToday() {
        const hariSekarang = new Date().toLocaleDateString('id-ID', { weekday: 'long' });
        document.getElementById("hari-ini").innerText = "Hari ini: " + hariSekarang;

        const rows = document.querySelectorAll("tbody tr");
        rows.forEach(row => {
            if (row.getAttribute("data-hari") === hariSekarang) {
                row.classList.add("highlight");
            }
        });
    }
</script>

</body>
</html>
