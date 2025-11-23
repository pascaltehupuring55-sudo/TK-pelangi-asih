<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>KB PAUD Pelangi Asih 3 Soalena</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f5f7fa;
            color: #333;
            line-height: 1.6;
            padding: 10px;
            font-size: 14px;
        }
        
        .container {
            max-width: 100%;
            margin: 0 auto;
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            padding: 15px;
            position: relative;
            overflow-x: hidden;
        }
        
        header {
            text-align: center;
            margin-bottom: 20px;
            padding-bottom: 15px;
            border-bottom: 2px solid #4a90e2;
        }
        
        h1 {
            color: #2c3e50;
            margin-bottom: 8px;
            font-size: 20px;
            line-height: 1.3;
        }
        
        h2 {
            color: #3498db;
            font-size: 16px;
            margin-bottom: 15px;
        }
        
        h3 {
            color: #2c3e50;
            margin: 20px 0 12px;
            padding-bottom: 6px;
            border-bottom: 1px solid #e1e1e1;
            font-size: 18px;
        }
        
        .nav-tabs {
            display: flex;
            margin-bottom: 15px;
            border-bottom: 1px solid #ddd;
            overflow-x: auto;
            white-space: nowrap;
            -webkit-overflow-scrolling: touch;
        }
        
        .tab-button {
            padding: 10px 15px;
            background: none;
            border: none;
            cursor: pointer;
            font-size: 14px;
            font-weight: 600;
            color: #7f8c8d;
            border-bottom: 3px solid transparent;
            transition: all 0.3s;
            flex-shrink: 0;
        }
        
        .tab-button.active {
            color: #3498db;
            border-bottom: 3px solid #3498db;
        }
        
        .tab-content {
            display: none;
        }
        
        .tab-content.active {
            display: block;
        }
        
        .table-container {
            overflow-x: auto;
            margin-bottom: 20px;
            -webkit-overflow-scrolling: touch;
        }
        
        table {
            width: 100%;
            border-collapse: collapse;
            margin-bottom: 15px;
            min-width: 600px;
        }
        
        th, td {
            padding: 10px 8px;
            text-align: left;
            border-bottom: 1px solid #e1e1e1;
            font-size: 12px;
        }
        
        th {
            background-color: #3498db;
            color: white;
            font-weight: 600;
            position: sticky;
            left: 0;
        }
        
        tr:nth-child(even) {
            background-color: #f8f9fa;
        }
        
        tr:hover {
            background-color: #e8f4fc;
        }
        
        .gender-male {
            color: #3498db;
            font-weight: bold;
        }
        
        .gender-female {
            color: #e84393;
            font-weight: bold;
        }
        
        .summary {
            background-color: #e8f4fc;
            padding: 12px;
            border-radius: 8px;
            margin-top: 15px;
            font-size: 14px;
        }
        
        .summary h3 {
            color: #2c3e50;
            margin-bottom: 8px;
            border-bottom: none;
            font-size: 16px;
        }
        
        .summary p {
            margin-bottom: 6px;
        }
        
        footer {
            text-align: center;
            margin-top: 20px;
            padding-top: 15px;
            border-top: 1px solid #e1e1e1;
            color: #7f8c8d;
            font-size: 14px;
        }
        
        .student-details {
            display: none;
            margin-top: 15px;
            padding: 15px;
            background-color: #f8f9fa;
            border-radius: 8px;
            border-left: 4px solid #3498db;
        }
        
        .student-details.active {
            display: block;
        }
        
        .evaluation-section {
            margin-bottom: 15px;
        }
        
        .evaluation-section h4 {
            color: #2c3e50;
            margin-bottom: 8px;
            font-size: 16px;
        }
        
        .evaluation-content {
            background-color: white;
            padding: 12px;
            border-radius: 6px;
            border: 1px solid #e1e1e1;
            font-size: 14px;
        }
        
        .back-button {
            background-color: #7f8c8d;
            color: white;
            border: none;
            padding: 10px 15px;
            border-radius: 4px;
            cursor: pointer;
            margin-bottom: 12px;
            font-size: 14px;
            width: 100%;
        }
        
        .back-button:hover {
            background-color: #6c7b7d;
        }
        
        .view-nilai-btn {
            background-color: #3498db;
            color: white;
            border: none;
            padding: 6px 10px;
            border-radius: 4px;
            cursor: pointer;
            font-size: 12px;
            white-space: nowrap;
        }
        
        .view-nilai-btn:hover {
            background-color: #2980b9;
        }
        
        /* Login Styles */
        .login-container {
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 80vh;
            padding: 10px;
        }
        
        .login-form {
            background-color: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            width: 100%;
            max-width: 400px;
        }
        
        .login-form h2 {
            text-align: center;
            margin-bottom: 20px;
            color: #2c3e50;
            font-size: 20px;
        }
        
        .user-type-selector {
            display: flex;
            margin-bottom: 15px;
            border-radius: 4px;
            overflow: hidden;
            border: 1px solid #ddd;
        }
        
        .user-type-option {
            flex: 1;
            padding: 12px 8px;
            text-align: center;
            background-color: #f8f9fa;
            cursor: pointer;
            transition: all 0.3s;
            font-size: 14px;
        }
        
        .user-type-option.active {
            background-color: #3498db;
            color: white;
        }
        
        .form-group {
            margin-bottom: 15px;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 6px;
            font-weight: 600;
            color: #2c3e50;
            font-size: 14px;
        }
        
        .form-group input, .form-group select {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 4px;
            font-size: 16px; /* Larger for mobile */
            transition: border-color 0.3s;
            -webkit-appearance: none;
        }
        
        .form-group input:focus, .form-group select:focus {
            border-color: #3498db;
            outline: none;
        }
        
        .login-button {
            width: 100%;
            padding: 14px;
            background-color: #3498db;
            color: white;
            border: none;
            border-radius: 4px;
            font-size: 16px;
            cursor: pointer;
            transition: background-color 0.3s;
            margin-top: 10px;
        }
        
        .login-button:hover {
            background-color: #2980b9;
        }
        
        .error-message {
            color: #e74c3c;
            margin-top: 10px;
            text-align: center;
            display: none;
            font-size: 14px;
        }
        
        .logout-button {
            position: absolute;
            top: 15px;
            right: 15px;
            background-color: #e74c3c;
            color: white;
            border: none;
            padding: 8px 12px;
            border-radius: 4px;
            cursor: pointer;
            font-size: 12px;
            z-index: 100;
        }
        
        .logout-button:hover {
            background-color: #c0392b;
        }
        
        .user-info {
            position: absolute;
            top: 15px;
            right: 100px;
            color: #2c3e50;
            font-weight: 600;
            font-size: 14px;
            text-align: right;
            max-width: 150px;
        }
        
        .user-role {
            background-color: #3498db;
            color: white;
            padding: 3px 6px;
            border-radius: 4px;
            font-size: 10px;
            margin-left: 5px;
            display: inline-block;
        }
        
        .parent-child-select {
            margin-bottom: 15px;
        }
        
        .parent-child-select select {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 4px;
            font-size: 16px;
        }
        
        /* Mobile-specific improvements */
        @media (max-width: 480px) {
            body {
                padding: 5px;
                font-size: 13px;
            }
            
            .container {
                padding: 10px;
                border-radius: 8px;
            }
            
            h1 {
                font-size: 18px;
            }
            
            h2 {
                font-size: 14px;
            }
            
            h3 {
                font-size: 16px;
            }
            
            .tab-button {
                padding: 8px 12px;
                font-size: 13px;
            }
            
            th, td {
                padding: 8px 6px;
                font-size: 11px;
            }
            
            .logout-button, .user-info {
                position: relative;
                top: 0;
                right: 0;
                margin-bottom: 10px;
                text-align: center;
            }
            
            .user-info {
                max-width: 100%;
                margin-bottom: 5px;
            }
            
            .login-form {
                padding: 15px;
            }
            
            .login-form h2 {
                font-size: 18px;
            }
            
            .user-type-option {
                padding: 10px 6px;
                font-size: 13px;
            }
            
            .form-group input, .form-group select {
                padding: 14px;
                font-size: 16px;
            }
            
            .login-button {
                padding: 16px;
            }
            
            .summary {
                padding: 10px;
                font-size: 13px;
            }
            
            .evaluation-content {
                padding: 10px;
                font-size: 13px;
            }
            
            .back-button {
                padding: 12px;
            }
        }
        
        @media (max-width: 360px) {
            h1 {
                font-size: 16px;
            }
            
            h2 {
                font-size: 13px;
            }
            
            .tab-button {
                padding: 6px 10px;
                font-size: 12px;
            }
            
            th, td {
                padding: 6px 4px;
                font-size: 10px;
            }
        }
        
        /* Touch improvements */
        button, .tab-button, .user-type-option {
            -webkit-tap-highlight-color: transparent;
            touch-action: manipulation;
        }
        
        input, select {
            -webkit-tap-highlight-color: transparent;
        }
        
        /* Loading indicator */
        .loading {
            display: none;
            text-align: center;
            padding: 20px;
        }
        
        .spinner {
            border: 4px solid #f3f3f3;
            border-top: 4px solid #3498db;
            border-radius: 50%;
            width: 40px;
            height: 40px;
            animation: spin 1s linear infinite;
            margin: 0 auto;
        }
        
        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
    </style>
</head>
<body>
    <!-- Login Screen -->
    <div id="login-screen" class="login-container">
        <div class="login-form">
            <h2>Login KB PAUD Pelangi Asih 3 Soalena</h2>
            
            <div class="user-type-selector">
                <div class="user-type-option active" data-type="admin">Admin</div>
                <div class="user-type-option" data-type="guru">Guru</div>
                <div class="user-type-option" data-type="orangtua">Orangtua</div>
            </div>
            
            <div class="form-group">
                <label for="username">Nama</label>
                <input type="text" id="username" placeholder="Masukkan nama">
            </div>
            
            <div class="form-group">
                <label for="password">Password</label>
                <input type="password" id="password" placeholder="Masukkan password">
            </div>
            
            <!-- Selector untuk orangtua (hanya tampil jika tipe pengguna orangtua) -->
            <div id="parent-child-select" class="parent-child-select" style="display: none;">
                <label for="child-select">Pilih Anak</label>
                <select id="child-select">
                    <option value="">-- Pilih Anak --</option>
                </select>
            </div>
            
            <button class="login-button" onclick="login()">Login</button>
            <div id="login-error" class="error-message">Nama atau password salah!</div>
            
            <div class="loading" id="login-loading">
                <div class="spinner"></div>
                <p>Memproses login...</p>
            </div>
        </div>
    </div>
    
    <!-- Main Content (Initially Hidden) -->
    <div id="main-content" class="container" style="display: none;">
        <div class="user-info">
            <span id="current-user">User</span>
            <span id="user-role" class="user-role">Role</span>
        </div>
        <button class="logout-button" onclick="logout()">Logout</button>
        
        <header>
            <h1>KB PAUD PELANGI ASIH 3 SOALENA</h1>
            <h2>DATA SISWA DAN NILAI TAHUN AJARAN 2025 - 2026</h2>
        </header>
        
        <!-- Tab Navigation (Tampil untuk Admin dan Guru) -->
        <div id="nav-tabs" class="nav-tabs" style="display: none;">
            <button class="tab-button active" onclick="openTab('siswa')">Data Siswa</button>
            <button class="tab-button" onclick="openTab('guru')">Data Guru</button>
            <button class="tab-button" onclick="openTab('kontrak')">Riwayat Kontrak</button>
        </div>
        
        <!-- Tab Data Siswa -->
        <div id="siswa" class="tab-content active">
            <h3>Data Siswa</h3>
            <div class="table-container">
                <table>
                    <thead>
                        <tr>
                            <th>NO.</th>
                            <th>NAMA SISWA</th>
                            <th>L/P</th>
                            <th>TTL</th>
                            <th>NIK</th>
                            <th>NILAI</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>1</td>
                            <td>JULLIA OLHA TESLATU</td>
                            <td class="gender-female">P</td>
                            <td>Nabire, 23-09-2019</td>
                            <td>8106076309190001</td>
                            <td><button class="view-nilai-btn" onclick="showStudentDetails(1)">Lihat</button></td>
                        </tr>
                        <tr>
                            <td>2</td>
                            <td>ROSARIO VINCENT C TETERISSA</td>
                            <td class="gender-male">L</td>
                            <td>Kamal, 19-06-2020</td>
                            <td>8106071906200001</td>
                            <td><button class="view-nilai-btn" onclick="showStudentDetails(2)">Lihat</button></td>
                        </tr>
                        <tr>
                            <td>3</td>
                            <td>MARIA ALENA MAIPAUW</td>
                            <td class="gender-female">P</td>
                            <td>Sendawar, 02-11-2019</td>
                            <td>6407074211190000</td>
                            <td><button class="view-nilai-btn" onclick="showStudentDetails(3)">Lihat</button></td>
                        </tr>
                        <!-- Data siswa lainnya (disingkat untuk contoh) -->
                    </tbody>
                </table>
            </div>
            
            <div class="summary">
                <h3>Ringkasan Data Siswa</h3>
                <p><strong>Jumlah Total Siswa:</strong> 27</p>
                <p><strong>Jumlah Siswa Laki-laki:</strong> 11</p>
                <p><strong>Jumlah Siswa Perempuan:</strong> 16</p>
                <p><strong>Tahun Ajaran:</strong> 2025 - 2026</p>
            </div>
            
            <!-- Detail Siswa dan Nilai -->
            <div id="student-details" class="student-details">
                <button class="back-button" onclick="hideStudentDetails()">← Kembali ke Daftar Siswa</button>
                <h3 id="student-name">Nama Siswa</h3>
                
                <div class="evaluation-section">
                    <h4>LITERASI & MATEMATIKA</h4>
                    <div class="evaluation-content" id="literasi-math">
                        Evaluasi akan ditampilkan di sini
                    </div>
                </div>
                
                <div class="evaluation-section">
                    <h4>PROJEK PANCASILA</h4>
                    <div class="evaluation-content" id="projek-pancasila">
                        Evaluasi akan ditampilkan di sini
                    </div>
                </div>
                
                <div class="evaluation-section">
                    <h4>AGAMA & BUDI PEKERTI</h4>
                    <div class="evaluation-content" id="agama-budipekerti">
                        Evaluasi akan ditampilkan di sini
                    </div>
                </div>
                
                <div class="evaluation-section">
                    <h4>JATI DIRI</h4>
                    <div class="evaluation-content" id="jati-diri">
                        Evaluasi akan ditampilkan di sini
                    </div>
                </div>
            </div>
        </div>
        
        <!-- Tab Data Guru -->
        <div id="guru" class="tab-content">
            <h3>Data Guru</h3>
            <div class="table-container">
                <table>
                    <thead>
                        <tr>
                            <th>NO.</th>
                            <th>NAMA</th>
                            <th>JK</th>
                            <th>TTL</th>
                            <th>STATUS</th>
                            <th>JABATAN</th>
                        </tr>
                    </thead>
                    <tbody>
                        <t
