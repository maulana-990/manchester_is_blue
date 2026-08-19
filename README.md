[porto.html](https://github.com/user-attachments/files/30732351/porto.html)

<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fuad Maulana - Portfolio</title>
    <!-- Font Awesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts (Poppins) -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #6c5ce7;[variable.php](https://github.com/user-attachments/files/30732365/variable.php)
[style.css](https://github.com/user-attachments/files/30732359/style.css)
[siswa.php](https://github.com/user-attachments/files/30732358/siswa.php)

            --primary-light: #a29bfe;
            --primary-dark: #5140ed;
            --purple-bg: #f3f0ff;
            --card-bg: #ffffff;
            --text-main: #2d3436;
            --text-muted: #636e72;
            --border-color: #e2e8f0;
            --radius-lg: 16px;
            --radius-md: 10px;
            --radius-sm: 6px;
            --shadow: 0 10px 30px rgba(108, 92, 231, 0.08);
            --shadow-sm: 0 4px 12px rgba(0,0,0,0.05);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }

        body {
            background-color: #f8f9fa;
            color: var(--text-main);
            line-height: 1.6;
            padding-bottom: 20px;
        }

        .container {
            max-width: 1140px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* HEADER / NAVBAR */
        header {
            background: #fff;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 15px rgba(0,0,0,0.04);
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 70px;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 12px;
            font-size: 1.25rem;
            font-weight: 700;
            color: #1e293b;
        }

        .logo-badge {
            background: var(--primary);
            color: white;
            padding: 6px 12px;
            border-radius: 8px;
            font-weight: 800;
            font-size: 1.1rem;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 25px;
        }

        .nav-links a {
            text-decoration: none;
            color: #475569;
            font-weight: 500;
            font-size: 0.95rem;
            transition: all 0.3s;
            position: relative;
            padding-bottom: 4px;
        }

        .nav-links a:hover, .nav-links a.active {
            color: var(--primary);
        }

        .nav-links a.active::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 3px;
            background: var(--primary);
            border-radius: 2px;
        }

        /* HERO SECTION */
        .hero {
            padding: 60px 0 40px;
            background: linear-gradient(135deg, #f8f9ff 0%, #f1f0fe 100%);
            border-radius: 0 0 30px 30px;
            margin-bottom: 40px;
            position: relative;
            overflow: hidden;
        }

        .hero-grid {
            display: grid;
            grid-template-columns: 400px 1fr;
            gap: 50px;
            align-items: center;
        }

        .hero-img-wrapper {
            position: relative;
            display: flex;
            justify-content: center;
        }

        .hero-img-bg {
            width: 320px;
            height: 320px;
            background: #dcd6ff;
            border-radius: 50%;
            position: absolute;
            bottom: 0;
            z-index: 1;
        }

        .hero-img {
            width: 330px;
            height: 380px;
            object-fit: cover;
            position: relative;
            z-index: 2;
            border-bottom-left-radius: 160px;
            border-bottom-right-radius: 160px;
        }

        .hero-content h3 {
            font-size: 1.25rem;
            color: #475569;
            font-weight: 500;
            margin-bottom: 5px;
        }

        .hero-content h1 {
            font-size: 2.8rem;
            font-weight: 800;
            color: #0f172a;
            line-height: 1.2;
            margin-bottom: 8px;
        }

        .hero-content h2 {
            font-size: 1.4rem;
            color: var(--primary);
            font-weight: 600;
            margin-bottom: 20px;
        }

        .hero-content p {
            color: #64748b;
            font-size: 0.98rem;
            max-width: 580px;
            margin-bottom: 30px;
            line-height: 1.7;
        }

        .hero-btns {
            display: flex;
            gap: 15px;
            margin-bottom: 30px;
        }

        .btn {
            padding: 12px 24px;
            border-radius: 8px;
            font-weight: 600;
            text-decoration: none;
            display: inline-flex;
            align-items: center;
            gap: 8px;
            font-size: 0.95rem;
            transition: all 0.3s;
            cursor: pointer;
        }

        .btn-primary {
            background: var(--primary);
            color: white;
            box-shadow: 0 4px 15px rgba(108, 92, 231, 0.3);
            border: none;
        }

        .btn-primary:hover {
            background: var(--primary-dark);
            transform: translateY(-2px);
        }

        .btn-outline {
            background: transparent;
            color: var(--primary);
            border: 2px solid var(--primary);
        }

        .btn-outline:hover {
            background: rgba(108, 92, 231, 0.05);
            transform: translateY(-2px);
        }

        .social-links {
            display: flex;
            gap: 15px;
        }

        .social-icon {
            width: 40px;
            height: 40px;
            border-radius: 8px;
            background: white;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #334155;
            text-decoration: none;
            box-shadow: 0 2px 8px rgba(0,0,0,0.06);
            transition: all 0.3s;
            font-size: 1.1rem;
        }

        .social-icon:hover {
            background: var(--primary);
            color: white;
            transform: translateY(-3px);
        }

        /* SECTION STYLES */
        .section-card {
            background: white;
            border-radius: var(--radius-lg);
            padding: 30px;
            margin-bottom: 30px;
            box-shadow: var(--shadow-sm);
            border: 1px solid #f1f5f9;
        }

        .section-header {
            display: flex;
            align-items: center;
            gap: 12px;
            margin-bottom: 25px;
        }

        .icon-box {
            width: 42px;
            height: 42px;
            background: var(--primary);
            color: white;
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.2rem;
        }

        .section-title {
            font-size: 1.35rem;
            font-weight: 700;
            color: #0f172a;
            letter-spacing: 0.5px;
            text-transform: uppercase;
        }

        /* TENTANG SAYA */
        .tentang-grid {
            display: grid;
            grid-template-columns: 1fr 1.2fr;
            gap: 40px;
        }

        .tentang-desc {
            color: #475569;
            font-size: 0.95rem;
            line-height: 1.8;
        }

        .info-table {
            width: 100%;
            border-collapse: collapse;
        }

        .info-table tr {
            border-bottom: 1px dashed #f1f5f9;
        }

        .info-table tr:last-child {
            border-bottom: none;
        }

        .info-table td {
            padding: 8px 0;
            font-size: 0.92rem;
        }

        .info-label {
            font-weight: 600;
            color: #334155;
            width: 160px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .info-label i {
            color: var(--primary);
            width: 16px;
        }

        .info-colon {
            width: 20px;
            color: #94a3b8;
        }

        .info-val {
            color: #475569;
            font-weight: 500;
        }

        /* GRID 2 COLUMNS FOR MID SECTIONS */
        .grid-2 {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
        }

        .grid-2-custom {
            display: grid;
            grid-template-columns: 1fr 1.2fr;
            gap: 30px;
        }

        /* PENDIDIKAN & PENGALAMAN TIMELINE */
        .timeline {
            position: relative;
            padding-left: 20px;
        }

        .timeline::before {
            content: '';
            position: absolute;
            left: 4px;
            top: 8px;
            bottom: 8px;
            width: 2px;
            background: #e2e8f0;
        }

        .timeline-item {
            position: relative;
            margin-bottom: 25px;
        }

        .timeline-item:last-child {
            margin-bottom: 0;
        }

        .timeline-dot {
            position: absolute;
            left: -20px;
            top: 6px;
            width: 10px;
            height: 10px;
            border-radius: 50%;
            background: var(--primary);
            border: 2px solid white;
            box-shadow: 0 0 0 2px var(--primary);
        }

        .timeline-date {
            font-size: 0.85rem;
            font-weight: 700;
            color: var(--primary);
            margin-bottom: 4px;
        }

        .timeline-title {
            font-size: 1rem;
            font-weight: 700;
            color: #1e293b;
        }

        .timeline-subtitle {
            font-size: 0.88rem;
            color: #64748b;
            margin-bottom: 4px;
        }

        /* KEAHLIAN / SKILLS */
        .skill-item {
            margin-bottom: 18px;
        }

        .skill-info {
            display: flex;
            justify-content: space-between;
            margin-bottom: 6px;
            font-size: 0.9rem;
            font-weight: 600;
            color: #334155;
        }

        .skill-bar-bg {
            height: 8px;
            background: #e2e8f0;
            border-radius: 10px;
            overflow: hidden;
        }

        .skill-bar-fill {
            height: 100%;
            background: var(--primary);
            border-radius: 10px;
        }

        /* TOOLS & TEKNOLOGI */
        .tools-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 15px;
        }

        .tool-card {
            background: #f8fafc;
            border: 1px solid #f1f5f9;
            border-radius: 12px;
            padding: 15px;
            text-align: center;
            transition: all 0.3s;
        }

        .tool-card:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 15px rgba(0,0,0,0.05);
            border-color: #cbd5e1;
        }

        .tool-icon {
            height: 40px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 8px;
            font-size: 2rem;
        }

        .tool-name {
            font-size: 0.8rem;
            font-weight: 600;
            color: #475569;
        }

        /* PORTOFOLIO / PROYEK */
        .portfolio-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
        }

        .project-card {
            border-radius: 12px;
            overflow: hidden;
            border: 1px solid #e2e8f0;
            background: #fff;
            transition: all 0.3s;
        }

        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 12px 25px rgba(0,0,0,0.08);
        }

        .project-img {
            width: 100%;
            height: 180px;
            object-fit: cover;
            background: #cbd5e1;
            border-bottom: 1px solid #e2e8f0;
        }

        .project-body {
            padding: 20px;
        }

        .project-title {
            font-size: 1.05rem;
            font-weight: 700;
            color: #0f172a;
            margin-bottom: 8px;
        }

        .project-desc {
            font-size: 0.85rem;
            color: #64748b;
            margin-bottom: 15px;
            line-height: 1.5;
            height: 55px;
        }

        .project-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 6px;
        }

        .tag {
            padding: 4px 10px;
            border-radius: 6px;
            font-size: 0.72rem;
            font-weight: 700;
            color: white;
        }

        .tag-orange { background: #ff7675; }
        .tag-blue { background: #74b9ff; }
        .tag-yellow { background: #fdcb6e; color: #2d3436; }
        .tag-purple { background: #a29bfe; }

        /* SERTIFIKAT */
        .cert-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 15px;
            margin-bottom: 15px;
        }

        .cert-img {
            width: 100%;
            height: 100px;
            object-fit: cover;
            border-radius: 8px;
            border: 1px solid #e2e8f0;
        }

        .cert-list {
            list-style: none;
            margin-bottom: 20px;
        }

        .cert-list li {
            font-size: 0.88rem;
            color: #475569;
            margin-bottom: 6px;
            position: relative;
            padding-left: 15px;
        }

        .cert-list li::before {
            content: '•';
            color: var(--primary);
            font-weight: bold;
            position: absolute;
            left: 0;
        }

        /* PRESTASI */
        .prestasi-list {
            list-style: none;
        }

        .prestasi-item {
            display: flex;
            align-items: center;
            gap: 10px;
            margin-bottom: 12px;
            font-size: 0.9rem;
            color: #334155;
            font-weight: 500;
        }

        .prestasi-item i {
            color: var(--primary);
        }

        /* KONTAK */
        .contact-grid {
            display: grid;
            grid-template-columns: repeat(5, 1fr);
            gap: 15px;
        }

        .contact-card {
            background: #f8fafc;
            border: 1px solid #f1f5f9;
            border-radius: 12px;
            padding: 15px;
            display: flex;
            align-items: center;
            gap: 12px;
            text-decoration: none;
            color: inherit;
            transition: all 0.3s;
        }

        .contact-card:hover {
            border-color: var(--primary);
            background: #fff;
            box-shadow: 0 4px 12px rgba(108, 92, 231, 0.1);
        }

        .contact-icon {
            width: 38px;
            height: 38px;
            border-radius: 8px;
            background: #f1f0fe;
            color: var(--primary);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.1rem;
            flex-shrink: 0;
        }

        .contact-info label {
            display: block;
            font-size: 0.75rem;
            color: #94a3b8;
            font-weight: 600;
        }

        .contact-info span {
            font-size: 0.82rem;
            font-weight: 600;
            color: #334155;
            word-break: break-all;
        }

        /* FOOTER */
        footer {
            background: #1e1b4b;
            color: white;
            text-align: center;
            padding: 25px 0;
            margin-top: 40px;
            font-size: 0.88rem;
            position: relative;
        }

        footer p {
            color: #cbd5e1;
            margin-bottom: 4px;
        }

        footer i.fa-heart {
            color: #ef4444;
        }

        .scroll-top {
            position: fixed;
            bottom: 30px;
            right: 30px;
            width: 45px;
            height: 45px;
            background: var(--primary);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            text-decoration: none;
            box-shadow: 0 4px 15px rgba(108, 92, 231, 0.4);
            transition: all 0.3s;
            z-index: 99;
        }

        .scroll-top:hover {
            transform: translateY(-3px);
            background: var(--primary-dark);
        }

        /* RESPONSIVE DESIGN */
        @media (max-width: 992px) {
            .hero-grid {
                grid-template-columns: 1fr;
                text-align: center;
            }
            .hero-content p {
                margin: 0 auto 30px;
            }
            .hero-btns, .social-links {
                justify-content: center;
            }
            .tentang-grid, .grid-2, .grid-2-custom {
                grid-template-columns: 1fr;
            }
            .portfolio-grid {
                grid-template-columns: 1fr 1fr;
            }
            .contact-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        @media (max-width: 600px) {
            .nav-links {
                display: none; /* Hide on mobile for simplicity */
            }
            .portfolio-grid {
                grid-template-columns: 1fr;
            }
            .tools-grid {
                grid-template-columns: repeat(2, 1fr);
            }
            .contact-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>

    <!-- NAVBAR -->
    <header>
        <div class="container navbar">
            <div class="logo">
                <span class="logo-badge">FM</span>
                <span>Fuad Maulana</span>
            </div>
            <ul class="nav-links">
                <li><a href="#home" class="active">Home</a></li>
                <li><a href="#tentang">Tentang Saya</a></li>
                <li><a href="#pendidikan">Pendidikan</a></li>
                <li><a href="#keahlian">Keahlian</a></li>
                <li><a href="#portofolio">Portofolio</a></li>
                <li><a href="#sertifikat">Sertifikat</a></li>
                <li><a href="#pengalaman">Pengalaman</a></li>
                <li><a href="#kontak">Kontak</a></li>
            </ul>
        </div>
    </header>

    <!-- HERO SECTION -->
    <section id="home" class="hero">
        <div class="container hero-grid">
            <div class="hero-img-wrapper">
                <div class="hero-img-bg"></div>
                <!-- Placeholder image representing photo -->
                <img src="ey.png" alt="Fuad Maulana" class="hero-img">
            </div>
            <div class="hero-content">
                <h3>Halo, saya</h3>
                <h1>Fuad Maulana</h1>
                <h2>Web Developer | UI/UX Designer</h2>
                <p>Saya adalah lulusan MTS Al-Huda tahun ajaran 2021-2024.</p>
                <div class="hero-btns">
                    <a href="#portofolio" class="btn btn-primary"><i class="fas fa-folder-open"></i> Lihat Portofolio</a>
                    <a href="#kontak" class="btn btn-outline"><i class="fas fa-paper-plane"></i> Hubungi Saya</a>
                </div>
                <div class="social-links">
                    <a href="https://github.com" class="social-icon" target="_blank"><i class="fab fa-github"></i></a>
                    <a href="https://linkedin.com" class="social-icon" target="_blank"><i class="fab fa-linkedin-in"></i></a>
                    <a href="https://instagram.com" class="social-icon" target="_blank"><i class="fab fa-instagram"></i></a>
                    <a href="dauffildaf@gmail.com" class="social-icon"><i class="fas fa-envelope"></i></a>
                    <a href="abdulmarix@gmail.com" class="social-icon"><i class="fas fa-envelope"></i></a>
                </div>
            </div>
        </div>
    </section>

    <div class="container">

        <!-- TENTANG SAYA -->
        <section id="tentang" class="section-card">
            <div class="section-header">
                <div class="icon-box"><i class="fas fa-user"></i></div>
                <h2 class="section-title">Tentang Saya</h2>
            </div>
            <div class="tentang-grid">
                <div class="tentang-desc">
                    <p>Saya adalah seorang pengembang web dan desainer antarmuka yang memiliki ketertarikan di bidang teknologi informasi. Saya memiliki kemampuan dalam membangun website yang responsif, menarik, dan mudah digunakan. Saya selalu berusaha memberikan hasil terbaik dalam setiap proyek yang saya kerjakan.</p>
                </div>
                <div>
                    <table class="info-table">
                        <tr>
                            <td class="info-label"><i class="fas fa-user"></i> Nama Lengkap</td>
                            <td class="info-colon">:</td>
                            <td class="info-val">Fuad Maulana</td>
                        </tr>
                        <tr>
                            <td class="info-label"><i class="fas fa-calendar-alt"></i> Tempat, Tgl Lahir</td>
                            <td class="info-colon">:</td>
                            <td class="info-val">Bandung, 36 Demaret 20089</td>
                        </tr>
                        <tr>
                            <td class="info-label"><i class="fas fa-map-marker-alt"></i> Alamat</td>
                            <td class="info-colon">:</td>
                            <td class="info-val">Bandung, Jawa Barat</td>
                        </tr>
                        <tr>
                            <td class="info-label"><i class="fas fa-envelope"></i> Email</td>
                            <td class="info-colon">:</td>
                            <td class="info-val">dauffildaf@gmail.com</td>
                            <td class="info-val">abdulmarix@gmail.com</td>
                        </tr>
                        <tr>
                            <td class="info-label"><i class="fas fa-phone"></i> No. HP</td>
                            <td class="info-colon">:</td>
                            <td class="info-val">0897-3526-8255</td>
                            <td class="info-val">0858-6733-9362</td>
                        </tr>
                        <tr>
                            <td class="info-label"><i class="fas fa-briefcase"></i>Siswa</td>
                            <td class="info-colon">:</td>
                            <td class="info-val">Rekayasa Perangkat Lunak</td>
                        </tr>
                        <tr>
                            <td class="info-label"><i class="fas fa-graduation-cap"></i> Status</td>
                            <td class="info-colon">:</td>
                            <td class="info-val">Lulusan MTS AL-HUDA</td>
                        </tr>
                        <tr>
                            <td class="info-label"><i class="fas fa-heart"></i> Hobi</td>
                            <td class="info-colon">:</td>
                            <td class="info-val">Musican dan Sleep</td>
                        </tr>
                    </table>
                </div>
            </div>
        </section>

        <!-- PENDIDIKAN & KEAHLIAN / TOOLS -->
        <div class="grid-2">
            <!-- PENDIDIKAN -->
            <section id="pendidikan" class="section-card">
                <div class="section-header">
                    <div class="icon-box"><i class="fas fa-graduation-cap"></i></div>
                    <h2 class="section-title">Pendidikan</h2>
                </div>
                <div class="timeline">
                    <div class="timeline-item">
                        <div class="timeline-dot"></div>
                        <div class="timeline-date">2015 – 2021</div>
                        <div class="timeline-title">SDN BEOR SEMPUR 01</div>
                        <div class="timeline-subtitle"></div>
                    </div>
                    <div class="timeline-item">
                        <div class="timeline-dot"></div>
                        <div class="timeline-date">2021 – 2024</div>
                        <div class="timeline-title">MTS AL-HUDA</div>
                        <div class="timeline-subtitle">Keagamaan</div>
                    </div>
                    <div class="timeline-item">
                        <div class="timeline-dot"></div>
                        <div class="timeline-date">2024 – Sekarang</div>
                        <div class="timeline-title">SMK MUTHIA HARAPAN CICALENGKA</div>
                        <div class="timeline-subtitle">REKAYA PERANGKAT LUNAK (RPL)</div>
                    </div>
                </div>
            </section>

            <!-- KEAHLIAN -->
            <section id="keahlian" class="section-card">
                <div class="section-header">
                    <div class="icon-box"><i class="fas fa-code"></i></div>
                    <h2 class="section-title">Keahlian</h2>
                </div>
                <div class="skill-item">
                    <div class="skill-info">
                        <span>Valorant</span>
                        <span>1001%</span>
                    </div>
                    <div class="skill-bar-bg"><div class="skill-bar-fill" style="width: 90%;"></div></div>
                </div>
                <div class="skill-item">
                    <div class="skill-info">
                        <span>PES</span>
                        <span>1002%</span>
                    </div>
                    <div class="skill-bar-bg"><div class="skill-bar-fill" style="width: 85%;"></div></div>
                </div>
                <div class="skill-item">
                    <div class="skill-info">
                        <span>TURU</span>
                        <span>100%</span>
                    </div>
                    <div class="skill-bar-bg"><div class="skill-bar-fill" style="width: 80%;"></div></div>
                </div>
                <div class="skill-item">
                    <div class="skill-info">
                        <span>SLEEP</span>
                        <span>90%</span>
                    </div>
                    <div class="skill-bar-bg"><div class="skill-bar-fill" style="width: 75%;"></div></div>
                </div>
                <div class="skill-item">
                    <div class="skill-info">
                        <span>PB</span>
                        <span>1000%</span>
                    </div>
                    <div class="skill-bar-bg"><div class="skill-bar-fill" style="width: 80%;"></div></div>
                </div>
                <div class="skill-item">
                    <div class="skill-info">
                        <span>UI/UX Design (Figma)</span>
                        <span>50%</span>
                    </div>
                    <div class="skill-bar-bg"><div class="skill-bar-fill" style="width: 85%;"></div></div>
                </div>
            </section>
        </div>

        <!-- TOOLS & TEKNOLOGI -->
        <section class="section-card">
            <div class="section-header">
                <div class="icon-box"><i class="fas fa-laptop-code"></i></div>
                <h2 class="section-title">Tools & Teknologi</h2>
            </div>
            <div class="tools-grid">
                <div class="tool-card">
                    <div class="tool-icon" style="color: #e34f26;"><i class="fab fa-html5"></i></div>
                    <div class="tool-name">HTML</div>
                </div>
                <div class="tool-card">
                    <div class="tool-icon" style="color: #1572b6;"><i class="fab fa-css3-alt"></i></div>
                    <div class="tool-name">CSS</div>
                </div>
                <div class="tool-card">
                    <div class="tool-icon" style="color: #f7df1e;"><i class="fab fa-js"></i></div>
                    <div class="tool-name">JavaScript</div>
                </div>
                <div class="tool-card">
                    <div class="tool-icon" style="color: #777bb4;"><i class="fab fa-php"></i></div>
                    <div class="tool-name">PHP</div>
                </div>
                <div class="tool-card">
                    <div class="tool-icon" style="color: #00758f;"><i class="fas fa-database"></i></div>
                    <div class="tool-name">MySQL</div>
                </div>
                <div class="tool-card">
                    <div class="tool-icon" style="color: #f24e1e;"><i class="fab fa-figma"></i></div>
                    <div class="tool-name">Figma</div>
                </div>
                <div class="tool-card">
                    <div class="tool-icon" style="color: #007acc;"><i class="fas fa-code"></i></div>
                    <div class="tool-name">VS Code</div>
                </div>
                <div class="tool-card">
                    <div class="tool-icon" style="color: #f05032;"><i class="fab fa-git-alt"></i></div>
                    <div class="tool-name">Git & GitHub</div>
                </div>
                <div class="tool-card">
                    <div class="tool-icon" style="color: #7952b3;"><i class="fab fa-bootstrap"></i></div>
                    <div class="tool-name">Bootstrap</div>
                </div>
            </div>
        </section>

        <!-- PORTOFOLIO / PROYEK -->
        <section id="portofolio" class="section-card">
            <div class="section-header">
                <div class="icon-box"><i class="fas fa-briefcase"></i></div>
                <h2 class="section-title">Portofolio / Proyek</h2>
            </div>
            <div class="portfolio-grid">
                <!-- Project 1 -->
                <div class="project-card">
                    <img src="https://images.unsplash.com/photo-1562774053-701939374585?q=80&w=500&auto=format&fit=crop" alt="Website Sekolah" class="project-img">
                    <div class="project-body">
                        <div class="project-title">Website Sekolah</div>
                        <div class="project-desc">Website profil sekolah yang berisi informasi sekolah, berita, galeri, dan kontak.</div>
                        <div class="project-tags">
                            <span class="tag tag-orange">HTML</span>
                            <span class="tag tag-blue">CSS</span>
                            <span class="tag tag-yellow">JavaScript</span>
                        </div>
                    </div>
                </div>
                <!-- Project 2 -->
                <div class="project-card">
                    <img src="https://images.unsplash.com/photo-1507842217343-583bb7270b66?q=80&w=500&auto=format&fit=crop" alt="Sistem Informasi Perpustakaan" class="project-img">
                    <div class="project-body">
                        <div class="project-title">Sistem Informasi Perpustakaan</div>
                        <div class="project-desc">Aplikasi perpustakaan untuk mengelola data buku, peminjaman, dan anggota.</div>
                        <div class="project-tags">
                            <span class="tag tag-purple">PHP</span>
                            <span class="tag tag-blue">MySQL</span>
                            <span class="tag tag-purple">Bootstrap</span>
                        </div>
                    </div>
                </div>
                <!-- Project 3 -->
                <div class="project-card">
                    <img src="https://images.unsplash.com/photo-1472851294608-062f824d29cc?q=80&w=500&auto=format&fit=crop" alt="E-Commerce Sederhana" class="project-img">
                    <div class="project-body">
                        <div class="project-title">E-Commerce Sederhana</div>
                        <div class="project-desc">Website toko online sederhana dengan fitur keranjang belanja.</div>
                        <div class="project-tags">
                            <span class="tag tag-orange">HTML</span>
                            <span class="tag tag-blue">CSS</span>
                            <span class="tag tag-yellow">JavaScript</span>
                            <span class="tag tag-purple">PHP</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- SERTIFIKAT, PENGALAMAN, PRESTASI -->
        <div class="grid-2-custom">
            <!-- SERTIFIKAT -->
            <section id="sertifikat" class="section-card">
                <div class="section-header">
                    <div class="icon-box"><i class="fas fa-certificate"></i></div>
                    <h2 class="section-title">Sertifikat</h2>
                </div>
               
                <ul class="cert-list">
                    <li>LDKS SMK Muthia Harapan Cicalengka</li>
                    <li>LDKS SMK Muthia Harapan Cicalengka</li>
                </ul>
                <a href="#" class="btn btn-outline" style="font-size: 0.82rem; padding: 8px 16px;">Lihat Semua Sertifikat</a>
            </section>

            <!-- PENGALAMAN & PRESTASI -->
            <div>
                <!-- PENGALAMAN -->
                <section id="pengalaman" class="section-card" style="margin-bottom: 20px;">
                    <div class="section-header">
                        <div class="icon-box"><i class="fas fa-briefcase"></i></div>
                        <h2 class="section-title">Pengalaman</h2>
                    </div>
                    <div class="timeline">
                        <div class="timeline-item">
                            <div class="timeline-dot"></div>
                            <div class="timeline-date">2018</div>
                            <div class="timeline-title">Camping</div>
                            <div class="timeline-subtitle">Di SDN BEOR 1</div>
                        </div>
                        <div class="timeline-item">
                            <div class="timeline-dot"></div>
                            <div class="timeline-date">2024</div>
                            <div class="timeline-title">LDKS</div>
                            <div class="timeline-subtitle">Di SMK Muthia Harapan Cicalengka</div>
                        </div>
                        <div class="timeline-item">
                            <div class="timeline-dot"></div>
                            <div class="timeline-date">2026 – Sekarang</div>
                            <div class="timeline-title">PKL (Praktik Kerja Lapangan)</div>
                            <div class="timeline-subtitle">Di SMK Muthia Harapan Cicalengka</div>
                        </div>
                    </div>
                </section>

                <!-- PRESTASI -->
                <section class="section-card">
                    <div class="section-header">
                        <div class="icon-box"><i class="fas fa-trophy"></i></div>
                        <h2 class="section-title">Prestasi</h2>
                    </div>
                    <ul class="prestasi-list">
                        <li class="prestasi-item"><i class="fas fa-star"></i>Juara 1 Lomba Adzan</li>
                        <li class="prestasi-item"><i class="fas fa-star"></i>Peringkat 1 Mts AL-Matsurat</li>
                    </ul>
                </section>
            </div>
        </div>

        <!-- KONTAK SAYA -->
        <section id="kontak" class="section-card">
            <div class="section-header">
                <div class="icon-box"><i class="fas fa-paper-plane"></i></div>
                <h2 class="section-title">Kontak Saya</h2>
            </div>
            <div class="contact-grid">
                <a href="mailto:dauffildaf@gmail.com" class="contact-card">
                    <div class="contact-icon"><i class="fas fa-envelope"></i></div>
                    <div class="contact-info">
                        <label>Email</label>
                        <span>dauffildaf@gmail.com</span>
                    </div>
                </a>
                <a href="https://wa.me/6288971323613" class="contact-card">
                    <div class="contact-icon"><i class="fas fa-phone"></i></div>
                    <div class="contact-info">
                        <label>No. HP</label>
                        <span>0889-7132-3613</span>
                    </div>
                </a>
                 <a href="https://wa.me/6289847535780" class="contact-card">
                    <div class="contact-icon"><i class="fas fa-phone"></i></div>
                    <div class="contact-info">
                        <label>No. HP</label>
                        <span>0898-4753-5780</span>
                    </div>
                </a>
                <div class="contact-card">
                    <div class="contact-icon"><i class="fas fa-map-marker-alt"></i></div>
                    <div class="contact-info">
                        <label>Alamat</label>
                        <span>Bandung, Jawa Barat</span>
                    </div>
                </div>
                <a href="https://instagram.com/fuadfadli7.dev" class="contact-card">
                    <div class="contact-icon"><i class="fab fa-instagram"></i></div>
                    <div class="contact-info">
                        <label>Instagram</label>
                        <span>@fuadfadli7</span>
                    </div>
                </a>
                 <a href="https://instagram.com/abdulmarix.dev" class="contact-card">
                    <div class="contact-icon"><i class="fab fa-instagram"></i></div>
                    <div class="contact-info">
                        <label>Instagram</label>
                        <span>@abdulmarix</span>
                    </div>
                </a>
                <a href="https://linkedin.com/in/fuad_maulana" class="contact-card">
                    <div class="contact-icon"><i class="fab fa-linkedin-in"></i></div>
                    <div class="contact-info">
                        <label>LinkedIn</label>
                        <span>linkedin.com/in/fuad_maulana</span>
                    </div>
                </a>
            </div>
        </section>

    </div>

    <!-- FOOTER -->
    <footer>
        <div class="container">
            <p>© 2026 Fuad Maulana All Rights Reserved.</p>
            <p>Dibuat dengan <i class="fas fa-heart"></i> menggunakan HTML & CSS</p>
        </div>
        <a href="#home" class="scroll-top"><i class="fas fa-chevron-up"></i></a>
    </footer>


        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }

        body {
            background-color: #f8f9fa;
            color: var(--text-main);
            line-height: 1.6;
            padding-bottom: 20px;
        }

        .container {
            max-width: 1140px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* HEADER / NAVBAR */
        header {
            background: #fff;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 15px rgba(0,0,0,0.04);
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 70px;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 12px;
            font-size: 1.25rem;
            font-weight: 700;
            color: #1e293b;
        }

        .logo-badge {
            background: var(--primary);
            color: white;
            padding: 6px 12px;
            border-radius: 8px;
            font-weight: 800;
            font-size: 1.1rem;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 25px;
        }

        .nav-links a {
            text-decoration: none;
            color: #475569;
            font-weight: 500;
            font-size: 0.95rem;
            transition: all 0.3s;
            position: relative;
            padding-bottom: 4px;
        }

        .nav-links a:hover, .nav-links a.active {
            color: var(--primary);
        }

        .nav-links a.active::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 3px;
            background: var(--primary);
            border-radius: 2px;
        }

        /* HERO SECTION */
        .hero {
            padding: 60px 0 40px;
            background: linear-gradient(135deg, #f8f9ff 0%, #f1f0fe 100%);
            border-radius: 0 0 30px 30px;
            margin-bottom: 40px;
            position: relative;
            overflow: hidden;
        }

        .hero-grid {
            display: grid;
            grid-template-columns: 400px 1fr;
            gap: 50px;
            align-items: center;
        }

        .hero-img-wrapper {
            position: relative;
            display: flex;
            justify-content: center;
        }

        .hero-img-bg {
            width: 320px;
            height: 320px;
            background: #dcd6ff;
            border-radius: 50%;
            position: absolute;
            bottom: 0;
            z-index: 1;
        }

        .hero-img {
            width: 330px;
            height: 380px;
            object-fit: cover;
            position: relative;
            z-index: 2;
            border-bottom-left-radius: 160px;
            border-bottom-right-radius: 160px;
        }

        .hero-content h3 {
            font-size: 1.25rem;
            color: #475569;
            font-weight: 500;
            margin-bottom: 5px;
        }

        .hero-content h1 {
            font-size: 2.8rem;
            font-weight: 800;
            color: #0f172a;
            line-height: 1.2;
            margin-bottom: 8px;
        }

        .hero-content h2 {
            font-size: 1.4rem;
            color: var(--primary);
            font-weight: 600;
            margin-bottom: 20px;
        }

        .hero-content p {
            color: #64748b;
            font-size: 0.98rem;
            max-width: 580px;
            margin-bottom: 30px;
            line-height: 1.7;
        }

        .hero-btns {
            display: flex;
            gap: 15px;
            margin-bottom: 30px;
        }

        .btn {
            padding: 12px 24px;
            border-radius: 8px;
            font-weight: 600;
            text-decoration: none;
            display: inline-flex;
            align-items: center;
            gap: 8px;
            font-size: 0.95rem;
            transition: all 0.3s;
            cursor: pointer;
        }

        .btn-primary {
            background: var(--primary);
            color: white;
            box-shadow: 0 4px 15px rgba(108, 92, 231, 0.3);
            border: none;
        }

        .btn-primary:hover {
            background: var(--primary-dark);
            transform: translateY(-2px);
        }

        .btn-outline {
            background: transparent;
            color: var(--primary);
            border: 2px solid var(--primary);
        }

        .btn-outline:hover {
            background: rgba(108, 92, 231, 0.05);
            transform: translateY(-2px);
        }

        .social-links {
            display: flex;
            gap: 15px;
        }

        .social-icon {
            width: 40px;
            height: 40px;
            border-radius: 8px;
            background: white;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #334155;
            text-decoration: none;
            box-shadow: 0 2px 8px rgba(0,0,0,0.06);
            transition: all 0.3s;
            font-size: 1.1rem;
        }

        .social-icon:hover {
            background: var(--primary);
            color: white;
            transform: translateY(-3px);
        }

        /* SECTION STYLES */
        .section-card {
            background: white;
            border-radius: var(--radius-lg);
            padding: 30px;
            margin-bottom: 30px;
            box-shadow: var(--shadow-sm);
            border: 1px solid #f1f5f9;
        }

        .section-header {
            display: flex;
            align-items: center;
            gap: 12px;
            margin-bottom: 25px;
        }

        .icon-box {
            width: 42px;
            height: 42px;
            background: var(--primary);
            color: white;
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.2rem;
        }

        .section-title {
            font-size: 1.35rem;
            font-weight: 700;
            color: #0f172a;
            letter-spacing: 0.5px;
            text-transform: uppercase;
        }

        /* TENTANG SAYA */
        .tentang-grid {
            display: grid;
            grid-template-columns: 1fr 1.2fr;
            gap: 40px;
        }

        .tentang-desc {
            color: #475569;
            font-size: 0.95rem;
            line-height: 1.8;
        }

        .info-table {
            width: 100%;
            border-collapse: collapse;
        }

        .info-table tr {
            border-bottom: 1px dashed #f1f5f9;
        }

        .info-table tr:last-child {
            border-bottom: none;
        }

        .info-table td {
            padding: 8px 0;
            font-size: 0.92rem;
        }

        .info-label {
            font-weight: 600;
            color: #334155;
            width: 160px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .info-label i {
            color: var(--primary);
            width: 16px;
        }

        .info-colon {
            width: 20px;
            color: #94a3b8;
        }

        .info-val {
            color: #475569;
            font-weight: 500;
        }

        /* GRID 2 COLUMNS FOR MID SECTIONS */
        .grid-2 {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
        }

        .grid-2-custom {
            display: grid;
            grid-template-columns: 1fr 1.2fr;
            gap: 30px;
        }

        /* PENDIDIKAN & PENGALAMAN TIMELINE */
        .timeline {
            position: relative;
            padding-left: 20px;
        }

        .timeline::before {
            content: '';
            position: absolute;
            left: 4px;
            top: 8px;
            bottom: 8px;
            width: 2px;
            background: #e2e8f0;
        }

        .timeline-item {
            position: relative;
            margin-bottom: 25px;
        }

        .timeline-item:last-child {
            margin-bottom: 0;
        }

        .timeline-dot {
            position: absolute;
            left: -20px;
            top: 6px;
            width: 10px;
            height: 10px;
            border-radius: 50%;
            background: var(--primary);
            border: 2px solid white;
            box-shadow: 0 0 0 2px var(--primary);
        }

        .timeline-date {
            font-size: 0.85rem;
            font-weight: 700;
            color: var(--primary);
            margin-bottom: 4px;
        }

        .timeline-title {
            font-size: 1rem;
            font-weight: 700;
            color: #1e293b;
        }

        .timeline-subtitle {
            font-size: 0.88rem;
            color: #64748b;
            margin-bottom: 4px;
        }

        /* KEAHLIAN / SKILLS */
        .skill-item {
            margin-bottom: 18px;
        }

        .skill-info {
            display: flex;
            justify-content: space-between;
            margin-bottom: 6px;
            font-size: 0.9rem;
            font-weight: 600;
            color: #334155;
        }

        .skill-bar-bg {
            height: 8px;
            background: #e2e8f0;
            border-radius: 10px;
            overflow: hidden;
        }

        .skill-bar-fill {
            height: 100%;
            background: var(--primary);
            border-radius: 10px;
        }

        /* TOOLS & TEKNOLOGI */
        .tools-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 15px;
        }

        .tool-card {
            background: #f8fafc;
            border: 1px solid #f1f5f9;
            border-radius: 12px;
            padding: 15px;
            text-align: center;
            transition: all 0.3s;
        }

        .tool-card:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 15px rgba(0,0,0,0.05);
            border-color: #cbd5e1;
        }

        .tool-icon {
            height: 40px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 8px;
            font-size: 2rem;
        }

        .tool-name {
            font-size: 0.8rem;
            font-weight: 600;
            color: #475569;
        }

        /* PORTOFOLIO / PROYEK */
        .portfolio-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
        }

        .project-card {
            border-radius: 12px;
            overflow: hidden;
            border: 1px solid #e2e8f0;
            background: #fff;
            transition: all 0.3s;
        }

        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 12px 25px rgba(0,0,0,0.08);
        }

        .project-img {
            width: 100%;
            height: 180px;
            object-fit: cover;
            background: #cbd5e1;
            border-bottom: 1px solid #e2e8f0;
        }

        .project-body {
            padding: 20px;
        }

        .project-title {
            font-size: 1.05rem;
            font-weight: 700;
            color: #0f172a;
            margin-bottom: 8px;
        }

        .project-desc {
            font-size: 0.85rem;
            color: #64748b;
            margin-bottom: 15px;
            line-height: 1.5;
            height: 55px;
        }

        .project-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 6px;
        }

        .tag {
            padding: 4px 10px;
            border-radius: 6px;
            font-size: 0.72rem;
            font-weight: 700;
            color: white;
        }

        .tag-orange { background: #ff7675; }
        .tag-blue { background: #74b9ff; }
        .tag-yellow { background: #fdcb6e; color: #2d3436; }
        .tag-purple { background: #a29bfe; }

        /* SERTIFIKAT */
        .cert-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 15px;
            margin-bottom: 15px;
        }

        .cert-img {
            width: 100%;
            height: 100px;
            object-fit: cover;
            border-radius: 8px;
            border: 1px solid #e2e8f0;
        }

        .cert-list {
            list-style: none;
            margin-bottom: 20px;
        }

        .cert-list li {
            font-size: 0.88rem;
            color: #475569;
            margin-bottom: 6px;
            position: relative;
            padding-left: 15px;
        }

        .cert-list li::before {
            content: '•';
            color: var(--primary);
            font-weight: bold;
            position: absolute;
            left: 0;
        }

        /* PRESTASI */
        .prestasi-list {
            list-style: none;
        }

        .prestasi-item {
            display: flex;
            align-items: center;
            gap: 10px;
            margin-bottom: 12px;
            font-size: 0.9rem;
            color: #334155;
            font-weight: 500;
        }

        .prestasi-item i {
            color: var(--primary);
        }

        /* KONTAK */
        .contact-grid {
            display: grid;
            grid-template-columns: repeat(5, 1fr);
            gap: 15px;
        }

        .contact-card {
            background: #f8fafc;
            border: 1px solid #f1f5f9;
            border-radius: 12px;
            padding: 15px;
            display: flex;
            align-items: center;
            gap: 12px;
            text-decoration: none;
            color: inherit;
            transition: all 0.3s;
        }

        .contact-card:hover {
            border-color: var(--primary);
            background: #fff;
            box-shadow: 0 4px 12px rgba(108, 92, 231, 0.1);
        }

        .contact-icon {
            width: 38px;
            height: 38px;
            border-radius: 8px;
            background: #f1f0fe;
            color: var(--primary);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.1rem;
            flex-shrink: 0;
        }

        .contact-info label {
            display: block;
            font-size: 0.75rem;
            color: #94a3b8;
            font-weight: 600;
        }

        .contact-info span {
            font-size: 0.82rem;
            font-weight: 600;
            color: #334155;
            word-break: break-all;
        }

        /* FOOTER */
        footer {
            background: #1e1b4b;
            color: white;
            text-align: center;
            padding: 25px 0;
            margin-top: 40px;
            font-size: 0.88rem;
            position: relative;
        }

        footer p {
            color: #cbd5e1;
            margin-bottom: 4px;
        }

        footer i.fa-heart {
            color: #ef4444;
        }

        .scroll-top {
            position: fixed;
            bottom: 30px;
            right: 30px;
            width: 45px;
            height: 45px;
            background: var(--primary);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            text-decoration: none;
            box-shadow: 0 4px 15px rgba(108, 92, 231, 0.4);
            transition: all 0.3s;
            z-index: 99;
        }

        .scroll-top:hover {
            transform: translateY(-3px);
            background: var(--primary-dark);
        }

        /* RESPONSIVE DESIGN */
        @media (max-width: 992px) {
            .hero-grid {
                grid-template-columns: 1fr;
                text-align: center;
            }
            .hero-content p {
                margin: 0 auto 30px;
            }
            .hero-btns, .social-links {
                justify-content: center;
            }
            .tentang-grid, .grid-2, .grid-2-custom {
                grid-template-columns: 1fr;
            }
            .portfolio-grid {
                grid-template-columns: 1fr 1fr;
            }
            .contact-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        @media (max-width: 600px) {
            .nav-links {
                display: none; /* Hide on mobile for simplicity */
            }
            .portfolio-grid {
                grid-template-columns: 1fr;
            }
            .tools-grid {
                grid-template-columns: repeat(2, 1fr);
            }
            .contact-grid {
                grid-template-columns: 1fr;
            }
        }
