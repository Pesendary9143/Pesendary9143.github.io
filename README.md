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
        .button-container {
            display: flex; /* Use flexbox to align buttons horizontally */
            gap: 10px; /* Space between buttons */
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
        }
        .button:hover {
            background-color: #ccc;
        }
        #email-input {
            display: none;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <h1>Welcome to Our Website</h1>
    <div class="button-container">
        <button class="button" onclick="window.location.href='not_found.html'">Search</button>
        <button class="button" onclick="document.getElementById('email-input').style.display='block';">Sign Up</button>
        <button class="button" onclick="window.location.href='about_us.html'">About Us</button>
        <button class="button" onclick="window.location.href='browse.html'">Browse</button>
        <button class="button" onclick="window.location.href='customer_service.html'">Customer Service Number</button>
    </div>

    <div id="email-input">
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
