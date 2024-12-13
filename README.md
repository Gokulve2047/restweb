# Ex.07 Restaurant Website
## Date:13-12-2024

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```
home.html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>East Blue | Home</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            font-family: 'Roboto', sans-serif;
            color: #f5f5f5;
            background: #121212;
            line-height: 1.6;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: #1f1f1f;
            color: #f5f5f5;
            padding: 15px 20px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        header img {
            height: 50px;
        }

        header nav {
            display: flex;
            gap: 20px;
        }

        header nav a {
            text-decoration: none;
            color: #f5f5f5;
            font-weight: 500;
            font-size: 1rem;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #ff9800;
        }

        .banner {
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 40px 20px;
            background: linear-gradient(135deg, #1c1c1c, #292929), url('banner-placeholder.jpg') no-repeat center center/cover;
            color: #f5f5f5;
            height: 300px;
            text-shadow: 0 4px 8px rgba(0, 0, 0, 0.7);
            text-align: center;
        }

        .banner-content {
            background: rgba(0, 0, 0, 0.6);
            padding: 25px 40px;
            border-radius: 10px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.5);
        }

        .banner-content h1 {
            font-family: 'Playfair Display', serif;
            font-size: 3rem;
            margin-bottom: 15px;
            color: #0e63a3;
        }

        .banner-content p {
            font-size: 1.2rem;
            margin-bottom: 20px;
            color: #f5f5f5;
        }

        .banner-content a {
            background: #0779a5;
            color: #121212;
            padding: 12px 25px;
            text-decoration: none;
            font-weight: bold;
            border-radius: 50px;
            transition: background 0.3s ease, transform 0.3s ease;
        }

        .banner-content a:hover {
            background: #0797b7;
            transform: translateY(-5px);
        }

        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            padding: 40px 20px;
            background: #1f1f1f;
        }

        .feature {
            background: #292929;
            border-radius: 15px;
            padding: 20px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.4);
            text-align: center;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .feature:hover {
            transform: translateY(-10px);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.6);
        }

        .feature img {
            width: 100%;
            border-radius: 15px;
            margin-bottom: 15px;
        }

        .feature h3 {
            font-size: 1.4rem;
            margin-bottom: 10px;
            color: #1086b9;
            font-family: 'Playfair Display', serif;
        }

        .feature p {
            font-size: 1rem;
            color: #cccccc;
        }

        footer {
            background: #121212;
            color: #999;
            text-align: center;
            padding: 20px;
            margin-top: 40px;
        }

        footer a {
            color: #0f85bc;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s ease;
        }

        footer a:hover {
            color: #f5f5f5;
        }

        @media (max-width: 768px) {
            header nav {
                flex-direction: column;
                align-items: center;
                gap: 10px;
            }

            .banner {
                height: auto;
                padding: 30px 15px;
            }

            .banner-content h1 {
                font-size: 2.5rem;
            }

            .banner-content p {
                font-size: 1rem;
            }
        }

        @media (max-width: 480px) {
            .banner-content h1 {
                font-size: 2rem;
            }

            .banner-content p {
                font-size: 0.9rem;
            }

            .banner-content a {
                padding: 10px 20px;
                font-size: 0.9rem;
            }
        }
    </style>
</head>

<body>
    <header>
        <img src="logo.jpg" alt="EAST BLUE Logo">
        <nav>
            <a href="home.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="contact.html">Contact</a>
            <a href="admin.html">Admin</a>
        </nav>
    </header>

    <div class="banner">
        <div class="banner-content">
            <h1>EAST BLUE</h1>
        </div>
    </div>

    <section id="features" class="features">
        <div class="feature">
            <img src="home page.jpg" alt="High quality dishes">
            <h3>High Quality Dishes</h3>
            <p>Indulge in the finest and freshest meals crafted with love and expertise.</p>
        </div>
    </section>
    <footer>
        <p>&copy; 2024 EAST BLUE. All rights reserved. | <a href="#">Privacy Policy</a></p>
    </footer>
</body>

</html>

menu.html

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>EAST BLUE - Menu</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            font-family: 'Poppins', sans-serif;
            color: #fff;
            background: #1c1c1c;
            line-height: 1.6;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: linear-gradient(135deg, #3f2b96, #a8c0ff);
            color: white;
            padding: 15px 20px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        header h1 {
            font-size: 2rem;
            font-family: 'Playfair Display', serif;
            color: #f4f4f4;
        }

        header nav a {
            text-decoration: none;
            color: #f4f4f4;
            font-weight: 600;
            margin: 0 15px;
            transition: color 0.3s ease;
            font-size: 1rem;
        }

        header nav a:hover {
            color: #0762a8;
        }

        .menu-container {
            padding: 50px 20px;
            background: #282828;
            text-align: center;
        }

        .menu-container h1 {
            font-size: 3rem;
            color: #0773a9;
            margin-bottom: 30px;
            font-family: 'Playfair Display', serif;
        }

        .menu-items {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            justify-content: center;
        }

        .menu-item {
            background: #333;
            border-radius: 15px;
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.4);
            width: 280px;
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            text-align: left;
        }

        .menu-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-bottom: 3px solid #036db4;
            transition: transform 0.3s ease;
        }

        .menu-item:hover {
            transform: scale(1.05);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.5);
        }

        .menu-item:hover img {
            transform: scale(1.1);
        }

        .menu-details {
            padding: 15px;
        }

        .menu-details h3 {
            font-size: 1.6rem;
            color: #1a8cd3;
            margin-bottom: 10px;
            font-weight: 600;
        }

        .menu-details p {
            font-size: 1rem;
            color: #ddd;
            margin-bottom: 10px;
        }

        .menu-details .price {
            font-weight: bold;
            font-size: 1.2rem;
            color: #ff4500;
        }

        footer {
            background: #3f2b96;
            color: white;
            text-align: center;
            padding: 15px 0;
        }

        footer a {
            color: #1b8fc9;
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s ease;
        }

        footer a:hover {
            color: #f4f4f4;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 1.5rem;
            }

            .menu-items {
                flex-direction: column;
                gap: 20px;
            }

            .menu-item {
                width: 100%;
            }

            header nav a {
                font-size: 0.9rem;
                margin: 0 10px;
            }
        }
    </style>
</head>

<body>

    <header>
        <h1>EAST BLUE</h1>
        <nav>
            <a href="home.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="contact.html">Contact</a>
            <a href="admin.html">Administration</a>
        </nav>
    </header>

    <div class="menu-container">
        <h1>Menu</h1>
        <div class="menu-items">
            <div class="menu-item">
                <img src="crab.jpg" alt="Classic Briyani">
                <div class="menu-details">
                    <h3>Crab</h3>
                    <p class="price">₹600/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="fish fry.jpg" alt="Burger">
                <div class="menu-details">
                    <h3>Fish Fry</h3>
                    <p class="price">₹250/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="grilled fish.avif" alt="Orange Cocktail">
                <div class="menu-details">
                    <h3>Grilled Fish</h3>
                    <p class="price">₹300/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="lapster.jpg" alt="Royal Falooda">
                <div class="menu-details">
                    <h3>Lapster</h3>
                    <p class="price">₹800/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="prawn.webp" alt="Parotta">
                <div class="menu-details">
                    <h3>Prawn</h3>
                    <p class="price">₹320/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="squid grill.jpg" alt="Pasta">
                <div class="menu-details">
                    <h3>Squid Grill</h3>
                    <p class="price">₹420/-</p>
                </div>
            </div>
        </div>
    </div>

    <footer>
        <p>&copy; 2024 EAST BLUE. All rights reserved. | <a href="home.html">Back to Home</a></p>
    </footer>

</body>

</html>

contact.html

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>EAST BLUE - Menu</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            font-family: 'Poppins', sans-serif;
            color: #fff;
            background: #1c1c1c;
            line-height: 1.6;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: linear-gradient(135deg, #3f2b96, #a8c0ff);
            color: white;
            padding: 15px 20px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        header h1 {
            font-size: 2rem;
            font-family: 'Playfair Display', serif;
            color: #f4f4f4;
        }

        header nav a {
            text-decoration: none;
            color: #f4f4f4;
            font-weight: 600;
            margin: 0 15px;
            transition: color 0.3s ease;
            font-size: 1rem;
        }

        header nav a:hover {
            color: #0762a8;
        }

        .menu-container {
            padding: 50px 20px;
            background: #282828;
            text-align: center;
        }

        .menu-container h1 {
            font-size: 3rem;
            color: #0773a9;
            margin-bottom: 30px;
            font-family: 'Playfair Display', serif;
        }

        .menu-items {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            justify-content: center;
        }

        .menu-item {
            background: #333;
            border-radius: 15px;
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.4);
            width: 280px;
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            text-align: left;
        }

        .menu-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-bottom: 3px solid #036db4;
            transition: transform 0.3s ease;
        }

        .menu-item:hover {
            transform: scale(1.05);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.5);
        }

        .menu-item:hover img {
            transform: scale(1.1);
        }

        .menu-details {
            padding: 15px;
        }

        .menu-details h3 {
            font-size: 1.6rem;
            color: #1a8cd3;
            margin-bottom: 10px;
            font-weight: 600;
        }

        .menu-details p {
            font-size: 1rem;
            color: #ddd;
            margin-bottom: 10px;
        }

        .menu-details .price {
            font-weight: bold;
            font-size: 1.2rem;
            color: #ff4500;
        }

        footer {
            background: #3f2b96;
            color: white;
            text-align: center;
            padding: 15px 0;
        }

        footer a {
            color: #1b8fc9;
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s ease;
        }

        footer a:hover {
            color: #f4f4f4;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 1.5rem;
            }

            .menu-items {
                flex-direction: column;
                gap: 20px;
            }

            .menu-item {
                width: 100%;
            }

            header nav a {
                font-size: 0.9rem;
                margin: 0 10px;
            }
        }
    </style>
</head>

<body>

    <header>
        <h1>EAST BLUE</h1>
        <nav>
            <a href="home.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="contact.html">Contact</a>
            <a href="admin.html">Administration</a>
        </nav>
    </header>

    <div class="menu-container">
        <h1>Menu</h1>
        <div class="menu-items">
            <div class="menu-item">
                <img src="crab.jpg" alt="Classic Briyani">
                <div class="menu-details">
                    <h3>Crab</h3>
                    <p class="price">₹600/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="fish fry.jpg" alt="Burger">
                <div class="menu-details">
                    <h3>Fish Fry</h3>
                    <p class="price">₹250/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="grilled fish.avif" alt="Orange Cocktail">
                <div class="menu-details">
                    <h3>Grilled Fish</h3>
                    <p class="price">₹300/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="lapster.jpg" alt="Royal Falooda">
                <div class="menu-details">
                    <h3>Lapster</h3>
                    <p class="price">₹800/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="prawn.webp" alt="Parotta">
                <div class="menu-details">
                    <h3>Prawn</h3>
                    <p class="price">₹320/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="squid grill.jpg" alt="Pasta">
                <div class="menu-details">
                    <h3>Squid Grill</h3>
                    <p class="price">₹420/-</p>
                </div>
            </div>
        </div>
    </div>

    <footer>
        <p>&copy; 2024 EAST BLUE. All rights reserved. | <a href="home.html">Back to Home</a></p>
    </footer>

</body>

</html>

admin.html

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>EAST BLUE - Administration</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            font-family: 'Poppins', sans-serif;
            color: #fff;
            background-color: #1e1e2f;
            line-height: 1.6;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: linear-gradient(135deg, #0d0d0e, #2575fc);
            padding: 15px 20px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
        }

        header h1 {
            font-size: 2rem;
            font-family: 'Playfair Display', serif;
            color: #076ab1;
        }

        header nav a {
            text-decoration: none;
            color: white;
            font-weight: 600;
            margin: 0 15px;
            font-size: 1rem;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #07090a;
        }

        .admin-container {
            padding: 50px 20px;
            text-align: center;
        }

        .admin-container h1 {
            font-size: 2.8rem;
            color: #0b5aaa;
            margin-bottom: 40px;
            font-family: 'Playfair Display', serif;
        }

        .admin-items {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            justify-content: center;
        }

        .admin-item {
            background: #282845;
            border-radius: 15px;
            box-shadow: 0 6px 10px rgba(0, 0, 0, 0.3);
            width: 280px;
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            text-align: left;
        }

        .admin-item img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            border-bottom: 5px solid #1163b0;
        }

        .admin-item:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 15px rgba(0, 0, 0, 0.5);
        }

        .admin-details {
            padding: 20px;
        }

        .admin-details h3 {
            font-size: 1.5rem;
            color: #0b80b2;
            margin-bottom: 10px;
            font-family: 'Playfair Display', serif;
        }

        .admin-details p {
            font-size: 1rem;
            color: #d3d3e7;
        }

        footer {
            background: linear-gradient(135deg, #0e0e0f, #2575fc);
            color: white;
            text-align: center;
            padding: 20px 0;
        }

        footer a {
            color: #0a8fb4;
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s ease;
        }

        footer a:hover {
            color: #66ccff;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 1.5rem;
            }

            .admin-items {
                flex-direction: column;
                gap: 20px;
            }

            .admin-item {
                width: 100%;
            }

            header nav a {
                font-size: 0.9rem;
                margin: 0 5px;
            }

            .admin-container h1 {
                font-size: 2.2rem;
            }
        }
    </style>
</head>

<body>

    <header>
        <h1>EAST BLUE</h1>
        <nav>
            <a href="home.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="contact.html">Contact</a>
            <a href="admin.html">Administration</a>
        </nav>
    </header>

    <div class="admin-container">
        <h1>Meet Our Leadership Team</h1>
        <div class="admin-items">
            <div class="admin-item">
                <img src="WhatsApp Image 2024-12-13 at 10.41.39 PM.jpeg" alt="CEO">
                <div class="admin-details">
                    <h3>Gokul</h3>
                    <p>CEO of EAST BLUE</p>
                </div>
            </div>

            <div class="admin-item">
                <img src="manager.jpg" alt="Manager">
                <div class="admin-details">
                    <h3>VIJAY</h3>
                    <p>Manager</p>
                </div>
            </div>

            <div class="admin-item">
                <img src="sanji cheff.webp" alt="Master Chef">
                <div class="admin-details">
                    <h3>sANJI</h3>
                    <p>Master Chef</p>
                </div>
            </div>

            <div class="admin-item">
                <img src="ass manager.avif" alt="Assistant Managing Director">
                <div class="admin-details">
                    <h3>Rasmika</h3>
                    <p>Assistant Managing Director</p>
                </div>
            </div>
        </div>
    </div>

    <footer>
        <p>&copy; 2024 EAST BLUE. All rights reserved. | <a href="home.html">Back to Home</a></p>
    </footer>

</body>

</html>

```


## OUTPUT:
![alt text](<Screenshot (1).png>)
![alt text](<Screenshot (4).png>)
![alt text](<Screenshot (5).png>)
![alt text](<Screenshot (6).png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
