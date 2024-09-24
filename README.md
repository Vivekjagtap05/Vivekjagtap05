HTML 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Book Store</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Navigation Bar -->
    <header>
        <h1>Book Store</h1>
        <nav>
            <ul>
                <li><a href="#books">Books</a></li>
                <li><a href="#about">About Us</a></li>
                <li><a href="#contact">Contact</a></li>
                <li><a href="#cart">Cart (<span id="cart-count">0</span>)</a></li>
            </ul>
        </nav>
    </header>

    <!-- Main Section -->
    <section id="books">
        <h2>Our Books</h2>
        <div class="book-container">
            <div class="book">
                <img src="book1.jpg" alt="Book 1">
                <h3>Book Title 1</h3>
                <p class="price">$10.00</p>
                <button class="add-to-cart" data-title="Book Title 1" data-price="10.00">Add to Cart</button>
            </div>
            <div class="book">
                <img src="book2.jpg" alt="Book 2">
                <h3>Book Title 2</h3>
                <p class="price">$15.00</p>
                <button class="add-to-cart" data-title="Book Title 2" data-price="15.00">Add to Cart</button>
            </div>
            <div class="book">
                <img src="book3.jpg" alt="Book 3">
                <h3>Book Title 3</h3>
                <p class="price">$20.00</p>
                <button class="add-to-cart" data-title="Book Title 3" data-price="20.00">Add to Cart</button>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about">
        <h2>About Us</h2>
        <p>Welcome to our book store! We offer a wide variety of books for all ages and interests. Whether you're looking for the latest bestseller or a classic, we've got you covered.</p>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <h2>Contact Us</h2>
        <p>Email: support@bookstore.com</p>
        <p>Phone: (123) 456-7890</p>
    </section>

    <!-- Cart Section -->
    <section id="cart">
        <h2>Your Cart</h2>
        <div id="cart-items">
            <p>Your cart is empty.</p>
        </div>
        <div id="cart-total">
            <p>Total: $<span id="total-price">0.00</span></p>
        </div>
    </section>

    <script src="scripts.js"></script>
</body>
</html>

 css
 /* Basic Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    color: #333;
}

/* Header and Navigation */
header {
    background-color: #333;
    color: white;
    padding: 10px 0;
    text-align: center;
}

header h1 {
    margin: 10px 0;
}

nav ul {
    list-style-type: none;
}

nav ul li {
    display: inline;
    margin-right: 20px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-weight: bold;
}

/* Main Content Styles */
section {
    padding: 20px;
    max-width: 1200px;
    margin: auto;
}

h2 {
    margin-bottom: 20px;
    text-align: center;
}

.book-container {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}

.book {
    background-color: white;
    padding: 15px;
    margin: 10px;
    width: 30%;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    text-align: center;
}

.book img {
    max-width: 100%;
    height: auto;
}

.book h3 {
    margin: 10px 0;
}

.price {
    color: #f00;
    font-weight: bold;
}

button.add-to-cart {
    padding: 10px 15px;
    background-color: #333;
    color: white;
    border: none;
    cursor: pointer;
    margin-top: 10px;
}

button.add-to-cart:hover {
    background-color: #555;
}

/* About and Contact Sections */
#about, #contact {
    background-color: #fff;
    padding: 20px;
    margin-top: 20px;
    text-align: center;
}

#about p, #contact p {
    margin-bottom: 10px;
}

/* Cart Section */
#cart {
    background-color: white;
    padding: 20px;
    margin-top: 20px;
    text-align: center;
}

#cart-items {
    margin-bottom: 20px;
}

#cart-total {
    font-weight: bold;
}

#cart-total span {
    color: #f00;
}
/* Basic Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    color: #333;
}

/* Header and Navigation */
header {
    background-color: #333;
    color: white;
    padding: 10px 0;
    text-align: center;
}

header h1 {
    margin: 10px 0;
}

nav ul {
    list-style-type: none;
}

nav ul li {
    display: inline;
    margin-right: 20px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-weight: bold;
}

/* Main Content Styles */
section {
    padding: 20px;
    max-width: 1200px;
    margin: auto;
}

h2 {
    margin-bottom: 20px;
    text-align: center;
}

.book-container {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}

.book {
    background-color: white;
    padding: 15px;
    margin: 10px;
    width: 30%;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    text-align: center;
}

.book img {
    max-width: 100%;
    height: auto;
}

.book h3 {
    margin: 10px 0;
}

.price {
    color: #f00;
    font-weight: bold;
}

button.add-to-cart {
    padding: 10px 15px;
    background-color: #333;
    color: white;
    border: none;
    cursor: pointer;
    margin-top: 10px;
}

button.add-to-cart:hover {
    background-color: #555;
}

/* About and Contact Sections */
#about, #contact {
    background-color: #fff;
    padding: 20px;
    margin-top: 20px;
    text-align: center;
}

#about p, #contact p {
    margin-bottom: 10px;
}

/* Cart Section */
#cart {
    background-color: white;
    padding: 20px;
    margin-top: 20px;
    text-align: center;
}

#cart-items {
    margin-bottom: 20px;
}

#cart-total {
    font-weight: bold;
}

#cart-total span {
    color: #f00;
}
javascript 
// JavaScript for Cart Functionality
let cart = [];

// Function to update cart count
function updateCartCount() {
    document.getElementById("cart-count").innerText = cart.length;
}

// Function to update cart total price
function updateCartTotal() {
    let total = 0;
    cart.forEach(item => {
        total += parseFloat(item.price);
    });
    document.getElementById("total-price").innerText = total.toFixed(2);
}

// Function to render cart items
function renderCartItems() {
    const cartItemsContainer = document.getElementById("cart-items");
    cartItemsContainer.innerHTML = '';

    if (cart.length === 0) {
        cartItemsContainer.innerHTML = '<p>Your cart is empty.</p>';
    } else {
        cart.forEach((item, index) => {
            const itemElement = document.createElement("div");
            itemElement.innerText = `${item.title} - $${item.price}`;
            cartItemsContainer.appendChild(itemElement);
        });
    }
}

// Function to add a book to the cart
function addToCart(title, price) {
    cart.push({ title, price });
    updateCartCount();
    updateCartTotal();
    renderCartItems();
}

// Event listeners for "Add to Cart" buttons
document.querySelectorAll('.add-to-cart').forEach(button => {
    button.addEventListener('click', () => {
        const title = button.getAttribute('data-title');
        const price = button.getAttribute('data-price');
        addToCart(title, price);
    });
});
