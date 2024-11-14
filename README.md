/your-repo
    ├── index.html
    ├── not_found.html
    ├── thank_you.html
    ├── about_us.html
    ├── browse.html
    └── customer_service.html

    <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Main Page</title>
    <style>
        body {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            font-family: Arial, sans-serif;
            background-color: #000;
            color: #fff;
        }
        h1 {
            font-size: 36px;
            margin-bottom: 40px;
        }
        .button {
            padding: 15px 25px;
            font-size: 16px;
            color: #000;
            background-color: #fff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
            margin: 10px;
        }
        .button:hover {
            background-color: #ccc;
        }
    </style>
</head>
<body>
    <h1>Welcome to Our Website</h1>
    <button class="button" onclick="window.location.href='not_found.html'">Search</button>
    <button class="button" onclick="document.getElementById('email-input').style.display='block';">Sign Up</button>
    <button class="button" onclick="window.location.href='about_us.html'">About Us</button>
    <button class="button" onclick="window.location.href='browse.html'">Browse</button>
    <button class="button" onclick="window.location.href='customer_service.html'">Customer Service Number</button>

    <div id="email-input" style="display:none; margin-top: 20px;">
        <input type="email" placeholder="Enter your email" required>
        <button class="button" onclick="signUp()">Submit</button>
    </div>

    <script>
        function signUp() {
            document.getElementById('email-input').style.display = 'none';
            window.location.href = 'thank_you.html';
        }
    </script>
</body>
</html>
