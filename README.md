<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menu Card</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 20px;
        }

        .container {
            max-width: 800px;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        h1 {
            text-align: center;
            color: #333;
        }

        .menu {
            margin-bottom: 20px;
        }

        .menu-item {
            border-bottom: 1px solid #ccc;
            padding: 10px 0;
        }

        .menu-item h2 {
            margin: 0;
            color: #555;
        }

        .price {
            font-weight: bold;
            color: #e67e22;
        }

        button {
            background-color: #3498db;
            color: white;
            border: none;
            padding: 10px 15px;
            cursor: pointer;
            border-radius: 5px;
        }

        button:hover {
            background-color: #2980b9;
        }

        .cart {
            margin-top: 20px;
            padding: 10px;
            background-color: #f9f9f9;
            border: 1px solid #ccc;
            border-radius: 5px;
        }

        .cart h2 {
            margin: 0;
            color: #333;
        }

        .cart ul {
            list-style-type: none;
            padding: 0;
        }

        .cart li {
            margin: 5px 0;
        }

        .menu-item img {
            width: 15%;
            margin-bottom: 10px;
        }

        .buy-btn {
            background-color: #27ae60;
            padding: 12px 25px;
            border: none;
            border-radius: 5px;
            font-size: 18px;
            cursor: pointer;
            transition: background-color 0.3s;
            margin-top: 20px;
        }

        .buy-btn:hover {
            background-color: #3168de;
        }

        .message-box {
            margin-top: 20px;
        }

        .message-box input {
            width: calc(100% - 30px);
            padding: 10px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Restaurant Menu</h1>
        <div class="menu">
            <div class="menu-item">
                <h2>Spaghetti Carbonara</h2>
                <p>A classic Italian pasta dish made with eggs, cheese, pancetta, and pepper.</p>
                <div class="row">
                    <div class="column">
                        <img src="menu card pictures/Spaghetti Carbonara.jpg" alt="Spaghetti Carbonara">
                    </div>
                    <span class="price">$17.99</span>
                    <button onclick="addToCart('Spaghetti Carbonara', 17.99)">Add to Cart</button>
                </div>
            </div>
            <div class="menu-item">
                <h2>Blueberry Mojito</h2>
                <p>Fresh cocktail exported from Cuba.</p>
                <div class="row">
                    <div class="column">
                        <img src="menu card pictures/blueberry mojito.jpg" alt="blueberry mojito">
                    </div>
                    <span class="price">$14.99</span>
                    <button onclick="addToCart('Blueberry Mojito', 14.99)">Add to Cart</button>
                </div>
            </div>
            <div class="menu-item">
                <h2>Fruit Salad</h2>
                <p>Fruit salads are an excellent way to get a variety of essential nutrients all in one delicious serving.</p>
                <div class="row">
                    <div class="column">
                        <img src="menu card pictures/Fruit Salad.jpg" alt="Fruit Salad">
                    </div>
                    <span class="price">$10.99</span>
                    <button onclick="addToCart('Fruit Salad', 10.99)">Add to Cart</button>
                </div>
            </div>
            <div class="menu-item">
                <h2>Hot Ham Cheese Sliders</h2>
                <p>Baked ham and cheese sliders are the most delicious sandwiches.</p>
                <div class="row">
                    <div class="column">
                        <img src="menu card pictures/Hot Ham Cheese Sliders.jpg" alt="Hot Ham Cheese Sliders">
                    </div>
                    <span class="price">$12.99</span>
                    <button onclick="addToCart('Hot Ham Cheese Sliders', 12.99)">Add to Cart</button>
                </div>
            </div>
            <div class="menu-item">
                <h2>Steak Fries</h2>
                <p>Wedges of potatoes fried to crispy perfection.</p>
                <div class="row">
                    <div class="column">
                        <img src="menu card pictures/Steak fries.jpg" alt="Steak fries">
                    </div>
                    <span class="price">$8.99</span>
                    <button onclick="addToCart('Steak Fries', 8.99)">Add to Cart</button>
                </div>
            </div>
            <div class="menu-item">
                <h2>Cheesecake Brownies</h2>
                <p>Fudgy brownies and creamy cheesecake.</p>
                <div class="row">
                    <div class="column">
                        <img src="menu card pictures/Cheesecake brownies.jpg" alt="Cheesecake brownies">
                    </div>
                    <span class="price">$10.99</span>
                    <button onclick="addToCart('Cheesecake Brownies', 10.99)">Add to Cart</button>
                </div>
            </div>
            <div class="menu-item">
                <h2>Chilli Cheese Toast</h2>
                <p>Popular snack and street food in India.</p>
                <div class="row">
                    <div class="column">
                        <img src="menu card pictures/Chilli cheese toast.jpg" alt="Chilli cheese toast">
                    </div>
                    <span class="price">$10.99</span>
                    <button onclick="addToCart('Chilli Cheese Toast', 10.99)">Add to Cart</button>
                </div>
            </div>
            <div class="menu-item">
                <h2>Veg Burger</h2>
                <p>Say hello to the BEST veggie burger!</p>
                <div class="row">
                    <div class="column">
                        <img src="menu card pictures/Veg burger.jpg" alt="Veg burger">
                    </div>
                    <span class="price">$9.99</span>
                    <button onclick="addToCart('Veg Burger', 9.99)">Add to Cart</button>
                </div>
            </div>
            <div class="menu-item">
                <h2>Hot Dog</h2>
                <p>Grilled, steamed, or boiled sausage.</p>
                <div class="row">
                    <div class="column">
                        <img src="menu card pictures/Hot dog.jpg" alt="Hot dog">
                    </div>
                    <span class="price">$5.99</span>
                    <button onclick="addToCart('Hot Dog', 5.99)">Add to Cart</button>
                </div>
            </div>
        </div>
        <div id="cart" class="cart">
            <h2>Your Cart</h2>
            <ul id="cart-items"></ul>
            <p id="total-price">Total: $0.00</p>
        </div>
        <div class="message-box">
            <input type="text" id="message" placeholder="Enter your message here">
            <button class="buy-btn" onclick="buyNow()">Buy Now</button>
        </div>
    </div>
    <script>
        let cart = [];
        let total = 0;

        function addToCart(item, price) {
            cart.push(item);
            total += price;
            updateCart();
        }

        function updateCart() {
            const cartItems = document.getElementById('cart-items');
            cartItems.innerHTML = '';

            cart.forEach((item) => {
                const li = document.createElement('li');
                li.textContent = item;
                cartItems.appendChild(li);
            });

            document.getElementById('total-price').textContent = `Total: $${total.toFixed(2)}`;
        }

        function buyNow() {
            const email = "itsangryend@gmail.com"; // Replace with
            // Replace with the recipient's email
            const subject = "Order from Restaurant Menu"; // Email subject
            const message = document.getElementById('message').value; // User's message
            let body = `Order details:\n\nItems:\n`;

            cart.forEach(item => {
                body += `- ${item}\n`;
            });

            body += `\nTotal: $${total.toFixed(2)}\n\nMessage: ${message}`;

            window.location.href = `mailto:${email}?subject=${encodeURIComponent(subject)}&body=${encodeURIComponent(body)}`;
        }
    </script>
</body>
</html>
