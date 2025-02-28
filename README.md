# Health-website-
# Creating the website project files

import zipfile



# File contents

index_html = """<!DOCTYPE html>

<html lang="en">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Healthy Living</title>

    <link rel="stylesheet" href="style.css">

</head>

<body>

    <header>

        <img src="logo.png" alt="Healthy Living Logo" class="logo">

        <h1>Welcome to Healthy Living</h1>

        <p>Your guide to balanced diets, weight management, and nutrition.</p>

    </header>

    <nav>

        <ul>

            <li><a href="#">Home</a></li>

            <li><a href="#">Nutrition Basics</a></li>

            <li><a href="#">Weight Management</a></li>

            <li><a href="#">Healthy Foods</a></li>

            <li><a href="#">Contact</a></li>

        </ul>

    </nav>

    <main>

        <section>

            <h2>Why a Balanced Diet Matters</h2>

            <p>Eating a balanced diet is crucial for maintaining good health and well-being. It provides essential nutrients your body needs to function properly.</p>

        </section>

    </main>

    <footer>

        <p>&copy; 2025 Healthy Living. All rights reserved.</p>

    </footer>

</body>

</html>

"""



style_css = """body {

    font-family: Arial, sans-serif;

    margin: 0;

    padding: 0;

    background-color: #f4f4f4;

    color: #333;

}

header {

    background: #2c7a7b;

    color: white;

    text-align: center;

    padding: 20px;

}

.logo {

    width: 100px;

    height: auto;

}

nav ul {

    list-style: none;

    padding: 0;

    text-align: center;

    background: #1e5555;

}

nav ul li {

    display: inline;

    margin: 0 15px;

}

nav ul li a {

    color: white;

    text-decoration: none;

}

main {

    padding: 20px;

}

footer {

    text-align: center;

    padding: 10px;

    background: #2c7a7b;

    color: white;

    margin-top: 20px;

}

"""



script_js = """document.addEventListener("DOMContentLoaded", function() {

    console.log("Website loaded successfully!");

});

"""



# Creating the ZIP file

zip_path = "/mnt/data/health_website.zip"

with zipfile.ZipFile(zip_path, 'w') as zipf:

    zipf.writestr("index.html", index_html)

    zipf.writestr("style.css", style_css)

    zipf.writestr("script.js", script_js)



zip_path
git add .
