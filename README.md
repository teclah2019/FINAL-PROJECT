# FINAL-PROJECT

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Blog</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="about.html">About</a></li>
                <li><a href="contact.html">Contact</a></li>
            </ul>
        </nav>
        <h1>Welcome to My Blog</h1>
    </header>
    
    <main>
        <section>
            <article>
                <h2>My First Blog Post</h2>
                <p>Welcome to my first post! Here's some interesting content...</p>
                <a href="single-post.html">Read more</a>
            </article>
            <article>
                <h2>Another Blog Post</h2>
                <p>This is another blog post with some more interesting content...</p>
                <a href="single-post.html">Read more</a>
            </article>
        </section>
    </main>
    
    <footer>
        <p>&copy; 2025 My Blog | All Rights Reserved</p>
    </footer>
    
    <script src="script.js"></script>
</body>
</html>


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Our Products</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="products.html">Products</a></li>
                <li><a href="cart.html">Cart</a></li>
            </ul>
        </nav>
        <h1>Our Products</h1>
    </header>

    <main>
        <section class="product-list">
            <article class="product">
                <img src="product1.jpg" alt="Product 1">
                <h3>Product 1</h3>
                <p>$19.99</p>
                <button>Add to Cart</button>
            </article>
            <article class="product">
                <img src="product2.jpg" alt="Product 2">
                <h3>Product 2</h3>
                <p>$29.99</p>
                <button>Add to Cart</button>
            </article>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 My Ecommerce Site | All Rights Reserved</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>


/* Reset default styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Header and navigation styles */
header {
    background-color: #333;
    color: white;
    padding: 20px;
}

header h1 {
    text-align: center;
}

header nav ul {
    list-style-type: none;
    text-align: center;
}

header nav ul li {
    display: inline;
    margin: 0 15px;
}

header nav ul li a {
    color: white;
    text-decoration: none;
}

/* Product styling */
.product-list {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
}

.product {
    background-color: #f9f9f9;
    padding: 20px;
    margin: 10px;
    width: 250px;
    text-align: center;
    border: 1px solid #ddd;
}

.product img {
    width: 100%;
    height: auto;
}

/* Responsive design */
@media (max-width: 600px) {
    header nav ul {
        display: block;
        text-align: left;
    }

    .product-list {
        flex-direction: column;
    }
}


// script.js for form validation (e.g., on the contact page)
document.querySelector('form').addEventListener('submit', function(event) {
    const name = document.querySelector('input[name="name"]').value;
    if (name === '') {
        alert('Please enter your name');
        event.preventDefault();
    }
});


// script.js for Ecommerce site: Add product to cart
document.querySelectorAll('.product button').forEach(button => {
    button.addEventListener('click', () => {
        alert('Product added to cart!');
    });
});
