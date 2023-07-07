<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Pomo Tasks - Terms of Use</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --main-color: #F46036;
            --accent-color: #FF8338;
        }

        body {
            font-family: 'Montserrat', sans-serif;
            background: linear-gradient(to right, var(--main-color), var(--accent-color));
            color: #fff;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            text-align: center;
            overflow: hidden;
        }

        .container {
            max-width: 800px;
            margin: 20px;
            padding: 20px;
            box-shadow: 0 0 15px rgba(0,0,0,0.1);
            background: rgba(255,255,255,0.1);
            backdrop-filter: blur(5px);
            border-radius: 10px;
            border: 1px solid rgba(255,255,255,0.15);
            overflow: auto;
            height: 90vh;
        }

        img {
            width: 100px;
            margin-bottom: 20px;
        }

        h1, h2, h3, h4, p {
            margin: 10px 0;
            line-height: 1.6;
        }

        .top-btn {
            position: fixed;
            right: 30px;
            bottom: 30px;
            background: var(--accent-color);
            color: #fff;
            border: none;
            padding: 10px 15px;
            border-radius: 50px;
            text-decoration: none;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
            opacity: 0;
            transform: translateY(10px);
            transition: all 0.3s ease-in-out;
            display: none;
        }

        .top-btn.show {
            opacity: 1;
            transform: translateY(0);
            display: inline-block;
        }
    </style>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <script>
        $(document).ready(function() {
            var btn = $('.top-btn');

            $(window).scroll(function() {
                if ($(window).scrollTop() > 300) {
                    btn.addClass('show');
                } else {
                    btn.removeClass('show');
                }
            });

            btn.on('click', function(e) {
                e.preventDefault();
                $('html, body').animate({scrollTop:0}, '300');
            });
        });
    </script>
</head>
<body>
    <div class="container">
        <img src="logo.png" alt="Pomodoro Timer App logo">
        <h1>Terms and Conditions</h1>
        <p>Your access to and use of the Service is conditioned on your acceptance of and compliance with these Terms. These Terms apply to all visitors, users and others who access or use the Service.</p>
        <h2>1. Links To Other Web Sites</h2>
        <p>Our Service may contain links to third-party web sites or services that are not owned or controlled by Pomo Tasks.</p>
        <p>Pomo Tasks has no control over, and assumes no responsibility for, the content, privacy policies, or practices of any third party web sites or services. You further acknowledge and agree that Pomo Tasks shall not be responsible or liable, directly or indirectly, for any damage or loss caused or alleged to be caused by or in connection with use of or reliance on any such content, goods or services available on or through any such web sites or services.</p>
        <h2>2. Changes To This Terms of Use</h2>
        <p>We reserve the right, at our sole discretion, to modify or replace these Terms at any time. If a revision is material we will try to provide at least 30 days' notice prior to any new terms taking effect. What constitutes a material change will be determined at our sole discretion.</p>
        <h2>3. Contact Us</h2>
        <p>If you have any questions about these Terms, please contact us at pomotasks25@gmail.com.</p>
    </div>
    <a href="#" class="top-btn">Top</a>
</body>
</html>
