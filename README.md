<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image and PDF Tools - ToolHub</title>
    <meta name="description" content="A collection of free online tools for image and PDF manipulation.">
    <meta name="keywords" content="image tools, pdf tools, online tools, free tools">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
    <style>
        /* Basic Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            background-color: #f5f5f5;
            color: #333;
        }

        /* Header Styles */
        header {
            background-color: #003366;
            color: #FFF;
            padding: 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }

        .logo {
            font-size: 1.5em;
            font-weight: bold;
        }

        nav ul {
            list-style: none;
            display: flex;
        }

        nav ul li {
            margin-left: 20px;
        }

        nav ul li a {
            color: #FFF;
            text-decoration: none;
        }

        nav ul li a:hover {
            text-decoration: underline;
        }

        /* Hero Section with Slider */
        .hero {
            margin-top: 60px;
        }

        .slider {
            position: relative;
            overflow: hidden;
            height: 400px;
        }

        .slide {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            background-color: #E0F7FA;
            opacity: 0;
            transition: opacity 0.5s;
        }

        .slide.active {
            opacity: 1;
        }

        .slide img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .slide h2 {
            margin: 10px 0;
        }

        .slide p {
            margin-bottom: 20px;
        }

        .btn {
            background-color: #007BFF;
            color: #FFF;
            padding: 10px 20px;
            text-decoration: none;
            border-radius: 5px;
        }

        .btn:hover {
            background-color: #0056b3;
        }

        /* Search Section */
        .search {
            text-align: center;
            margin: 20px 0;
        }

        #searchInput {
            width: 50%;
            padding: 10px;
            font-size: 1em;
        }

        /* Tools Section */
        .tools {
            padding: 20px;
        }

        .tool-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
        }

        .tool-card {
            background-color: #FFF;
            border: 1px solid #E0F7FA;
            padding: 20px;
            text-align: center;
            transition: transform 0.3s;
        }

        .tool-card:hover {
            transform: translateY(-5px);
        }

        .tool-card i {
            font-size: 2em;
            color: #007BFF;
            margin-bottom: 10px;
        }

        .tool-card h3 {
            margin: 10px 0;
        }

        .tool-card p {
            font-size: 0.9em;
        }

        /* Testimonials Section */
        .testimonials {
            padding: 20px;
            background-color: #f9f9f9;
        }

        .testimonial {
            margin: 20px 0;
            text-align: center;
        }

        /* Footer Styles */
        footer {
            background-color: #003366;
            color: #FFF;
            text-align: center;
            padding: 20px;
        }

        .social-media a {
            color: #FFF;
            margin: 0 10px;
            font-size: 1.5em;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            nav ul {
                flex-direction: column;
            }

            nav ul li {
                margin: 10px 0;
            }

            .slider {
                height: 300px;
            }

            .slide img {
                height: 150px;
            }

            #searchInput {
                width: 80%;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">ToolHub</div>
        <nav>
            <ul>
                <li><a href="#">Image Tools</a></li>
                <li><a href="#">PDF Tools</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section class="hero">
            <div class="slider">
               <div class="slide active">
                  <img src="image-compressor.jpg" alt="Image Compressor">
                  <h2>Image Compressor</h2>
                  <p>Reduce image size without losing quality.</p>
                  <a href="/tools/image-compressor" class="btn">Use Tool</a>
              </div>
                <div class="slide">
                    <img src="pdf-merger.jpg" alt="PDF Merger">
                    <h2>PDF Merger</h2>
                    <p>Combine multiple PDFs into one.</p>
                    <a href="#" class="btn">tool/img-compress.html</a>
                </div>
                <div class="slide">
                    <img src="image-to-pdf.jpg" alt="Image to PDF">
                    <h2>Image to PDF</h2>
                    <p>Convert images to PDF documents.</p>
                    <a href="#" class="btn">Use Tool</a>
                </div>
            </div>
        </section>
        <section class="search">
            <input type="text" id="searchInput" placeholder="Search for a tool...">
        </section>
        <section class="tools">
            <h2>All Tools</h2>
            <div class="tool-grid">
                <div class="tool-card">
                    <i class="fas fa-compress"></i>
                    <h3>Image Compressor</h3>
                    <p>Reduce image size without losing quality.</p>
                </div>
                <div class="tool-card">
                    <i class="fas fa-expand"></i>
                    <h3>Image Resizer</h3>
                    <p>Change image dimensions easily.</p>
                </div>
                <div class="tool-card">
                    <i class="fas fa-exchange-alt"></i>
                    <h3>Image Converter</h3>
                    <p>Convert images to different formats.</p>
                </div>
                <div class="tool-card">
                    <i class="fas fa-file-pdf"></i>
                    <h3>PDF Merger</h3>
                    <p>Combine multiple PDFs into one.</p>
                </div>
                <div class="tool-card">
                    <i class="fas fa-cut"></i>
                    <h3>PDF Splitter</h3>
                    <p>Split PDFs into individual pages.</p>
                </div>
                <div class="tool-card">
                    <i class="fas fa-file-word"></i>
                    <h3>PDF to Word</h3>
                    <p>Convert PDFs to editable Word documents.</p>
                </div>
            </div>
        </section>
        <section class="testimonials">
            <h2>What Our Users Say</h2>
            <div class="testimonial">
                <p>"ToolHub has saved me so much time with its easy-to-use tools!"</p>
                <p>- Jane Doe</p>
            </div>
            <div class="testimonial">
                <p>"The image compressor is fantastic! Highly recommend."</p>
                <p>- John Smith</p>
            </div>
        </section>
    </main>
    <footer>
        <p>&copy; 2023 ToolHub. All rights reserved.</p>
        <div class="social-media">
            <a href="#"><i class="fab fa-facebook"></i></a>
            <a href="#"><i class="fab fa-twitter"></i></a>
            <a href="#"><i class="fab fa-instagram"></i></a>
        </div>
    </footer>
    <script>
        // Slider Functionality
        const slides = document.querySelectorAll('.slide');
        let currentSlide = 0;

        function showSlide(index) {
            slides.forEach((slide, i) => {
                slide.classList.remove('active');
                if (i === index) {
                    slide.classList.add('active');
                }
            });
        }

        function nextSlide() {
            currentSlide = (currentSlide + 1) % slides.length;
            showSlide(currentSlide);
        }

        setInterval(nextSlide, 5000); // Change slide every 5 seconds
        showSlide(currentSlide);

        // Search Functionality
        const searchInput = document.getElementById('searchInput');
        const toolCards = document.querySelectorAll('.tool-card');

        searchInput.addEventListener('input', function() {
            const searchTerm = searchInput.value.toLowerCase();
            toolCards.forEach(card => {
                const title = card.querySelector('h3').textContent.toLowerCase();
                if (title.includes(searchTerm)) {
                    card.style.display = 'block';
                } else {
                    card.style.display = 'none';
                }
            });
        });
    </script>
</body>
</html>
