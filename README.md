<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Pomo Tasks</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
    <style>
        @keyframes fadeIn {
            from {
                opacity: 0;
            }

            to {
                opacity: 1;
            }
        }

        @keyframes float {
            0% {
                box-shadow: 0 5px 15px 0px rgba(0,0,0,0.6);
                transform: translateY(0px);
            }
            50% {
                box-shadow: 0 25px 15px 0px rgba(0,0,0,0.2);
                transform: translateY(-20px);
            }
            100% {
                box-shadow: 0 5px 15px 0px rgba(0,0,0,0.6);
                transform: translateY(0px);
            }
        }

        @keyframes gradientBG {
            0% {
                background-position: 0% 50%;
            }
            50% {
                background-position: 100% 50%;
            }
            100% {
                background-position: 0% 50%;
            }
        }

        body {
            font-family: 'Montserrat', sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #ff0000, #ff7f00, #ff6600, #ff5050);
            background-size: 200% 200%;
            animation: gradientBG 10s ease infinite;
            overflow-x: hidden;
        }

        .container {
            animation: fadeIn 1s, float 6s infinite;
            width: 80%;
            margin: 0 auto;
            padding: 20px;
            background-color: rgba(255, 255, 255, 0.9);
            border-radius: 10px;
            transition: background 0.5s;
        }

        h1 {
            color: #333;
            text-align: center;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
        }

        h2 {
            color: #666;
        }

        p {
            color: #333;
        }

        img {
            display: block;
            margin: 0 auto;
            width: 100px;
            box-shadow: 0px 5px 15px rgba(0,0,0,0.1);
            background-color: rgba(255, 255, 255, 0.9);
            padding: 20px;
            border-radius: 10px;
            opacity: 0.9;
        }

        .top-btn {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background: #ff7f00;
            color: white;
            padding: 10px 20px;
            border-radius: 50px;
            text-decoration: none;
            font-size: 14px;
            transition: all 0.3s;
            opacity: 0.7;
            display: none;
        }

        .top-btn:hover {
            opacity: 1;
        }

        .top-btn::before {
            content: "Scroll to top";
            position: absolute;
            bottom: 100%;
            left: 50%;
            opacity: 0;
            transform: translateX(-50%) scale(0.5);
            transition: all 0.3s;
            pointer-events: none;
        }

        .top-btn:hover::before {
            bottom: 120%;
            opacity: 1;
            transform: translateX(-50%) scale(1);
        }
    </style>
</head>
<body>
    <div class="container">
        <img src="P.png" alt="Pomodoro Timer App logo">
        <h1>Privacy Policy</h1>
        <h2>Last Updated: <span class="last-updated">July 7, 2023</span></h2>
        <h2>Introduction</h2>
        <p>Welcome to the Pomodoro Timer App! This Privacy Policy explains how we collect, use, disclose, and safeguard your information when you use our mobile application. Please read this policy carefully. If you disagree with its terms, please discontinue use of the application immediately.</p>

        <h2>Data Collection and Use</h2>
        <p>This app only collects data necessary for the payment process and for basic functionality of the application. We do not collect personal data outside of this scope.</p>
        <p>The data is only collected when you manually input it during the payment process.</p>
        <p>We use a third-party payment processing service called Revenue Cat to handle transactions. As such, some of your information may be shared with Revenue Cat during the transaction process. We recommend reviewing Revenue Cat’s privacy policy to understand how they use and protect your information.</p>

        <h2>User Rights</h2>
        <p>As we do not collect or store personal data beyond what is necessary for the payment process, user rights pertaining to data access, modification, or deletion may be limited. For any concerns or requests related to your data, please contact us directly.</p>

        <h2>Data Security</h2>
        <p>Your payment data is secure as it is processed through Revenue Cat, a third-party payment processing service, which implements its own security measures. We do not handle or store this data on our servers.</p>

        <h2>Children’s Privacy</h2>
        <p>Our application is intended for a general audience and does not knowingly collect or solicit personal information from anyone under the age of 13.</p>

        <h2>International Data Transfers</h2>
        <p>We do not transfer data internationally.</p>

        <h2>Changes to Privacy Policy</h2>
        <p>We may update this Privacy Policy as necessary. Any updates will be notified through the app.</p>

        <h2>Device Permissions</h2>
        <p>For the optimal functioning of the app, we require certain permissions from your device, such as access to notifications and live activities. These permissions do not involve access to your personal data and are solely used to ensure proper app functionality.</p>

        <h2>Contact Us</h2>
        <p>For any questions or concerns about this Privacy Policy, please contact us at:</p>
        <p>Email: pomotasks25@gmail.com</p>
        <p>Phone: +48 797543138</p>
    </div>
    <a href="#" class="top-btn">Top</a>
</body>
</html>
