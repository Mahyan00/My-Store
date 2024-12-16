# My-Store
Welcome everyone Hello how are you
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Store</title>
    <link rel="stylesheet" href="style.css">
    <link rel="website icon" type="jpg" href="14.jpg">
</head>
<body>
    <!-- Header Section -->
    <header>
        <h1>Welcome to My Online Store</h1>
        <img src="14.jpg" alt="this img" width="280px">
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#products">Products</a></li>
                <li><a href="#contact">Contact</a></li>
                <li><a href="#cart">Cart</a></li>
            </ul>
        </nav>
    </header>

    <!-- Home Section -->
    <section id="home">
        <h2>Find the Best Products Here</h2>
        <img src="13.jpg" alt="img" width="300px">
        <p>Discover a variety of products tailored to your needs!</p>
    </section>

    <!-- Product Section -->
    <section id="products">
        <h2>Our Products</h2>
        <div class="product">
            <img src="13.jpg" alt="Product 1 Image">
            <h3>Product 1</h3>
            <p>Short description of Product 1.</p>
            <p>Price: $5.00</p>
            <button>Add to Cart</button>
        </div>
        <section id="products">
            <h2>Our Products</h2>
            <div class="product">
                <img src="12.jpg" alt="Product 1 Image">
                <h3>Product 1</h3>
                <p>Short description of Product 1.</p>
                <p>Price: $10.00</p>
                <button>Add to Cart</button>
            </div>
            <div class="product">
                <img src="11.jpg" alt="Product 2 Image">
                <h3>Product 2</h3>
                <p>Short description of Product 2.</p>
                <p>Price: $15.00</p>
                <button>Add to Cart</button>
            </div>
        </section>
        <!-- Add more products as needed -->
    </section>

    <!-- Cart Section -->
    <section id="cart">
        <h2>Your Cart</h2>
        <img src="12.jpg" alt="img" width="300px">
        <p>No items in the cart yet.</p>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <h2>Contact Us</h2>
        <form action="#">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            <label for="message">Message:</label>
            <textarea id="message" name="message" required></textarea>
            <button type="submit">Submit</button>
        </form>
    </section>

    <!-- Footer Section -->
    <footer>
        <p>&copy; 2024 My Online Store. All rights reserved.</p>
    </footer>
    <script src="script.js"></script>
    <script>
        // Initialize an empty cart array
let cart = [];

// Select cart section to display items
const cartSection = document.getElementById("cart");

// Sample product data
const products = [
    { id: 1, name: "Product 1", price: 10.00 },
    { id: 2, name: "Product 2", price: 15.00 }
];

// Function to add product to cart
function addToCart(productId) {
    // Find product by ID
    const product = products.find(item => item.id === productId);

    // Add product to cart
    cart.push(product);

    // Update cart display
    displayCart();
}

// Function to display items in the cart
function displayCart() {
    // Clear the cart section
    cartSection.innerHTML = "<h2>Your Cart</h2>";

    if (cart.length === 0) {
        cartSection.innerHTML += "<p>No items in the cart yet.</p>";
    } else {
        // Calculate total price
        let totalPrice = 0;

        cart.forEach((item, index) => {
            cartSection.innerHTML += `
                <div class="cart-item">
                    <p>${item.name} - $${item.price.toFixed(2)}</p>
                    <button onclick="removeFromCart(${index})">Remove</button>
                </div>
            `;
            totalPrice += item.price;
        });

        cartSection.innerHTML += `<p>Total Price: $${totalPrice.toFixed(2)}</p>`;
    }
}

// Function to remove item from cart
function removeFromCart(index) {
    // Remove item by index
    cart.splice(index, 1);

    // Update cart display
    displayCart();
}

// Event listeners for "Add to Cart" buttons
document.querySelectorAll('.product button').forEach((button, index) => {
    button.addEventListener('click', () => addToCart(products[index].id));
});

    </script>

</body>
</html>
