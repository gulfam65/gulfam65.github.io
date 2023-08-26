<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>SSAS Public School</title>
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="/">Home</a></li>
                <li><a href="/about">About</a></li>
                <li><a href="/gallery">Gallery</a></li>
                <li><a href="/contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="home">
            <h1>Welcome to SSAS Public School</h1>
            <p>Admission Open</p>
        </section>
    </main>

    <footer>
        <p>&copy; 2023 SSAS Public School</p>
    </footer>

    <script>
        // JavaScript to update URLs without ".html" extension
        document.addEventListener("DOMContentLoaded", function () {
            const links = document.querySelectorAll("nav a");
            for (const link of links) {
                link.addEventListener("click", function (event) {
                    event.preventDefault();
                    const href = this.getAttribute("href");
                    history.pushState({}, "", href);
                });
            }
        });
    </script>
</body>
</html>
