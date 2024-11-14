<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Email Sign-Up</title>
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
            margin-bottom: 20px;
        }
        #email-input {
            padding: 10px;
            font-size: 16px;
            border: 1px solid #ccc;
            border-radius: 5px;
            width: 250px;
            margin-bottom: 20px;
            background-color: #000;
            color: #fff;
        }
        #sign-up-button {
            padding: 10px 20px;
            font-size: 16px;
            color: #000;
            background-color: #fff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        #sign-up-button:hover {
            background-color: #ccc;
        }
        #thank-you {
            font-size: 24px;
            display: none;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <h1>Sign Up for Our Newsletter</h1>
    <input type="email" id="email-input" placeholder="Enter your email" required>
    <button id="sign-up-button">Sign Up</button>
    <div id="thank-you">Thank you for signing up!</div>

    <script>
        const signUpButton = document.getElementById('sign-up-button');
        const thankYouMessage = document.getElementById('thank-you');

        signUpButton.addEventListener('click', () => {
            const emailInput = document.getElementById('email-input');
            if (emailInput.value.trim() !== '') {
                emailInput.value = '';
                thankYouMessage.style.display = 'block';
            }
        });
    </script>
</body>
</html>
