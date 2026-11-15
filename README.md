
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>REL Atelier | Luxury Bags</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Playfair+Display:wght@400;500;600;700&display=swap');

:root {
    --cream: #f8f5ef;
    --beige: #e9ded1;
    --brown: #302018;
    --gold: #c49b65;
    --white: #fffefa;
    --text: #51473f;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
}

body {
    font-family: 'DM Sans', sans-serif;
    background: var(--cream);
    color: var(--brown);
}

/* NAVIGATION */

header {
    background: var(--white);
    position: sticky;
    top: 0;
    z-index: 100;
    box-shadow: 0 2px 12px #00000008;
}

.navbar {
    max-width: 1250px;
    margin: auto;
    padding: 22px 5%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
    gap: 15px;
}

.logo {
    font-family: 'Playfair Display', serif;
    font-size: 30px;
    font-weight: bold;
    letter-spacing: 4px;
}

.logo span {
    font-family: 'DM Sans', sans-serif;
    color: var(--gold);
    font-size: 11px;
    letter-spacing: 5px;
}

nav {
    display: flex;
    gap: 25px;
    flex-wrap: wrap;
}

nav a {
    text-decoration: none;
    color: var(--brown);
    font-size: 13px;
    font-weight: 700;
    letter-spacing: 1px;
}

nav a:hover {
    color: var(--gold);
}

.cart-button {
    background: var(--brown);
    color: white;
    border: none;
    padding: 13px 22px;
    cursor: pointer;
    font-weight: bold;
}

/* GENERAL */

section {
    padding: 85px 7%;
    scroll-margin-top: 90px;
}

.eyebrow {
    color: #967750;
    font-size: 12px;
    font-weight: bold;
    letter-spacing: 3px;
    margin-bottom: 20px;
}

h1, h2, h3 {
    font-family: 'Playfair Display', serif;
}

.section-heading {
    text-align: center;
    margin-bottom: 50px;
}

.section-heading h2 {
    font-size: clamp(30px, 5vw, 45px);
    margin-bottom: 15px;
}

.section-heading p {
    color: #81776e;
    line-height: 1.8;
}

/* HERO */

.hero {
    min-height: 650px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 100px 8%;
    background: linear-gradient(135deg, #f9f6f0, #eee3d7);
}

.hero h1 {
    font-size: clamp(42px, 8vw, 75px);
    line-height: 1.15;
    max-width: 850px;
    margin-bottom: 25px;
}

.hero h1 em {
    color: #ad8c68;
}

.hero p {
    max-width: 720px;
    color: #756d66;
    font-size: 17px;
    line-height: 1.9;
    margin-bottom: 35px;
}

.btn {
    display: inline-block;
    background: var(--brown);
    color: white;
    padding: 17px 35px;
    text-decoration: none;
    border: none;
    cursor: pointer;
    font-weight: bold;
    letter-spacing: 1px;
    transition: .3s;
}

.btn:hover {
    background: #73543c;
    transform: translateY(-2px);
}

/* PRODUCTS */

.products {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 30px;
    max-width: 1100px;
    margin: auto;
}

.product-card {
    background: var(--white);
    border: 1px solid #e8e1d8;
    transition: .3s;
}

.product-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 15px 30px #0000000c;
}

.product-image {
    height: 340px;
    background: #f0ece5;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
}

.product-image img {
    width: 100%;
    height: 100%;
    object-fit: contain;
    padding: 15px;
}

.product-info {
    padding: 27px;
}

.tag {
    display: inline-block;
    background: #eee5d9;
    color: #79644d;
    padding: 9px 13px;
    font-size: 11px;
    font-weight: bold;
    letter-spacing: 1px;
    margin-bottom: 15px;
}

.product-info h3 {
    font-size: 23px;
    margin-bottom: 12px;
}

.price {
    font-size: 22px;
    font-weight: bold;
    margin-bottom: 20px;
}

.add-btn {
    width: 100%;
    padding: 15px;
    border: none;
    background: var(--brown);
    color: white;
    font-weight: bold;
    letter-spacing: 1px;
    cursor: pointer;
}

.add-btn:hover {
    background: #73543c;
}

.product-info p {
    color: #81776e;
    line-height: 1.8;
    margin-top: 22px;
}

/* STORY */

.story {
    background: var(--beige);
    text-align: center;
}

.story-content {
    max-width: 750px;
    margin: auto;
}

.story h2 {
    font-size: 45px;
    margin-bottom: 25px;
}

.story p {
    color: #756d66;
    font-size: 17px;
    line-height: 2;
}

/* ORDER SECTION */

.order-section {
    background: var(--brown);
    color: white;
}

.order-container {
    max-width: 850px;
    margin: auto;
}

.order-section .section-heading p {
    color: #d5c7b8;
}

.order-box {
    background: #453127;
    border: 1px solid #655043;
    padding: 35px;
    margin-bottom: 30px;
    border-radius: 5px;
}

.order-box h2 {
    font-size: 29px;
    margin-bottom: 25px;
}

.cart-item {
    display: flex;
    justify-content: space-between;
    gap: 15px;
    padding: 15px 0;
    border-bottom: 1px solid #665247;
}

.remove-btn {
    background: transparent;
    color: #e5b879;
    border: none;
    cursor: pointer;
    margin-left: 10px;
}

.total {
    display: flex;
    justify-content: space-between;
    color: #e5b879;
    font-weight: bold;
    font-size: 20px;
    margin-top: 25px;
}

.empty {
    color: #d5c7b8;
    line-height: 1.8;
}

/* FORM */

form label {
    display: block;
    margin: 20px 0 10px;
    font-weight: bold;
}

form input, form select, form textarea {
    width: 100%;
    padding: 17px;
    background: var(--white);
    border: 1px solid #d9cbbd;
    font-family: inherit;
    font-size: 15px;
    border-radius: 3px;
}

form button {
    width: 100%;
    margin-top: 25px;
    background: #e6b980;
    color: var(--brown);
    border: none;
    padding: 18px;
    font-weight: bold;
    letter-spacing: 1px;
    cursor: pointer;
}

form button:hover {
    background: #f0cca2;
}

.notice {
    color: #d5c7b8;
    line-height: 1.8;
    margin-top: 20px;
    font-size: 14px;
}

/* FOOTER */

footer {
    background: #211711;
    color: #d9c6b0;
    text-align: center;
    padding: 35px 15px;
    font-size: 13px;
    line-height: 2;
}

footer strong {
    color: #d7ae7a;
}

/* RESPONSIVE */

@media(max-width: 650px) {

    .navbar {
        justify-content: center;
    }

    nav {
        justify-content: center;
        gap: 14px;
    }

    nav a {
        font-size: 11px;
    }

    .logo {
        text-align: center;
    }

    .hero {
        min-height: 550px;
    }

    .hero p {
        font-size: 15px;
    }

    section {
        padding: 65px 5%;
    }

    .products {
        grid-template-columns: 1fr;
        gap: 25px;
    }

    .product-image {
        height: 300px;
    }

    .story h2 {
        font-size: 35px;
    }

    .order-box {
        padding: 23px;
    }
}
</style>
</head>

<body>

<!-- NAVIGATION -->

<header>
    <div class="navbar">

        <div class="logo">
            REL <span>ATELIER</span>
        </div>

        <nav>
            <a href="#home">HOME</a>
            <a href="#collection">BAG COLLECTION</a>
            <a href="#story">OUR STORY</a>
            <a href="#order">ORDER</a>
        </nav>

        <button class="cart-button"
        onclick="goToOrder()">
            MY BAG (<span id="cart-count">0</span>)
        </button>

    </div>
</header>


<!-- HOMEPAGE -->

<section class="hero" id="home">

    <div class="eyebrow">THE ART OF THE EVERYDAY</div>

    <h1>
        Make an entrance.<br>
        <em>Carry it beautifully.</em>
    </h1>

    <p>
        Meet the REL Atelier collection:
        timeless bags with refined details,
        elegant finishes, and a quietly
        luxurious feel.
    </p>

    <a href="#collection" class="btn">
        DISCOVER THE COLLECTION
    </a>

    <p style="margin-top:35px;font-size:14px;">
        ✦ Signature style, thoughtfully chosen.
    </p>

</section>


<!-- COLLECTION -->

<section id="collection">

    <div class="section-heading">

        <div class="eyebrow">
            THE REL ATELIER COLLECTION
        </div>

        <h2>Find your forever bag</h2>

        <p>
            Elegant silhouettes and considered
            details for every occasion.
        </p>

    </div>


    <div class="products" id="product-list">

        <!-- PRODUCT 1 -->

        <div class="product-card">

            <div class="product-image">
                <img
                src="https://images.unsplash.com/photo-1584917865442-de89df76afd3?w=900"
                alt="Black quilted handbag">
            </div>

            <div class="product-info">

                <span class="tag">QUILTED SIGNATURE</span>

                <h3>The Élise Top Handle</h3>

                <div class="price">₱100,000</div>

                <button class="add-btn"
                onclick="addToCart(0)">
                    ADD TO CART
                </button>

                <p>
                    A polished, structured silhouette
                    for dinners, events, and special occasions.
                </p>

            </div>
        </div>


        <!-- PRODUCT 2 -->

        <div class="product-card">

            <div class="product-image">
                <img
                src="https://images.unsplash.com/photo-1590874103328-eac38a683ce7?w=900"
                alt="Elegant shoulder handbag">
            </div>

            <div class="product-info">

                <span class="tag">WOVEN CLASSIC</span>

                <h3>The Margot Shoulder Bag</h3>

                <div class="price">₱99,000</div>

                <button class="add-btn"
                onclick="addToCart(1)">
                    ADD TO CART
                </button>

                <p>
                    A refined and versatile shoulder bag
                    with room for your everyday essentials.
                </p>

            </div>
        </div>


        <!-- PRODUCT 3 -->

        <div class="product-card">

            <div class="product-image">
                <img
                src="https://images.unsplash.com/photo-1548036328-c9fa89d128fa?w=900"
                alt="Mini fashion handbag">
            </div>

            <div class="product-info">

                <span class="tag">EVENING COLLECTION</span>

                <h3>The Noelle Mini Bag</h3>

                <div class="price">₱125,000</div>

                <button class="add-btn"
                onclick="addToCart(2)">
                    ADD TO CART
                </button>

                <p>
                    A compact statement piece made
                    to complete your evening look.
                </p>

            </div>
        </div>


        <!-- PRODUCT 4 -->

        <div class="product-card">

            <div class="product-image">
                <img
                src="https://images.unsplash.com/photo-1566150905458-1bf1fc113f0d?w=900"
                alt="Elegant structured tote bag">
            </div>

            <div class="product-info">

                <span class="tag">ATELIER SIGNATURE</span>

                <h3>The Celeste Tote</h3>

                <div class="price">₱150,000</div>

                <button class="add-btn"
                onclick="addToCart(3)">
                    ADD TO CART
                </button>

                <p>
                    A graceful, spacious tote for
                    workdays, weekends, and everything between.
                </p>

            </div>
        </div>

    </div>

    <p style="text-align:center;color:#81776e;margin-top:40px;line-height:2;">
        Beautifully chosen bags to carry, cherish,
        and keep for years to come.
        These are independent REL Atelier designs.
    </p>

</section>


<!-- OUR STORY -->

<section class="story" id="story">

    <div class="story-content">

        <div class="eyebrow">
            A MORE THOUGHTFUL WAY TO CHOOSE
        </div>

        <h2>For every day worth dressing up.</h2>

        <p>
            REL Atelier brings together timeless
            women's bags with thoughtful details
            and lasting style.

            From a polished everyday companion
            to a special-occasion piece, discover
            a bag you'll love to carry season
            after season.
        </p>

    </div>

</section>


<!-- ORDER SECTION -->

<section class="order-section" id="order">

    <div class="order-container">

        <div class="section-heading">

            <div class="eyebrow">
                SELECTED WITH CARE
            </div>

            <h2>Your bag order</h2>

            <p>
                Review your selection, enter your details,
                and choose pickup or delivery.
            </p>

        </div>


        <!-- CART -->

        <div class="order-box">

            <h2>Your Selection</h2>

            <div id="cart-items">
                <p class="empty">
                    Your selection is empty.
                    Explore the collection to find your bag.
                </p>
            </div>

            <div class="total">

                <span>Estimated total</span>

                <span id="total-price">₱0.00</span>

            </div>

            <p class="notice">
                Final order details will be confirmed
                by the atelier.
            </p>

        </div>


        <!-- CUSTOMER FORM -->

        <div class="order-box">

            <h2>Order details</h2>

            <form id="order-form">

                <label>Full name</label>

                <input
                type="text"
                id="customer-name"
                placeholder="e.g. Alex Santos"
                required>


                <label>Mobile number</label>

                <input
                type="tel"
                id="customer-phone"
                placeholder="e.g. 09XX XXX XXXX"
                required>


                <label>Email address</label>

                <input
                type="email"
                id="customer-email"
                placeholder="Your email address"
                required>


                <label>How would you like to receive it?</label>

                <select id="delivery" required>

                    <option value="Store pickup">
                        Store pickup
                    </option>

                    <option value="Home delivery">
                        Home delivery
                    </option>

                </select>


                <label>Payment preference</label>

                <select id="payment" required>

                    <option value="Cash">
                        Cash
                    </option>

                    <option value="GCash">
                        GCash
                    </option>

                </select>


                <label>Additional instructions</label>

                <textarea
                id="notes"
                rows="3"
                placeholder="Optional message..."></textarea>


                <button type="submit">
                    SUBMIT ORDER REQUEST
                </button>

            </form>

            <p class="notice">
                We'll confirm availability and your order
                details before preparing your bag.
            </p>

        </div>

    </div>

</section>


<!-- FOOTER -->

<footer>

    <strong>REL ATELIER</strong>

    <p>
        Timeless bags, thoughtfully chosen.
    </p>

    <p>
        © 2026 REL Atelier. All rights reserved.
    </p>

</footer>


<!-- JAVASCRIPT -->

<script>

// PRODUCT DATABASE

const products = [

    {
        name: "The Élise Top Handle",
        price: 100000
    },

    {
        name: "The Margot Shoulder Bag",
        price: 99000
    },

    {
        name: "The Noelle Mini Bag",
        price: 125000
    },

    {
        name: "The Celeste Tote",
        price: 150000
    }

];


// SHOPPING CART

let cart = [];


// ADD TO CART

function addToCart(index) {

    const product = products[index];

    const existing = cart.find(
        item => item.name === product.name
    );

    if (existing) {

        existing.quantity++;

    } else {

        cart.push({
            ...product,
            quantity: 1
        });

    }

    updateCart();

    alert(product.name + " added to your bag!");

}


// REMOVE PRODUCT

function removeFromCart(index) {

    cart.splice(index, 1);

    updateCart();

}


// UPDATE CART DISPLAY

function updateCart() {

    const cartItems =
    document.getElementById("cart-items");

    const count =
    document.getElementById("cart-count");

    const total =
    document.getElementById("total-price");

    let totalAmount = 0;

    let totalItems = 0;

    if (cart.length === 0) {

        cartItems.innerHTML =
        `<p class="empty">
        Your selection is empty.
        Explore the collection to find your bag.
        </p>`;

    } else {

        cartItems.innerHTML = "";

        cart.forEach((item, index) => {

            const subtotal =
            item.price * item.quantity;

            totalAmount += subtotal;

            totalItems += item.quantity;

            cartItems.innerHTML += `

                <div class="cart-item">

                    <div>
                        <strong>${item.name}</strong>
                        <p>
                        ₱${item.price.toLocaleString()}
                        × ${item.quantity}
                        </p>
                    </div>

                    <div>
                        <strong>
                        ₱${subtotal.toLocaleString()}
                        </strong>

                        <button class="remove-btn"
                        onclick="removeFromCart(${index})">
                            Remove
                        </button>
                    </div>

                </div>

            `;

        });

    }

    count.textContent = totalItems;

    total.textContent =
    "₱" + totalAmount.toLocaleString(
        "en-PH",
        {
            minimumFractionDigits: 2
        }
    );

}


// GO TO ORDER

function goToOrder() {

    document.getElementById("order")
    .scrollIntoView({
        behavior: "smooth"
    });

}


// SUBMIT ORDER

document.getElementById("order-form")
.addEventListener("submit", function(event) {

    event.preventDefault();

    if (cart.length === 0) {

        alert("Please add a bag to your cart first!");

        return;

    }

    const name =
    document.getElementById("customer-name").value;

    const phone =
    document.getElementById("customer-phone").value;

    const email =
    document.getElementById("customer-email").value;

    const delivery =
    document.getElementById("delivery").value;

    const payment =
    document.getElementById("payment").value;

    const notes =
    document.getElementById("notes").value;

    const total = cart.reduce(
        (sum, item) =>
        sum + item.price * item.quantity,
        0
    );

    let summary = cart.map(item =>
        `${item.name} x ${item.quantity}`
    ).join("\n");

    alert(

        "REL ATELIER ORDER REQUEST\n\n" +

        "Customer: " + name + "\n" +

        "Mobile: " + phone + "\n" +

        "Email: " + email + "\n\n" +

        "Selected bags:\n" + summary + "\n\n" +

        "Total: ₱" + total.toLocaleString() + "\n" +

        "Receiving method: " + delivery + "\n" +

        "Payment: " + payment + "\n" +

        "Instructions: " + notes + "\n\n" +

        "Your order request has been recorded in this demo. " +
        "Please contact the store to confirm your order."

    );

    // Reset after submission

    cart = [];

    updateCart();

    this.reset();

});

</script>

</body>
</html>
