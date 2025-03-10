# dd
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Event Management</title>
    <link rel="stylesheet" href="styles.css">
    <script src="script.js" defer></script>
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #1e1e2f;
            color: #f8f9fa;
            text-align: center;
            margin: 0;
            padding: 0;
        }
        header {
            background: #4a148c;
            color: white;
            padding: 15px 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }
        nav ul {
            list-style: none;
            padding: 0;
            display: flex;
            justify-content: center;
        }
        nav ul li {
            margin: 0 20px;
        }
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            font-size: 18px;
            cursor: pointer;
        }
        .hero {
            background: linear-gradient(135deg, #6a11cb, #2575fc);
            color: white;
            padding: 100px 20px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.6);
            margin-top: 70px;
        }
        .hero h2 {
            font-size: 42px;
        }
        .hero p {
            font-size: 20px;
            max-width: 600px;
            margin: auto;
        }
        .btn-primary {
            background: #ff9800;
            color: white;
            padding: 12px 24px;
            border: none;
            border-radius: 5px;
            font-size: 18px;
            cursor: pointer;
            transition: 0.3s;
            margin-top: 20px;
        }
        .btn-primary:hover {
            background: #e68900;
        }
        .event-list {
            padding: 50px;
            background: #29294d;
        }
        .event {
            background: #3c3c6e;
            padding: 20px;
            margin: 15px;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.3);
            border-radius: 8px;
            transition: 0.3s;
            color: white;
        }
        .event:hover {
            transform: scale(1.05);
        }
        .event img {
            width: 100%;
            border-radius: 8px;
        }
        footer {
            background: #4a148c;
            color: white;
            padding: 15px;
            margin-top: 30px;
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#home" onclick="scrollToSection('home')">Home</a></li>
                <li><a href="#events" onclick="scrollToSection('events')">Events</a></li>
                <li><a href="#payment" onclick="window.location.href='payment.html'">Payment</a></li>
                <li><a href="#contact" onclick="scrollToSection('contact')">Contact</a></li>
            </ul>
        </nav>
    </header>
    
    <section id="home" class="hero">
        <h2>Unforgettable Events Await You!</h2>
        <p>Experience the best event setups with premium services for up to 16 guests, starting at ₹45,000.</p>
        <button class="btn-primary" onclick="scrollToSection('events')">Explore Now</button>
    </section>
    
    <section id="events" class="event-list">
        <h2>Upcoming Events</h2>
        <div class="event">
            <img src="pool-party.jpg" alt="Pool Party">
            <h3>Pool Party</h3>
            <p>Enjoy a luxurious poolside experience with music, drinks, and fun.</p>
        </div>
        <div class="event">
            <img src="fun-party.jpg" alt="Fun Party">
            <h3>Fun Party</h3>
            <p>Experience thrilling games, interactive activities, and non-stop entertainment.</p>
        </div>
    </section>
    
    <footer>
        <p>&copy; 2024 Event Management | Designed for a Premium Experience</p>
    </footer>

    <script>
        function scrollToSection(id) {
            document.getElementById(id).scrollIntoView({
                behavior: 'smooth'
            });
        }
    </script>
</body>
</html>
