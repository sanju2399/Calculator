<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Free online calculators for finance, math, health, and more. Calculate mortgages, loans, BMI, taxes, and much more.">
    <meta name="keywords" content="calculator, financial calculator, mortgage calculator, loan calculator, BMI calculator, math calculator">
    <title>Free Online Calculators - Financial, Math, Health & More</title>
    <style>
        :root {
            --primary-color: #3498db;
            --secondary-color: #2c3e50;
            --accent-color: #e74c3c;
            --light-color: #ecf0f1;
            --dark-color: #2c3e50;
            --shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            --border-radius: 8px;
        }
        
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
        }
        
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }
        
        header {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
            padding: 1rem 0;
            box-shadow: var(--shadow);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: 700;
        }
        
        .logo span {
            color: var(--accent-color);
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 1.5rem;
        }
        
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }
        
        nav ul li a:hover {
            color: var(--accent-color);
        }
        
        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            color: white;
            font-size: 1.5rem;
            cursor: pointer;
        }
        
        .hero {
            background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), url('https://images.unsplash.com/photo-1551288049-bebda4e38f71?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 4rem 1rem;
            margin-bottom: 2rem;
        }
        
        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 1.5rem;
        }
        
        .search-bar {
            max-width: 600px;
            margin: 0 auto;
            position: relative;
        }
        
        .search-bar input {
            width: 100%;
            padding: 12px 20px;
            border: none;
            border-radius: 50px;
            font-size: 1rem;
            box-shadow: var(--shadow);
        }
        
        .search-bar button {
            position: absolute;
            right: 5px;
            top: 5px;
            background: var(--primary-color);
            color: white;
            border: none;
            border-radius: 50px;
            padding: 7px 15px;
            cursor: pointer;
        }
        
        .categories {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 1.5rem;
            margin: 2rem 0;
        }
        
        .category-card {
            background: white;
            border-radius: var(--border-radius);
            padding: 1.5rem;
            box-shadow: var(--shadow);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .category-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
        }
        
        .category-card h3 {
            color: var(--secondary-color);
            margin-bottom: 1rem;
            padding-bottom: 0.5rem;
            border-bottom: 2px solid var(--primary-color);
        }
        
        .calculator-list {
            list-style: none;
        }
        
        .calculator-list li {
            margin-bottom: 0.5rem;
        }
        
        .calculator-list a {
            color: #555;
            text-decoration: none;
            transition: color 0.3s;
            display: flex;
            align-items: center;
        }
        
        .calculator-list a:hover {
            color: var(--primary-color);
        }
        
        .calculator-list a::before {
            content: "➜";
            margin-right: 8px;
            color: var(--primary-color);
            font-size: 0.8rem;
        }
        
        .calculator-container {
            display: none;
            background: white;
            border-radius: var(--border-radius);
            padding: 2rem;
            box-shadow: var(--shadow);
            margin: 2rem 0;
        }
        
        .calculator-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 1.5rem;
            padding-bottom: 1rem;
            border-bottom: 1px solid #eee;
        }
        
        .calculator-header h2 {
            color: var(--secondary-color);
        }
        
        .back-btn {
            background: var(--light-color);
            color: var(--dark-color);
            border: none;
            padding: 8px 15px;
            border-radius: var(--border-radius);
            cursor: pointer;
            display: flex;
            align-items: center;
            transition: background 0.3s;
        }
        
        .back-btn:hover {
            background: #ddd;
        }
        
        .calculator-form {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 1.5rem;
        }
        
        .form-group {
            margin-bottom: 1rem;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 500;
            color: var(--secondary-color);
        }
        
        .form-group input, .form-group select {
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: var(--border-radius);
            font-size: 1rem;
        }
        
        .calculate-btn {
            grid-column: span 2;
            background: var(--primary-color);
            color: white;
            border: none;
            padding: 12px;
            border-radius: var(--border-radius);
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            transition: background 0.3s;
        }
        
        .calculate-btn:hover {
            background: #2980b9;
        }
        
        .result {
            grid-column: span 2;
            background: var(--light-color);
            padding: 1.5rem;
            border-radius: var(--border-radius);
            margin-top: 1rem;
            display: none;
        }
        
        .result h3 {
            color: var(--secondary-color);
            margin-bottom: 1rem;
        }
        
        .result-item {
            display: flex;
            justify-content: space-between;
            margin-bottom: 0.5rem;
            padding-bottom: 0.5rem;
            border-bottom: 1px solid #ddd;
        }
        
        .ads {
            margin: 2rem 0;
            text-align: center;
        }
        
        .ad-unit {
            background: #f8f9fa;
            border: 1px dashed #ccc;
            padding: 20px;
            margin: 1rem 0;
            border-radius: var(--border-radius);
            min-height: 90px;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        footer {
            background: var(--secondary-color);
            color: white;
            padding: 2rem 0;
            margin-top: 3rem;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }
        
        .footer-section h3 {
            margin-bottom: 1rem;
            color: var(--primary-color);
        }
        
        .footer-section ul {
            list-style: none;
        }
        
        .footer-section ul li {
            margin-bottom: 0.5rem;
        }
        
        .footer-section a {
            color: #ddd;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-section a:hover {
            color: var(--primary-color);
        }
        
        .copyright {
            text-align: center;
            margin-top: 2rem;
            padding-top: 1rem;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }
            
            nav ul {
                margin-top: 1rem;
                flex-wrap: wrap;
                justify-content: center;
            }
            
            nav ul li {
                margin: 0.5rem;
            }
            
            .calculator-form {
                grid-template-columns: 1fr;
            }
            
            .calculate-btn, .result {
                grid-column: 1;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
        }
        
        @media (max-width: 576px) {
            .mobile-menu-btn {
                display: block;
                position: absolute;
                top: 1rem;
                right: 1rem;
            }
            
            nav {
                display: none;
                width: 100%;
                margin-top: 1rem;
            }
            
            nav.active {
                display: block;
            }
            
            nav ul {
                flex-direction: column;
            }
            
            nav ul li {
                margin: 0.5rem 0;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">Calc<span>Hub</span></div>
                <button class="mobile-menu-btn">☰</button>
                <nav>
                    <ul>
                        <li><a href="#financial">Financial</a></li>
                        <li><a href="#math">Math</a></li>
                        <li><a href="#health">Health</a></li>
                        <li><a href="#other">Other</a></li>
                        <li><a href="#conversion">Conversion</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

    <section class="hero">
        <div class="container">
            <h1>Free Online Calculators</h1>
            <p>Calculate anything from mortgages and loans to BMI and taxes with our easy-to-use calculators</p>
            <div class="search-bar">
                <input type="text" placeholder="Search for a calculator...">
                <button>Search</button>
            </div>
        </div>
    </section>

    <div class="container">
        <div class="ads">
            <div class="ad-unit">
                <!-- Google AdSense Ad Unit -->
                <!-- Replace with your AdSense code -->
                <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-XXXXXXXXXXXXXXXX"
                     crossorigin="anonymous"></script>
                <ins class="adsbygoogle"
                     style="display:block"
                     data-ad-client="ca-pub-XXXXXXXXXXXXXXXX"
                     data-ad-slot="XXXXXXXXXX"
                     data-ad-format="auto"
                     data-full-width-responsive="true"></ins>
                <script>
                     (adsbygoogle = window.adsbygoogle || []).push({});
                </script>
            </div>
        </div>

        <div class="categories">
            <div class="category-card" id="financial">
                <h3>Financial Calculators</h3>
                <ul class="calculator-list">
                    <li><a href="#" data-calc="mortgage">Mortgage Calculator</a></li>
                    <li><a href="#" data-calc="loan">Loan Calculator</a></li>
                    <li><a href="#" data-calc="auto-loan">Auto Loan Calculator</a></li>
                    <li><a href="#" data-calc="interest">Interest Calculator</a></li>
                    <li><a href="#" data-calc="payment">Payment Calculator</a></li>
                    <li><a href="#" data-calc="retirement">Retirement Calculator</a></li>
                    <li><a href="#" data-calc="amortization">Amortization Calculator</a></li>
                    <li><a href="#" data-calc="investment">Investment Calculator</a></li>
                    <li><a href="#" data-calc="inflation">Inflation Calculator</a></li>
                    <li><a href="#" data-calc="finance">Finance Calculator</a></li>
                    <li><a href="#" data-calc="income-tax">Income Tax Calculator</a></li>
                    <li><a href="#" data-calc="compound-interest">Compound Interest Calculator</a></li>
                    <li><a href="#" data-calc="salary">Salary Calculator</a></li>
                    <li><a href="#" data-calc="interest-rate">Interest Rate Calculator</a></li>
                    <li><a href="#" data-calc="sales-tax">Sales Tax Calculator</a></li>
                </ul>
            </div>

            <div class="category-card" id="math">
                <h3>Math Calculators</h3>
                <ul class="calculator-list">
                    <li><a href="#" data-calc="scientific">Scientific Calculator</a></li>
                    <li><a href="#" data-calc="fraction">Fraction Calculator</a></li>
                    <li><a href="#" data-calc="percentage">Percentage Calculator</a></li>
                    <li><a href="#" data-calc="random">Random Number Generator</a></li>
                    <li><a href="#" data-calc="triangle">Triangle Calculator</a></li>
                    <li><a href="#" data-calc="standard-deviation">Standard Deviation Calculator</a></li>
                </ul>
            </div>

            <div class="category-card" id="health">
                <h3>Fitness & Health Calculators</h3>
                <ul class="calculator-list">
                    <li><a href="#" data-calc="bmi">BMI Calculator</a></li>
                    <li><a href="#" data-calc="calorie">Calorie Calculator</a></li>
                    <li><a href="#" data-calc="body-fat">Body Fat Calculator</a></li>
                    <li><a href="#" data-calc="bmr">BMR Calculator</a></li>
                    <li><a href="#" data-calc="ideal-weight">Ideal Weight Calculator</a></li>
                    <li><a href="#" data-calc="pace">Pace Calculator</a></li>
                    <li><a href="#" data-calc="pregnancy">Pregnancy Calculator</a></li>
                    <li><a href="#" data-calc="conception">Pregnancy Conception Calculator</a></li>
                    <li><a href="#" data-calc="due-date">Due Date Calculator</a></li>
                </ul>
            </div>

            <div class="category-card" id="other">
                <h3>Other Calculators</h3>
                <ul class="calculator-list">
                    <li><a href="#" data-calc="age">Age Calculator</a></li>
                    <li><a href="#" data-calc="date">Date Calculator</a></li>
                    <li><a href="#" data-calc="time">Time Calculator</a></li>
                    <li><a href="#" data-calc="hours">Hours Calculator</a></li>
                    <li><a href="#" data-calc="gpa">GPA Calculator</a></li>
                    <li><a href="#" data-calc="grade">Grade Calculator</a></li>
                    <li><a href="#" data-calc="concrete">Concrete Calculator</a></li>
                    <li><a href="#" data-calc="subnet">Subnet Calculator</a></li>
                </ul>
            </div>

            <div class="category-card" id="conversion">
                <h3>Conversion Calculators</h3>
                <ul class="calculator-list">
                    <li><a href="#" data-calc="length">Length Converter</a></li>
                    <li><a href="#" data-calc="weight">Weight Converter</a></li>
                    <li><a href="#" data-calc="temperature">Temperature Converter</a></li>
                    <li><a href="#" data-calc="currency">Currency Converter</a></li>
                    <li><a href="#" data-calc="area">Area Converter</a></li>
                    <li><a href="#" data-calc="volume">Volume Converter</a></li>
                </ul>
            </div>
        </div>

        <div class="calculator-container" id="calculator-display">
            <div class="calculator-header">
                <h2 id="calculator-title">Calculator</h2>
                <button class="back-btn" id="back-to-categories">← Back to Categories</button>
            </div>
            <div id="calculator-content">
                <!-- Calculator forms will be dynamically inserted here -->
            </div>
        </div>

        <div class="ads">
            <div class="ad-unit">
                <!-- Google AdSense Ad Unit -->
                <!-- Replace with your AdSense code -->
                <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-XXXXXXXXXXXXXXXX"
                     crossorigin="anonymous"></script>
                <ins class="adsbygoogle"
                     style="display:block"
                     data-ad-client="ca-pub-XXXXXXXXXXXXXXXX"
                     data-ad-slot="XXXXXXXXXX"
                     data-ad-format="auto"
                     data-full-width-responsive="true"></ins>
                <script>
                     (adsbygoogle = window.adsbygoogle || []).push({});
                </script>
            </div>
        </div>
    </div>

    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h3>About CalcHub</h3>
                    <p>CalcHub provides free online calculators for various purposes including finance, math, health, and more. Our tools are designed to be user-friendly and accurate.</p>
                </div>
                <div class="footer-section">
                    <h3>Quick Links</h3>
                    <ul>
                        <li><a href="#financial">Financial Calculators</a></li>
                        <li><a href="#math">Math Calculators</a></li>
                        <li><a href="#health">Health Calculators</a></li>
                        <li><a href="#other">Other Calculators</a></li>
                    </ul>
                </div>
                <div class="footer-section">
                    <h3>Legal</h3>
                    <ul>
                        <li><a href="#">Privacy Policy</a></li>
                        <li><a href="#">Terms of Service</a></li>
                        <li><a href="#">Disclaimer</a></li>
                    </
