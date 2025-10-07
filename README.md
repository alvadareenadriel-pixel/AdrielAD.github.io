<!doctype html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>🌐 My Personal Website</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">
  <style>
    /* === Background Futuristik === */
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
      background-size: 400% 400%;
      animation: gradientMove 15s ease infinite;
      color: white;
    }

    @keyframes gradientMove {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    /* === Navbar Transparan === */
    nav {
      background: rgba(0,0,0,0.6);
      padding: 15px;
      border-radius: 0 0 15px 15px;
      backdrop-filter: blur(10px);
      text-align: center;
    }
    nav ul {
      list-style: none;
      margin: 0;
      padding: 0;
    }
    nav ul li {
      display: inline-block;
      position: relative;
    }
    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
      font-weight: 500;
      transition: color 0.3s, border-bottom 0.3s;
    }
    nav a:hover {
      color: #ff00cc;
      border-bottom: 2px solid #ff00cc;
      padding-bottom: 3px;
    }

    /* === Dropdown === */
    .dropdown-content {
      display: none;
      position: absolute;
      background: rgba(0,0,0,0.9);
      min-width: 150px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.5);
      border-radius: 8px;
      z-index: 1;
    }
    .dropdown-content a {
      color: white;
      padding: 10px 15px;
      text-decoration: none;
      display: block;
      text-align: left;
      transition: background 0.3s;
    }
    .dropdown-content a:hover {
      background: #ff00cc;
      border-radius: 10px;
      color: white;
    }
    nav ul li:hover .dropdown-content {
      display: block;
    }

    /* === Header === */
    .header {
      text-align: center;
      padding: 40px;
      background: rgba(255,255,255,0.05);
      border-radius: 15px;
      margin: 20px auto;
      max-width: 900px;
      animation: fadeIn 2s ease;
    }

    .header h1 {
      font-size: 2.5rem;
      font-weight: 700;
      background: linear-gradient(90deg, #ff00cc, #3333ff);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    .header p {
      font-size: 1rem;
      font-weight: 300;
      margin-top: 10px;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(-20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    /* === Card Container === */
    .card-container {
      display: flex;
      justify-content: center;
      gap: 20px;
      flex-wrap: wrap;
      padding: 40px;
    }

    /* === Card Style === */
    .card {
      width: 280px;
      border-radius: 20px;
      overflow: hidden;
      background: rgba(255,255,255,0.08);
      backdrop-filter: blur(10px);
      box-shadow: 0 8px 20px rgba(0,0,0,0.5);
      transition: transform 0.3s, box-shadow 0.3s;
    }

    .card:hover {
      transform: translateY(-10px) scale(1.05);
      box-shadow: 0 15px 30px rgba(255,0,200,0.5);
    }

    .card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
    }

    .card-content {
      padding: 15px;
      text-align: center;
    }

    .card-content h3 {
      margin: 10px 0;
      font-weight: 500;
    }
  </style>
</head>
<body>
  
  <!-- Navbar -->
  <nav>
    <ul>
      <li><a href="template.html">🏠 Beranda</a></li>
      <li><a href="Aboutme.html">👤 Tentang Saya</a></li>
      <li>
        <a href="#">Ⓜ Menghitung ▼</a>
        <div class="dropdown-content">
          <a href="luas.html">Luas</a>
          <a href="volume.html">Volume</a>
        </div>
      </li>
      <li><a href="jadwal2.html">📅 Jadwal Pelajaran</a></li>
      <li><a href="lagu.html">🎵 Syair Lagu</a></li>
    </ul>
  </nav>

  <!-- Header -->
  <div class="header">
    <h1>Welcome to My Personal Website</h1>
    <p>Adriel Alva Dareen</p>
  </div>

  <!-- Cards -->
  <div class="card-container">
    <div class="card">
      <img src="C:\Users\User\Pictures\Saved Pictures\el edit.jpeg" alt="About Me">
      <div class="card-content">
        <h3>About Me</h3>
      </div>
    </div>

    <div class="card">
      <img src="C:\Users\User\Pictures\Saved Pictures\jadwal pelajaran.jpeg" alt="Schedule">
      <div class="card-content">
        <h3>Schedule</h3>
      </div>
    </div>

    <div class="card">
      <img src="C:\Users\User\Pictures\Saved Pictures\song.jpeg" alt="Music">
      <div class="card-content">
        <h3>Music</h3>
      </div>
    </div>
  </div>

</body>
</html>
<!doctype html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>📅 Jadwal Pelajaran</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: linear-gradient(135deg, #e8f5e9, #c8e6c9);
      margin: 0;
      padding: 20px;
    }

    h1 {
      text-align: center;
      margin-bottom: 25px;
      color: #2e7d32;
      text-shadow: 1px 1px 3px rgba(0,0,0,0.15);
    }

    .table-container {
      overflow-x: auto;
      background: #fff;
      padding: 20px;
      border-radius: 15px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.15);
      animation: fadeIn 1s ease;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      font-size: 14px;
      min-width: 600px;
    }

    thead {
      background: #2e7d32;
      color: white;
      position: sticky;
      top: 0;
      z-index: 2;
    }

    th, td {
      border: 1px solid #ddd;
      padding: 12px;
      text-align: center;
      transition: all 0.3s ease;
    }

    th {
      font-weight: bold;
      text-transform: uppercase;
      letter-spacing: 0.5px;
    }

    tbody tr:nth-child(even) {
      background: #b0fa84;
    }

    tbody tr:hover {
      background: #a5d6a7;
      color: white;
      transform: scale(1.01);
      cursor: pointer;
    }

    /* Efek animasi masuk */
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(15px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>
  <h1>📚 Jadwal Pelajaran (WIB)</h1>
  
  <div class="table-container">
    <table>
      <thead>
        <tr>
          <th>Jam</th>
          <th>Senin</th>
          <th>Selasa</th>
          <th>Rabu</th>
          <th>Kamis</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>07:00 - 07:40</td>
          <td>Upacara</td>
          <td>Kejuruan</td>
          <td>Bahasa Inggris</td>
          <td>Kejuruan</td>
        </tr>
        <tr>
          <td>07:40 - 08:20</td>
          <td>Kejuruan</td>
          <td>Kejuruan</td>
          <td>Bahasa Inggris</td>
          <td>Kejuruan</td>
        </tr>
        <tr>
          <td>08:20 - 09:00</td>
          <td>Kejuruan</td>
          <td>Kejuruan</td>
          <td>Kejuruan</td>
          <td>Kejuruan</td>
        </tr>
        <tr>
          <td>09:00 - 09:40</td>
          <td>Kejuruan</td>
          <td>Kejuruan</td>
          <td>Bahasa Inggris</td>
          <td>Bahasa Indonesia</td>
        </tr>
        <tr>
          <td>09:40 - 10:00</td>
          <td colspan="4">☕ Istirahat</td>
        </tr>
        <tr>
          <td>10:00 - 10:40</td>
          <td>Kejuruan</td>
          <td>Matematika</td>
          <td>Kejuruan</td>
          <td>Pendidikan Agama Islam</td>
        </tr>
        <tr>
          <td>10:40 - 11:20</td>
          <td>Kejuruan</td>
          <td>Matenatika</td>
          <td>Kejuruan</td>
          <td>Pendidikan Agama Islam</td>
        </tr>
        <tr>
          <td>11:20 - 12:00</td>
          <td>Kejuruan</td>
          <td>Matematika</td>
          <td>Kejuruan</td>
          <td>Pendidikan Agama Islam</td>
        </tr>
        <tr>
          <td>12:00 - 12:45</td>
          <td colspan="4">🍱 Istirahat</td>
        </tr>
        <tr>
          <td>12:45 - 13:25</td>
          <td>Kejuruan</td>
          <td>Kejuruan</td>
          <td>Kejuruan</td>
          <td>Kejuruan</td>
        </tr>
        <tr>
          <td>13:25 - 14:05</td>
          <td>Kejuruan</td>
          <td>Kejuruan</td>
          <td>Kejuruan</td>
          <td>Kejuruan</td>
        </tr>
        <tr>
          <td>14:05 - 14:45</td>
          <td>Kejuruan</td>
          <td>Kejuruan</td>
          <td>PKK</td>
          <td>Bahasa Korea</td>
        </tr>
        <tr>
          <td>14:45 - 15:25</td>
          <td>Kejuruan</td>
          <td>Kejuruan</td>
          <td>PKK</td>
          <td>Bahasa Korea</td>
        </tr>
      </tbody>
    </table>
  </div>

  <br>

  <!-- Tabel Jumat -->
  <div class="table-container" style="max-width: 500px; margin: auto;">
    <table>
      <thead>
        <tr>
          <th>Jam (WIB)</th>
          <th>Jumat</th>
        </tr>
      </thead>
      <tbody>
        <tr><td>07:00 - 07:40</td><td>Pengajian</td></tr>
        <tr><td>07:40 - 08:20</td><td>PKK</td></tr>
        <tr><td>08:20 - 09:00</td><td>PKK</td></tr>
        <tr><td>09:00 - 09:40</td><td>PKK</td></tr>
        <tr><td>09:40 - 10:00</td><td>☕ Istirahat</td></tr>
        <tr><td>10:00 - 10:40</td><td>Bahasa Indonea</td></tr>
        <tr><td>10:40 - 11:20</td><td>Bahasa Indonesia</td></tr>
        <tr><td>11:20 - 11:50</td><td>🍱 Istirahat</td></tr>
        <tr><td>11:50 - 12:50</td><td>🍱 Istirahat</td></tr>
        <tr><td>12:50 - 14:00</td><td>🍱 Istirahat</td></tr>
        <tr><td>14:00 - 17:00</td><td>🎯 Ekstrakurikuler</td></tr>
      </tbody>
    </table>
  </div>

</body>
</html>

```
