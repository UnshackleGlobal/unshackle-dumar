<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Unshackle Dumar</title>
    <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f7f7f7;
            color: #333;
        }

        .navbar {
            background-color: #f2f2f2;
            z-index: 1000;
        }

        .navbar-brand, .navbar-nav .nav-link {
            color: #333;
            font-weight: 700;
        }

        .navbar-nav .nav-link {
            margin-right: 1rem;
            color: #333;
        }

        .navbar-nav .btn-primary {
            background-color: #aeb093;
            border-color: #aeb093;
            color: #fff;
            margin-left: 1rem;
        }

        main {
            display: flex;
            align-items: flex-start;
            justify-content: space-between;
            padding: 20px;
            background-color: #fff;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            margin: 20px auto;
            max-width: 800px;
        }

        .logo-container {
            display: flex;
            align-items: center;
        }

        .logo {
            max-width: 200px;
            height: auto;
            margin-right: 20px;
        }

        .main-content {
            flex: 1;
        }

        .section-box {
            background-color: #f2f2f2;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            margin-bottom: 20px;
        }

        footer {
            background-color: #aeb093;
            color: #fff;
            margin-top: 20px;
            padding: 20px 0;
            text-align: center;
        }

        footer a {
            color: #fff;
            text-decoration: none;
        }

        footer a:hover {
            text-decoration: underline;
        }

        footer p {
            color: #ccc;
        }

        .container h2, .container h3 {
            color: #333;
        }

        .container p {
            color: #666;
        }
    </style>
</head>
<body>

    <nav class="navbar navbar-expand-lg">
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav ml-auto">
                <li class="nav-item"><a class="nav-link" href="#" id="home-link">Home</a></li>
                <li class="nav-item"><a class="nav-link" href="#" id="about-link">About Us</a></li>
                <li class="nav-item"><a class="nav-link" href="#" id="contact-link">Contact Us</a></li>
            </ul>
        </div>
    </nav>

    <main id="home-section">
        <div class="logo-container">
            <img src="unshackle logo.png" alt="Unshackle Dumar Logo" class="logo">
        </div>
        <div class="main-content">
            <div class="section-box">
                <h2>Welcome to Unshackle Dumar</h2>
                <p>Where we empower BAME women through education, health, and community development.</p>
                <p>Together, we strive to create positive change, uplift communities, and foster opportunities for growth and empowerment. Join us on our journey to make a lasting impact and build a brighter future for all.</p>
            </div>
        </div>
    </main>

    <main id="about-us" style="display: none;">
        <div class="logo-container">
            <img src="unshackle logo.png" alt="Unshackle Dumar Logo" class="logo">
        </div>
        <div class="main-content">
            <div class="section-box">
                <h2>About Us</h2>
                <p>Unshackle Dumar is committed to empowering women and girls through community projects, education, and advocacy.</p>
                <h3>Our Aims and Objectives</h3>
                <ul>
                    <li><strong>Empowerment and Well-being:</strong> We promote the well-being of women and girls through education, training, and support.</li>
                    <li><strong>Social Inclusion:</strong> We aim to include women and girls from diverse backgrounds in our community projects.</li>
                    <li><strong>Elimination of Harmful Practices:</strong> We work to eliminate harmful practices like Female Genital Mutilation (FGM) and violence against women.</li>
                </ul>
            </div>
        </div>
    </main>

    <main id="contact-us" style="display: none;">
        <div class="logo-container">
            <img src="unshackle logo.png" alt="Unshackle Dumar Logo" class="logo">
        </div>
        <div class="main-content">
            <div class="section-box">
                <h2>Contact Us</h2>
                <p>Email: unshackledumar2@gmail.com</p>
            </div>
        </div>
    </main>

    <footer class="text-center py-3">
        <div class="container">
            <p>&copy; 2024 Unshackle Dumar. All rights reserved.</p>
            <div>
                <a href="#">Privacy Policy</a> |
                <a href="#">Terms of Service</a>
            </div>
        </div>
    </footer>

    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.4/dist/umd/popper.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const homeSection = document.getElementById('home-section');
            const aboutUs = document.getElementById('about-us');
            const contactUs = document.getElementById('contact-us');

            // Initially show the home section
            homeSection.style.display = 'flex';
            aboutUs.style.display = 'none';
            contactUs.style.display = 'none';

            // Event listeners for navigation links
            document.getElementById('home-link').addEventListener('click', function(event) {
                event.preventDefault();
                homeSection.style.display = 'flex';
                aboutUs.style.display = 'none';
                contactUs.style.display = 'none';
            });

            document.getElementById('about-link').addEventListener('click', function(event) {
                event.preventDefault();
                homeSection.style.display = 'none';
                aboutUs.style.display = 'flex';
                contactUs.style.display = 'none';
            });

            document.getElementById('contact-link').addEventListener('click', function(event) {
                event.preventDefault();
                homeSection.style.display = 'none';
                aboutUs.style.display = 'none';
                contactUs.style.display = 'flex';
            });
        });
    </script>
</body>
</html>


