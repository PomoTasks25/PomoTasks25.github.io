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
                background-position: 50% 50%;
            }
            100% {
                background-position: 100% 50%;
            }
        }

body {
    font-family: 'Montserrat', sans-serif;
    margin: 0;
    padding: 0;
    background: #FCE1C6;
    overflow-x: hidden;
    color: #fff;
}

        .container {
            animation: fadeIn 1s;
            width: 80%;
            margin: 0 auto;
            padding: 20px;
            background-color: rgba(0, 0, 0, 0.8);
            border-radius: 10px;
            transition: background 0.5s;
            box-shadow: 0px 5px 15px rgba(0,0,0,0.1);
        }

        h1 {
            text-align: center;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.1);
            font-size: 36px;
            margin-top: 0;
        }

        h2 {
            font-size: 24px;
            color: #999;
            margin-bottom: 10px;
        }

        p {
            margin-bottom: 10px;
        }

        img {
            display: block;
            margin: 20px auto;
            width: 100px;
            border-radius: 50%;
            box-shadow: 0px 5px 15px rgba(0,0,0,0.2);
        }

.top-btn:hover {
    opacity: 1;
}

/* Removed the .top-btn::before, .top-btn:hover::before styles since you no longer want the red circle effect */

.top-btn {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 50px; /* Adjust width and height to better fit the SVG */
    height: 50px;
}



.last-updated-btn {
    position: fixed;
    top: 20px;
    right: 20px;
    background: #E82620;
    color: white;
    padding: 10px 20px;
    border-radius: 50px;
    text-decoration: none;
    font-size: 14px;
    transition: all 0.3s;
    opacity: 0.7;
    display: none;
    z-index: 9999;
}

        .last-updated-btn:hover {
            opacity: 1;
        }

        .last-updated-btn::before {
            content: attr(data-date);
            position: absolute;
            top: 100%;
            left: 50%;
            opacity: 0;
            transform: translateX(-50%) scale(0.5);
            transition: all 0.3s;
            pointer-events: none;
        }

        .last-updated-btn:hover::before {
            top: 120%;
            opacity: 1;
            transform: translateX(-50%) scale(1);
        }

        /* Dark/Light Mode Button */
        
.dark-light-btn {
    position: fixed;
    top: 20px;
    left: 20px;
    background: #E82620;
    color: #fff;
    border: none;
    border-radius: 50%;
    width: 40px;
    height: 40px;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 20px;
    cursor: pointer;
    transition: background 0.3s, color 0.3s;
    z-index: 9999;
}

.dark-light-btn:hover {
    background: #fff;
    color: #E82620;
}

.dark-mode {
    background: #E7B580;
    color: #fff;
}

.dark-mode .container {
    background-color: rgba(0, 0, 0, 0.8); /* or any other color of your choice */
    color: #000;
}

.main-title {
    text-align: center;
    text-shadow: 2px 2px 4px rgba(0,0,0,0.1);
    font-size: 36px;
    margin-top: 0;
    color: #D31A1E;  /* Color change */
}

.sub-title {
    font-size: 24px;
    color: #D31A1E; /* Updated color */
    margin-bottom: 10px;
}

.sub-title-small {
    font-size: 20px;
    color: #D31A1E; /* Updated color */
    margin-bottom: 10px;
}

h1, h2, h3, h4, h5, h6 {
            display: none;
        }
    </style>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>

    <script>
        $(document).ready(function() {
            // Dark/Light Mode
            $('.dark-light-btn').click(function() {
                $('body').toggleClass('dark-mode');
            });

            $(window).scroll(function() {
                if ($(this).scrollTop() > 200) {
                    $('.top-btn').fadeIn();
                } else {
                    $('.top-btn').fadeOut();
                }
            });

            $('.top-btn').click(function() {
                $('html, body').animate({scrollTop: 0}, 800);
                return false;
            });

            $('.last-updated-btn').fadeIn();
        });
    </script>

</head>

<body>
    
<div class="container">
    <img src="appstore.png" alt="Pomodoro Timer App logo">
    <p class="main-title">Welcome to the Pomo Tasks App!</p>
    <p>This Privacy Policy explains how we collect, use, disclose, and safeguard your information when you use our mobile application. Please read this policy carefully. If you disagree with its terms, please discontinue use of the application immediately.</p>

    <p class="sub-title">Data Collection and Use</p>
    <p>This app only collects data necessary for the payment process and for basic functionality of the application. We do not collect personal data outside of this scope.</p>
    <p>The data is only collected when you manually input it during the payment process.</p>
    <p>We use a third-party payment processing service called Revenue Cat to handle transactions. As such, some of your information may be shared with Revenue Cat during the transaction process. We recommend reviewing Revenue Cat’s privacy policy to understand how they use and protect your information.</p>

    <p class="sub-title">User Rights</p>
    <p>As we do not collect or store personal data beyond what is necessary for the payment process, user rights pertaining to data access, modification, or deletion may be limited. For any concerns or requests related to your data, please contact us directly.</p>

    <p class="sub-title">Data Security</p>
    <p>Your payment data is secure as it is processed through Revenue Cat, a third-party payment processing service, which implements its own security measures. We do not handle or store this data on our servers.</p>

    <p class="sub-title">Children’s Privacy</p>
    <p>Our application is intended for a general audience and does not knowingly collect or solicit personal information from anyone under the age of 13.</p>

    <p class="sub-title">International Data Transfers</p>
    <p>We do not transfer data internationally.</p>

    <p class="sub-title">Changes to Privacy Policy</p>
    <p>We may update this Privacy Policy as necessary. Any updates will be notified through the app.</p>

    <p class="sub-title">Device Permissions</p>
    <p>For the optimal functioning of the app, we require certain permissions from your device, such as access to notifications and live activities. These permissions do not involve access to your personal data and are solely used to ensure proper app functionality.</p>

    <p class="sub-title">Contact Us</p>
    <p>For any questions or concerns about this Privacy Policy, please contact us at:</p>
    <p>Email: pomotasks25@gmail.com</p>
    <p>Phone: +48 797543138</p>

    <p class="sub-title">Support</p>
    <p>If you encounter any issues while using our app or have any other concerns that need our assistance, you can contact our support team. We're here to help you!</p>
    <p>Here are the ways you can reach us:</p>

    <h3>Email</h3>
<p>For any general queries or technical support, please email us at <a href="mailto:pomotasks25@gmail.com">pomotasks25@gmail.com</a>. We aim to respond to your inquiries within 48 hours.</p>

    <h3>Phone</h3>
<p>You can also reach out to us via phone at +48 797 543 138. Our support team is available from Monday to Friday, 9:00 AM to 5:00 PM (Central European Time).</p>

</div>
<a href="#" class="top-btn">
  <svg xmlns="http://www.w3.org/2000/svg" x="0px" y="0px" width="100" height="100" viewBox="0 0 48 48">
    <path fill="#90caf9" d="M38.35,39.3c0.8,0.8,2,0.8,2.8,0l4.1-4.1c0.8-0.8,0.8-2,0-2.8l-15.8-15.8c-0.8-0.8-2-0.8-2.8,0	l-15.9,15.9c-0.8,0.8-0.8,2,0,2.8l4.1,4.1c0.8,0.8,2,0.8,2.8,0L28.05,29L38.35,39.3z"></path>
    <path fill="none" stroke="#18193f" stroke-linecap="round" stroke-linejoin="round" stroke-miterlimit="10" stroke-width="3" d="M20.664,28.386L24.05,25l10.3,10.3c0.8,0.8,2,0.8,2.8,0l4.1-4.1c0.8-0.8,0.8-2,0-2.8l-7.527-7.527"></path>
    <path fill="none" stroke="#18193f" stroke-linecap="round" stroke-linejoin="round" stroke-miterlimit="10" stroke-width="3" d="M28.914,16.064L25.45,12.6c-0.8-0.8-2-0.8-2.8,0L6.75,28.5c-0.8,0.8-0.8,2,0,2.8l4.1,4.1c0.8,0.8,2,0.8,2.8,0l2.066-2.066"></path>
  </svg>
</a>

<a href="#" class="last-updated-btn" data-date="Last Updated: August 13, 2023">Last Updated</a>
<button class="dark-light-btn" title="Toggle Dark/Light Mode">🌓</button>

</body>

</html>
