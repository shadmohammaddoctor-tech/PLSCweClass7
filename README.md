<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <!-- মেটা ডেসক্রিপশন ও কিওয়ার্ডস -->
    <meta name="description" content="PLSCweClass7 - Police Line's School And College, Natore-এর সপ্তম শ্রেণীর শিক্ষার্থীদের জন্য একটি অনলাইন শিক্ষা ও ক্লাস নোট শেয়ারিং প্ল্যাটফর্ম।">
    <meta name="keywords" content="PLSC, Police Line's School And College Natore, PLSCweClass, Class 7, Class Notes, Routine">
    <meta name="author" content="MD.SHAHARIYAN SAFIN (19)">
    
    <title>PLSCweClass7 | হোমপেজ</title>

    <!-- ফন্ট অসাম আইকন লাইব্রেরি -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <!-- গুগল ফন্টস (বাংলা ফন্টের জন্য) -->
    <link href="https://fonts.googleapis.com/css2?family=Hind+Siliguri:wght@300;400;500;600;700&display=swap" rel="stylesheet">

    <style>
        /* =================== 
           গ্লোবাল বা মূল স্টাইল 
        ==================== */
        :root {
            --primary-bg: #0a192f;
            --secondary-bg: #020c1b;
            --accent-color: #00bcd4;
            --accent-hover: #0097a7;
            --text-color: #333;
            --text-light: #8892b0;
            --white: #ffffff;
            --card-bg: #ffffff;
            --section-gray: #f4f6f9;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Hind Siliguri', 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #f0f4f8;
            color: var(--text-color);
            line-height: 1.6;
            overflow-x: hidden;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        ul {
            list-style: none;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* =================== 
           হেডার ও নেভিগেশন 
        ==================== */
        header {
            background-color: var(--primary-bg);
            color: var(--white);
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 5%;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.3);
            transition: all 0.3s ease;
        }

        .logo-area {
            display: flex;
            align-items: center;
            gap: 12px;
            cursor: pointer;
        }

        .logo-icon {
            font-size: 2.5rem;
            color: var(--accent-color);
            transition: transform 0.3s ease;
        }

        .logo-area:hover .logo-icon {
            transform: rotate(15deg) scale(1.1);
        }

        .brand-name {
            font-size: 1.8rem;
            font-weight: 800;
            letter-spacing: 1px;
            color: var(--white);
        }

        .brand-name span {
            color: var(--accent-color);
        }

        .school-name {
            font-size: 0.8rem;
            color: var(--text-light);
            margin-top: 2px;
            font-weight: 500;
        }

        nav {
            display: flex;
            align-items: center;
        }

        .nav-links {
            display: flex;
            gap: 30px;
        }

        .nav-links li a {
            color: var(--white);
            font-weight: 500;
            font-size: 1rem;
            transition: color 0.3s ease;
            position: relative;
        }

        .nav-links li a:hover,
        .nav-links li a.active {
            color: var(--accent-color);
        }

        .nav-links li a::after {
            content: '';
            width: 0;
            height: 2px;
            background: var(--accent-color);
            display: block;
            transition: width 0.3s;
            margin-top: 4px;
        }

        .nav-links li a:hover::after {
            width: 100%;
        }

        .burger {
            display: none;
            cursor: pointer;
            flex-direction: column;
            gap: 5px;
            z-index: 1001;
        }

        .burger div {
            width: 25px;
            height: 3px;
            background-color: var(--white);
            transition: all 0.3s ease;
            border-radius: 2px;
        }

        /* Burger Menu Animation */
        .burger.toggle .line1 { transform: rotate(-45deg) translate(-5px, 6px); }
        .burger.toggle .line2 { opacity: 0; }
        .burger.toggle .line3 { transform: rotate(45deg) translate(-5px, -6px); }

        /* =================== 
           হিরো বা ব্যানার সেকশন 
        ==================== */
        .hero {
            background: linear-gradient(rgba(10, 25, 47, 0.85), rgba(10, 25, 47, 0.85)), url('https://z-cdn-media.chatglm.cn/files/c9118450-ae92-48da-815d-ec11c62972b1.png?auth_key=1881614616-bbc3f2d705b74581bbe46bb7d34f8c0f-0-7bb4e6b4fc5ce590091861653eb1121e') center/cover no-repeat;
            min-height: 80vh;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: var(--white);
            padding: 0 20px;
            position: relative;
        }

        .hero-content {
            animation: fadeIn 1.2s ease-in-out;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .hero-content h2 {
            font-size: 2.8rem;
            margin-bottom: 15px;
            color: var(--accent-color);
            text-shadow: 0 2px 4px rgba(0,0,0,0.5);
        }

        .hero-content p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 30px auto;
            opacity: 0.9;
        }

        .btn-primary {
            background-color: var(--accent-color);
            color: var(--primary-bg);
            padding: 12px 35px;
            border-radius: 50px;
            font-weight: 700;
            font-size: 1.1rem;
            display: inline-block;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
            box-shadow: 0 4px 15px rgba(0, 188, 212, 0.4);
        }

        .btn-primary:hover {
            background-color: var(--accent-hover);
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(0, 188, 212, 0.6);
        }

        /* =================== 
           মূল কনটেন্ট (নোটিশ ও বাণী) 
        ==================== */
        .main-content {
            padding: 80px 0;
            margin-top: -50px;
            position: relative;
            z-index: 10;
        }

        .main-content .container {
            display: flex;
            gap: 30px;
            flex-wrap: wrap;
        }

        .speech-card, .notice-board {
            background: var(--card-bg);
            border-radius: 15px;
            padding: 30px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            flex: 1;
            min-width: 300px;
            transition: all 0.3s ease;
            border-top: 5px solid var(--accent-color);
        }

        .speech-card:hover, .notice-board:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 35px rgba(0,0,0,0.15);
        }

        .speech-card h3, .notice-board h3 {
            color: var(--primary-bg);
            font-size: 1.5rem;
            margin-bottom: 10px;
            display: flex;
            align-items: center;
        }

        .speech-card h3 i, .notice-board h3 i {
            color: var(--accent-color);
            margin-right: 10px;
            background: rgba(0, 188, 212, 0.1);
            padding: 10px;
            border-radius: 50%;
            font-size: 1.2rem;
        }

        .speech-card hr, .notice-board hr {
            border: 0;
            height: 1px;
            background: #eee;
            margin: 20px 0;
        }

        .speech-card p {
            font-style: italic;
            color: #555;
            line-height: 1.8;
            margin-bottom: 20px;
            font-size: 1.05rem;
        }

        .speech-card h4 {
            color: var(--primary-bg);
            text-align: right;
            margin-bottom: 5px;
            font-weight: 700;
        }

        .speech-card span {
            display: block;
            text-align: right;
            color: var(--accent-color);
            font-size: 0.9rem;
            font-weight: 600;
        }

        .notice-item {
            margin-bottom: 15px;
            border-left: 4px solid var(--accent-color);
            padding: 12px 15px;
            background: #f9fbfd;
            border-radius: 0 8px 8px 0;
            transition: background 0.3s;
        }

        .notice-item:hover {
            background: #eef6f9;
            border-left-width: 6px;
        }

        .date {
            font-size: 0.8rem;
            color: var(--accent-color);
            font-weight: 600;
            display: block;
            margin-bottom: 4px;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        .notice-item a {
            color: var(--primary-bg);
            font-weight: 500;
            display: block;
        }

        .notice-item a:hover {
            color: var(--accent-color);
        }

        .btn-secondary {
            display: inline-block;
            margin-top: 10px;
            color: var(--accent-color);
            border: 2px solid var(--accent-color);
            padding: 8px 25px;
            border-radius: 50px;
            font-weight: 600;
            transition: all 0.3s;
        }

        .btn-secondary:hover {
            background-color: var(--accent-color);
            color: white;
        }

        /* =================== 
           অ্যাকাডেমিক সেকশন (নতুন যুক্ত করা হয়েছে) 
        ==================== */
        .academic-section {
            padding: 60px 5%;
            background-color: var(--section-gray);
        }

        .academic-container {
            display: flex;
            gap: 30px;
            flex-wrap: wrap;
            max-width: 1200px;
            margin: 0 auto;
        }

        .routine-box, .download-box {
            flex: 1;
            min-width: 320px;
            background: white;
            padding: 25px;
            border-radius: 12px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s;
        }
        
        .routine-box:hover, .download-box:hover {
            transform: translateY(-5px);
        }

        .routine-box h3, .download-box h3 {
            color: var(--primary-bg);
            margin-bottom: 10px;
            font-size: 1.4rem;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .routine-box h3 i, .download-box h3 i {
            color: var(--accent-color);
        }

        /* টেবিল স্টাইল */
        .table-responsive {
            overflow-x: auto;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 15px;
            text-align: left;
        }

        table th, table td {
            padding: 12px;
            border-bottom: 1px solid #eee;
        }

        table th {
            background-color: var(--primary-bg);
            color: white;
            font-weight: 600;
        }

        table tr:hover {
            background-color: #f9f9f9;
        }

        /* ডাউনলোড লিস্ট স্টাইল */
        .download-list {
            margin-top: 15px;
        }

        .download-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px;
            background: #f8fafc;
            border-radius: 8px;
            margin-bottom: 12px;
            border-left: 4px solid var(--accent-color);
            transition: 0.3s;
        }

        .download-item:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 10px rgba(0,0,0,0.08);
            background: #fff;
        }

        .file-info {
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .pdf-icon {
            font-size: 2rem;
            color: #ff5722;
        }

        .doc-icon {
            font-size: 2rem;
            color: #2196f3;
        }

        .file-info h4 {
            font-size: 1rem;
            color: #333;
            margin-bottom: 2px;
        }

        .file-info p {
            font-size: 0.8rem;
            color: #777;
            margin: 0;
        }

        .btn-download {
            background-color: var(--primary-bg);
            color: white;
            width: 40px;
            height: 40px;
            display: flex;
            justify-content: center;
            align-items: center;
            border-radius: 50%;
            text-decoration: none;
            transition: 0.3s;
        }

        .btn-download:hover {
            background-color: var(--accent-color);
            color: var(--primary-bg);
            transform: rotate(10deg);
        }

        /* =================== 
           যোগাযোগ সেকশন 
        ==================== */
        .contact-section {
            background-color: var(--primary-bg);
            color: var(--white);
            padding: 80px 5%;
        }

        .contact-section h3 {
            text-align: center;
            font-size: 2rem;
            margin-bottom: 50px;
            color: var(--accent-color);
            position: relative;
        }

        .contact-section h3::after {
            content: '';
            display: block;
            width: 60px;
            height: 3px;
            background: var(--accent-color);
            margin: 10px auto 0;
            border-radius: 2px;
        }

        .contact-container {
            display: flex;
            gap: 50px;
            flex-wrap: wrap;
            max-width: 1200px;
            margin: 0 auto;
        }

        .contact-info, .contact-form {
            flex: 1;
            min-width: 300px;
        }

        .contact-info p {
            margin-bottom: 25px;
            font-size: 1.1rem;
            display: flex;
            align-items: center;
        }

        .contact-info i {
            color: var(--accent-color);
            margin-right: 15px;
            width: 25px;
            text-align: center;
            font-size: 1.2rem;
        }

        .contact-form input, .contact-form textarea {
            width: 100%;
            padding: 15px;
            margin-bottom: 20px;
            border: 1px solid #233554;
            border-radius: 8px;
            background: #172a45;
            color: var(--white);
            font-size: 1rem;
            font-family: inherit;
            transition: all 0.3s;
        }

        .contact-form input:focus, .contact-form textarea:focus {
            outline: none;
            border-color: var(--accent-color);
            background: #1e3552;
            box-shadow: 0 0 10px rgba(0, 188, 212, 0.1);
        }

        .contact-form input::placeholder, .contact-form textarea::placeholder {
            color: var(--text-light);
        }

        /* =================== 
           ফুটার 
        ==================== */
        footer {
            background-color: var(--secondary-bg);
            color: var(--text-light);
            text-align: center;
            padding: 30px 5%;
            font-size: 0.95rem;
            border-top: 1px solid #112240;
        }

        footer p {
            margin-bottom: 8px;
        }

        footer p i {
            animation: pulse 1.5s infinite;
        }

        /* Domain Link Style */
        .footer-domain {
            display: inline-block;
            margin-top: 10px;
            color: var(--accent-color);
            font-weight: 600;
            text-decoration: none;
            transition: color 0.3s;
        }

        .footer-domain:hover {
            color: var(--white);
            text-decoration: underline;
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.3); }
            100% { transform: scale(1); }
        }

        /* =================== 
           রেসপন্সিভ ডিজাইন (মোবাইল) 
        ==================== */
        @media screen and (max-width: 768px) {
            .nav-links {
                position: fixed;
                right: 0;
                top: 0;
                height: 100vh;
                background-color: #112240;
                display: flex;
                flex-direction: column;
                align-items: center;
                width: 70%;
                transform: translateX(100%);
                transition: transform 0.4s ease-in-out;
                justify-content: center;
                box-shadow: -5px 0 15px rgba(0,0,0,0.5);
                z-index: 999;
            }

            .nav-active {
                transform: translateX(0%);
            }

            .burger {
                display: flex;
            }

            .hero-content h2 {
                font-size: 2rem;
            }

            .hero-content p {
                font-size: 1rem;
            }

            .main-content {
                margin-top: 0;
                padding-top: 40px;
            }
            
            .contact-container {
                flex-direction: column;
            }
            
            .academic-container {
                flex-direction: column;
            }
        }
        
        /* টোস্ট নোটিফিকেশন স্টাইল */
        .toast {
            position: fixed;
            bottom: 30px;
            left: 50%;
            transform: translateX(-50%);
            background-color: var(--accent-color);
            color: var(--primary-bg);
            padding: 15px 30px;
            border-radius: 50px;
            font-weight: 600;
            box-shadow: 0 5px 15px rgba(0,0,0,0.3);
            opacity: 0;
            visibility: hidden;
            transition: all 0.3s;
            z-index: 2000;
        }
        
        .toast.show {
            opacity: 1;
            visibility: visible;
            bottom: 50px;
        }
    </style>
</head>
<body>

    <!-- হেডার ও নেভিগেশন বার -->
    <header>
        <div class="logo-area" onclick="window.location.reload()">
            <i class="fas fa-graduation-cap logo-icon"></i>
            <div>
                <h1 class="brand-name">PLSC<span>weClass7</span></h1>
                <p class="school-name">Police Line's School And College, Natore</p>
            </div>
        </div>
        <nav>
            <ul class="nav-links" id="navLinks">
                <li><a href="#" class="active" onclick="closeMenu()">হোম</a></li>
                <li><a href="#about" onclick="closeMenu()">আমাদের সম্পর্কে</a></li>
                <li><a href="#routine" onclick="closeMenu()">ক্লাস রুটিন</a></li>
                <li><a href="#notes" onclick="closeMenu()">নোটস ও সাজেশন</a></li>
                <li><a href="#gallery" onclick="closeMenu()">গ্যালারি</a></li>
                <li><a href="#contact" onclick="closeMenu()">যোগাযোগ</a></li>
            </ul>
            <div class="burger" onclick="toggleMenu()">
                <div class="line1"></div>
                <div class="line2"></div>
                <div class="line3"></div>
            </div>
        </nav>
    </header>

    <!-- হিরো বা ব্যানার সেকশন -->
    <section class="hero">
        <div class="hero-content">
            <h2>PLSCweClass7 এ আপনাকে স্বাগতম</h2>
            <p>Police Line's School And College, Natore-এর সপ্তম শ্রেণীর শিক্ষার্থীদের পড়াশোনাকে আরও সহজ, আকর্ষণীয় এবং ডিজিটালাইজড করার একটি যৌথ প্রয়াস। আমাদের সাথেই থাকুন উজ্জ্বল ভবিষ্যতের পথে।</p>
            <button class="btn-primary" onclick="scrollToSection('routine')">আজকের ক্লাস দেখুন</button>
        </div>
    </section>

    <!-- মূল কনটেন্ট (নোটিশ ও প্রধান বাণী) -->
    <section class="main-content" id="about">
        <div class="container">
            
            <!-- ক্লাসের বার্তা -->
            <div class="speech-card">
                <h3><i class="fas fa-bullhorn"></i> আমাদের লক্ষ্য</h3>
                <hr>
                <p>"PLSCweClass7 এর মূল উদ্দেশ্য হলো আমাদের ক্লাসের সকল সহপাঠীদের মধ্যে পড়াশোনার রিসোর্স সহজে শেয়ার করা। এখানে আমরা গুরুত্বপূর্ণ নোট, অ্যাসাইনমেন্টের আপডেট এবং পরীক্ষার সাজেশন নিয়মিত শেয়ার করবো যেন আমরা সবাই একসাথে ভালো ফলাফল করতে পারি।"</p>
                <h4>- ক্লাস মনিটর ও এডমিন প্যানেল</h4>
                <span>PLSCweClass7 টিম</span>
            </div>

            <!-- নোটিশ বোর্ড -->
            <div class="notice-board">
                <h3><i class="fas fa-bell"></i> ক্লাস নোটিশ</h3>
                <hr>
                <div class="notice-list">
                    <div class="notice-item">
                        <span class="date">১৬ জুন, ২০২৬</span>
                        <a href="#">আগামীকালের বিজ্ঞান ক্লাসের অ্যাসাইনমেন্ট জমা দেওয়ার শেষ সময়।</a>
                    </div>
                    <div class="notice-item">
                        <span class="date">১৪ জুন, ২০২৬</span>
                        <a href="#">গণিত বিষয়ের অধ্যায় ৫ এর বিশেষ নোট আপলোড করা হয়েছে।</a>
                    </div>
                    <div class="notice-item">
                        <span class="date">১২ জুন, ২০২৬</span>
                        <a href="#">সাপ্তাহিক ক্লাস টেস্টের সময়সূচী ও সিলেবাস।</a>
                    </div>
                </div>
                <a href="#" class="btn-secondary" onclick="showToast('সকল নোটিশ লোড হচ্ছে...')">সকল নোটিশ দেখুন</a>
            </div>

        </div>
    </section>

    <!-- অ্যাকাডেমিক সেকশন (রুটিন ও ডাউনলোড) -->
    <section class="academic-section" id="routine">
        <div class="academic-container">
            
            <div class="routine-box">
                <h3><i class="fas fa-calendar-alt"></i> আজকের ক্লাস রুটিন</h3>
                <hr>
                <div class="table-responsive">
                    <table>
                        <thead>
                            <tr>
                                <th>সময়</th>
                                <th>বিষয়</th>
                                <th>শিক্ষক</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td>০৯:০০ AM</td>
                                <td>বাংলা</td>
                                <td>এ. রহমান</td>
                            </tr>
                            <tr>
                                <td>১০:০০ AM</td>
                                <td>ইংরেজি</td>
                                <td>এস. ইসলাম</td>
                            </tr>
                            <tr>
                                <td>১১:০০ AM</td>
                                <td>গণিত</td>
                                <td>এম. হাসান</td>
                            </tr>
                            <tr>
                                <td>১২:০০ PM</td>
                                <td>বিজ্ঞান</td>
                                <td>কে. আহমেদ</td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>

            <div class="download-box" id="notes">
                <h3><i class="fas fa-cloud-download-alt"></i> ক্লাস নোটস ও ফাইল</h3>
                <hr>
                <div class="download-list">
                    <div class="download-item">
                        <div class="file-info">
                            <i class="far fa-file-pdf pdf-icon"></i>
                            <div>
                                <h4>গণিত - অধ্যায় ৫ (বীজগণিত)</h4>
                                <p>সাইজ: ৪.৫ MB | আপলোড: ১৫ জুন</p>
                            </div>
                        </div>
                        <a href="#" class="btn-download" onclick="handleDownload(event, 'গণিত - অধ্যায় ৫')"><i class="fas fa-download"></i></a>
                    </div>

                    <div class="download-item">
                        <div class="file-info">
                            <i class="far fa-file-pdf pdf-icon"></i>
                            <div>
                                <h4>বিজ্ঞান - অধ্যায় ২ (কোষ গঠন)</h4>
                                <p>সাইজ: ৩.২ MB | আপলোড: ১২ জুন</p>
                            </div>
                        </div>
                        <a href="#" class="btn-download" onclick="handleDownload(event, 'বিজ্ঞান - অধ্যায় ২')"><i class="fas fa-download"></i></a>
                    </div>
                    
                    <div class="download-item">
                        <div class="file-info">
                            <i class="far fa-file-word doc-icon"></i>
                            <div>
                                <h4>ইংরেজি - প্যারাগ্রাফ সাজেশন</h4>
                                <p>সাইজ: ১.৮ MB | আপলোড: ১০ জুন</p>
                            </div>
                        </div>
                        <a href="#" class="btn-download" onclick="handleDownload(event, 'ইংরেজি সাজেশন')"><i class="fas fa-download"></i></a>
                    </div>
                </div>
            </div>

        </div>
    </section>

    <!-- যোগাযোগ সেকশন -->
    <section class="contact-section" id="contact">
        <h3>যোগাযোগ ও মতামত</h3>
        <div class="contact-container">
            <div class="contact-info">
                <p><i class="fas fa-school"></i> Police Line's School And College, Natore</p>
                <p><i class="fas fa-envelope"></i> admin@plscweclass7.com</p>
                <p><i class="fas fa-users"></i> আমাদের সাথে যুক্ত থাকুন এবং আপনার গ্রুপ স্টাডিকে করুন আরও সহজ।</p>
                <p><i class="fas fa-map-marker-alt"></i> পুলিশ লাইন, নাটোর, বাংলাদেশ</p>
            </div>
            
            <form class="contact-form" id="contactForm" onsubmit="handleFormSubmit(event)">
                <input type="text" placeholder="আপনার নাম" required>
                <input type="email" placeholder="আপনার ইমেইল" required>
                <textarea placeholder="আপনার প্রশ্ন বা মতামত এখানে লিখুন..." rows="4" required></textarea>
                <button type="submit" class="btn-primary">বার্তা পাঠান</button>
            </form>
        </div>
    </section>

    <!-- ফুটার -->
    <footer>
        <p>&copy; ২০২৬ PLSCweClass7 | Police Line's School And College, Natore। সর্বস্বত্ব সংরক্ষিত।</p>
        <p>Developed with <i class="fas fa-heart" style="color: var(--accent-color);"></i> by MD.SHAHARIYAN SAFIN (19)</p>
        <!-- ডোমেইন যুক্ত করা হয়েছে -->
        <p>Visit our official website: <br>
            <a href="http://www.plscweclass7.com" target="_blank" class="footer-domain">
                <i class="fas fa-globe"></i> www.plscweclass7.com
            </a>
        </p>
    </footer>

    <!-- টোস্ট নোটিফিকেশন এলিমেন্ট -->
    <div id="toast" class="toast">বার্তা সফলভাবে পাঠানো হয়েছে!</div>

    <!-- জাভাস্ক্রিপ্ট -->
    <script>
        const navLinks = document.getElementById('navLinks');
        const burger = document.querySelector('.burger');

        // মেনু টগল ফাংশন
        function toggleMenu() {
            navLinks.classList.toggle('nav-active');
            burger.classList.toggle('toggle');
        }

        // মেনু বন্ধ করার ফাংশন (লিংকে ক্লিক করলে)
        function closeMenu() {
            navLinks.classList.remove('nav-active');
            burger.classList.remove('toggle');
        }

        // স্পেসিফিক সেকশনে স্ক্রল করা
        function scrollToSection(id) {
            const section = document.getElementById(id);
            if (section) {
                section.scrollIntoView({ behavior: 'smooth' });
            } else {
                showToast("সেকশনটি শীঘ্রই আসছে!");
            }
        }

        // ডাউনলোড হ্যান্ডলিং
        function handleDownload(event, fileName) {
            event.preventDefault();
            showToast(fileName + " ডাউনলোড শুরু হচ্ছে...");
        }

        // ফর্ম সাবমিট হ্যান্ডলিং
        function handleFormSubmit(event) {
            event.preventDefault();
            
            const btn = event.target.querySelector('button');
            const originalText = btn.innerText;
            btn.innerText = "পাঠানো হচ্ছে...";
            btn.style.opacity = "0.7";
            
            setTimeout(() => {
                showToast("ধন্যবাদ! আপনার বার্তা সফলভাবে পাঠানো হয়েছে।");
                event.target.reset();
                btn.innerText = originalText;
                btn.style.opacity = "1";
            }, 1500);
        }

        // টোস্ট মেসেজ দেখানোর ফাংশন
        function showToast(message) {
            const toast = document.getElementById('toast');
            toast.innerText = message;
            toast.classList.add('show');
            
            setTimeout(() => {
                toast.classList.remove('show');
            }, 3000);
        }
    </script>
</body>
</html>
