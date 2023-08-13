<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Pomo Tasks</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
    <style>
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
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
            0% { background-position: 0% 50%; }
            50% { background-position: 50% 50%; }
            100% { background-position: 100% 50%; }
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

        .top-btn:hover { opacity: 1; }
        .top-btn {
            display: flex;
            justify-content: center;
            align-items: center;
            width: 50px;
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

        .last-updated-btn:hover { opacity: 1; }
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
            background-color: rgba(0, 0, 0, 0.8);
            color: #000;
        }

        .main-title {
            text-align: center;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.1);
            font-size: 36px;
            margin-top: 0;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Welcome to Pomo Tasks</h1>
        <h2>Your personal task manager</h2>
        <img src="https://via.placeholder.com/150" alt="Placeholder image">
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam nec odio neque. Nullam condimentum fermentum risus, sit amet fermentum justo euismod eu. Integer id dictum purus. Praesent accumsan est id turpis cursus, non sollicitudin sem tincidunt. Sed ut laoreet sapien, in dapibus odio. Fusce vel finibus eros.</p>
    </div>

    <a href="#" class="last-updated-btn" data-date="Updated: 7th July 2023">
        <!-- Update SVG Icon -->
        <svg viewBox="0 0 24 24" width="24" height="24">
            <path fill="currentColor" d="M13.7 5.8c-.7 0-1.3.6-1.3 1.3s.6 1.3 1.3 1.3 1.3-.6 1.3-1.3-.6-1.3-1.3-1.3zM12 0C5.4 0 0 5.4 0 12s5.4 12 12 12 12-5.4 12-12S18.6 0 12 0zm7.8 18.9c-.2.2-.4.3-.7.3s-.5-.1-.7-.3L12 14.3l-5.7 5.7c-.2.2-.4.3-.7.3s-.5-.1-.7-.3c-.4-.4-.4-1 0-1.4l6.4-6.4-6.4-6.4c-.4-.4-.4-1 0-1.4s1-.4 1.4 0L12 9.7l5.7-5.7c.4-.4 1-.4 1.4 0s.4 1 0 1.4l-6.4 6.4 6.4 6.4c.4.4.4 1 0 1.4z"></path>
        </svg>
    </a>

    <button class="dark-light-btn">
        <!-- Sun and Moon SVG Icon -->
        <svg viewBox="0 0 24 24" width="24" height="24">
            <path fill="currentColor" d="M11.98 22A10 10 0 111.22 4.04a9.978 9.978 0 0010.76 17.96zm-.61-2v-.03a8 8 0 10.61-15.95A7.955 7.955 0 0012 4a8 8 0 00-.03 16zm2.62-15.6a.5.5 0 010 .7l-.64.65a.5.5 0 01-.7-.7l.64-.65a.5.5 0 01.7 0zm3.5 2.2a.5.5 0 01-.7 0l-.65-.64a.5.5 0 01.7-.7l.65.64a.5.5 0 010 .7zm1.4 3.5a.5.5 0 01-.5-.5v-.93a.5.5 0 011 0v.93a.5.5 0 01-.5.5zm-13.3-.5a.5.5 0 01-.5-.5v-.93a.5.5 0 011 0v.93a.5.5 0 01-.5.5zm.9-5.7a.5.5 0 010 .7l-.65.65a.5.5 0 11-.7-.7l.65-.65a.5.5 0 01.7 0zm2.2-3.5a.5.5 0 01-.7 0l-.64-.65a.5.5 0 01.7-.7l.64.65a.5.5 0 010 .7z"></path>
        </svg>
    </button>

    <script>
        const lastUpdatedButton = document.querySelector(".last-updated-btn");
        const darkLightButton = document.querySelector(".dark-light-btn");
        const body = document.body;

        let darkMode = localStorage.getItem('darkMode');
        if (darkMode === "enabled") {
            body.classList.add('dark-mode');
        }

        darkLightButton.addEventListener("click", function() {
            if (body.classList.contains('dark-mode')) {
                body.classList.remove('dark-mode');
                localStorage.setItem('darkMode', null);
            } else {
                body.classList.add('dark-mode');
                localStorage.setItem('darkMode', 'enabled');
            }
        });

        lastUpdatedButton.addEventListener("mouseenter", function() {
            lastUpdatedButton.textContent = "Click Me!";
        });

        lastUpdatedButton.addEventListener("mouseleave", function() {
            lastUpdatedButton.innerHTML = `
                <!-- Update SVG Icon -->
                <svg viewBox="0 0 24 24" width="24" height="24">
                    <path fill="currentColor" d="M13.7 5.8c-.7 0-1.3.6-1.3 1.3s.6 1.3 1.3 1.3 1.3-.6 1.3-1.3-.6-1.3-1.3-1.3zM12 0C5.4 0 0 5.4 0 12s5.4 12 12 12 12-5.4 12-12S18.6 0 12 0zm7.8 18.9c-.2.2-.4.3-.7.3s-.5-.1-.7-.3L12 14.3l-5.7 5.7c-.2.2-.4.3-.7.3s-.5-.1-.7-.3c-.4-.4-.4-1 0-1.4l6.4-6.4-6.4-6.4c-.4-.4-.4-1 0-1.4s1-.4 1.4 0L12 9.7l5.7-5.7c.4-.4 1-.4 1.4 0s.4 1 0 1.4l-6.4 6.4 6.4 6.4c.4.4.4 1 0 1.4z"></path>
                </svg>
            `;
        });
    </script>
</body>
</html>
