
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GitHub Page</title>
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
            display: flex;
            flex-direction: column;
            gap: 20px;
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
        #email-input,
        #about-us,
        #thank-you {
            display: none;
            margin-top: 20px;
            padding: 15px;
            background-color: #222;
            border-radius: 5px;
            text-align: center;
        }
    </style>
</head>
<body>
    <h1>GitHub Page</h1>
    <div class="button-container">
        <button id="newsletter-button" class="button">Sign Up for Newsletter</button>
        <button id="about-us-button" class="button">About Us</button>
        <button id="add-to-cart-button" class="button">Add to Cart</button>
    </div>
    <div id="email-input">
        <input type="email" placeholder="Enter your email" required>
        <button class="button">Submit</button>
    </div>
    <div id="about-us">We are Pesendary!</div>
    <div id="thank-you">Thank you!</div>

    <script>
        const newsletterButton = document.getElementById('newsletter-button');
        const aboutUsButton = document.getElementById('about-us-button');
        const addToCartButton = document.getElementById('add-to-cart-button');
        const emailInputContainer = document.getElementById('email-input');
        const aboutUsContainer = document.getElementById('about-us');
        const thankYouMessage = document.getElementById('thank-you');

        newsletterButton.addEventListener('click', () => {
            emailInputContainer.style.display = 'block';
        });

        emailInputContainer.querySelector('button').addEventListener('click', () => {
            emailInputContainer.style.display = 'none';
            thankYouMessage.style.display = 'block';
        });

        aboutUsButton.addEventListener('click', () => {
            aboutUsContainer.style.display = 'block';
        });

        addToCartButton.addEventListener('click', () => {
            thankYouMessage.style.display = 'block';
        });
    </script>
</body>
</html>
