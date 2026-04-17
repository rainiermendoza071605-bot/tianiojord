        <!DOCTYPE html>
        <html lang="en">
        <head>
            <meta charset="UTF-8">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
            <title>Jordan Tianio | Portfolio</title>
            <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
            <style>
                /* CSS Variables for easy color management */
                :root {
                    --primary-bg: #87ceeb; /* Sky blue gradient top */
                    --secondary-bg: #fdfd96; /* Pale yellow gradient bottom */
                    --dark-blue: #1a5276;
                    --text-color: #333;
                    --white: #ffffff;
                }

                * {
                    margin: 0;
                    padding: 0;
                    box-sizing: border-box;
                    font-family: 'Poppins', sans-serif;
                }

                body {
                    background: linear-gradient(to bottom, var(--primary-bg), var(--secondary-bg));
                    color: var(--text-color);
                    line-height: 1.6;
                    min-height: 100vh;
                }

                /* Navigation */
                nav {
                    display: flex;
                    justify-content: space-between;
                    align-items: center;
                    padding: 1rem 5%;
                    background: rgba(255, 255, 255, 0.2);
                    backdrop-filter: blur(5px);
                    position: sticky;
                    top: 0;
                    z-index: 1000;
                }

                .logo { font-weight: 600; font-size: 1.5rem; color: var(--dark-blue); }

                nav ul { display: flex; list-style: none; align-items: center; }
                nav ul li { margin-left: 20px; position: relative; }
                nav ul li a { 
                    text-decoration: none; 
                    color: var(--dark-blue); 
                    font-weight: 400;
                    transition: 0.3s;
                }

                /* --- ADDED SEARCH CSS --- */
                .search-container {
                    display: flex;
                    align-items: center;
                    background: rgba(255, 255, 255, 0.4);
                    padding: 5px 10px;
                    border-radius: 20px;
                    margin-left: 15px;
                    border: 1px solid var(--dark-blue);
                }
                #searchInput {
                    border: none;
                    background: transparent;
                    outline: none;
                    padding: 2px 5px;
                    width: 100px;
                    font-size: 0.8rem;
                    transition: width 0.4s;
                }
                #searchInput:focus { width: 150px; }
                #searchBtn {
                    background: transparent;
                    border: none;
                    cursor: pointer;
                    color: var(--dark-blue);
                    font-size: 1rem;
                }
                /* Highlight effect for found sections */
                .search-highlight {
                    animation: highlightFade 3s ease-in-out;
                }
                @keyframes highlightFade {
                    0% { background-color: rgba(255, 255, 0, 0.5); transform: scale(1.02); }
                    100% { background-color: transparent; transform: scale(1); }
                }
                /* ------------------------ */

                /* Dropdown Logic */
                .dropdown-content {
                    display: none;
                    position: absolute;
                    background: var(--white);
                    min-width: 120px;
                    box-shadow: 0px 8px 16px rgba(0,0,0,0.1);
                    top: 100%;
                }
                .dropdown:hover .dropdown-content { display: block; }
                .dropdown-content a { color: black; padding: 10px; display: block; font-size: 0.9rem;}

                /* Hero Section */
                .section { padding: 80px 10%; text-align: center; }
                h1 { font-size: 3.5rem; margin-bottom: 40px; color: var(--dark-blue); }

                .profile-container {
                    display: flex;
                    align-items: center;
                    gap: 40px;
                    text-align: left;
                    background: rgba(255, 255, 255, 0.3);
                    padding: 40px;
                    border-radius: 15px;
                }

                .profile-img {
                    width: 300px;
                    border: 5px solid var(--white);
                    border-radius: 10px;
                }

                .quote {
                    font-style: italic;
                    font-weight: 600;
                    margin: 10px 0;
                    display: block;
                }

                /* Gallery Section Layout */
                .gallery-grid {
                    display: flex;
                    justify-content: center;
                    gap: 30px;
                    flex-wrap: wrap;
                    margin-top: 40px;
                }

                .gallery-card {
                    flex: 1;
                    min-width: 250px;
                    max-width: 320px;
                    display: flex;
                    flex-direction: column;
                    align-items: center;
                    text-align: center;
                }

                .gallery-image-wrapper {
                    width: 100%;
                    aspect-ratio: 1 / 1;
                    background-color: #fff;
                    border: 5px solid var(--white);
                    box-shadow: 0 4px 10px rgba(0,0,0,0.1);
                    overflow: hidden;
                    margin-bottom: 15px;
                    border-radius: 8px;
                }

                .gallery-image-wrapper img {
                    width: 100%;
                    height: 100%;
                    object-fit: cover;
                }

                .gallery-label {
                    font-weight: 600;
                    color: var(--dark-blue);
                    font-size: 1.2rem;
                }

                /* Darker Blue Sections (Dreams/Interest) */
                .dark-section {
                    background-color: #246a8d;
                    color: white;
                    border-radius: 0;
                }

                .grid {
                    display: grid;
                    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
                    gap: 20px;
                    margin-top: 30px;
                }

                .card img {
                    width: 100%;
                    height: 200px;
                    object-fit: cover;
                    border-radius: 8px;
                }

                .card h3 { margin-top: 10px; }

                footer { text-align: center; padding: 20px; font-size: 0.8rem; }

                /* Responsive */
                @media (max-width: 768px) {
                    .profile-container { flex-direction: column; text-align: center; }
                    h1 { font-size: 2.5rem; }
                    nav { flex-direction: column; padding: 1rem; }
                    nav ul { margin-top: 10px; }
                    .search-container { margin-top: 10px; margin-left: 0; }
                }
            </style>
        </head>
        <body>

            <nav>
                <div class="logo">JT Portfolio</div>
            
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li class="dropdown">
                        <a href="#">Gallery ▾</a>
                        <div class="dropdown-content">
                            <a href="#gallery">My Image</a>
                            <a href="#family">My Family</a>
                        </div>
                    </li>
                    <li><a href="#dreams">Dreams</a></li>
                    <li><a href="#interest">Interest</a></li>
                    <li><a href="#about">About Me</a></li>
                    <li class="search-container">
                        <input type="text" id="searchInput" placeholder="Search...">
                        <button id="searchBtn">🔍</button>
                    </li>
                    </ul>
            </nav>

            <section id="home" class="section">
                <h1>Welcome To My Portfolio</h1>
                <div class="profile-container">
                    <img src="jordan.jpg" alt="Jordan Tianio" class="profile-img">
                    <div class="content">
                        <p>In the world of technology, we are taught that every complex system is built one line of code at a time. My life is much the same—a work in progress where my family is the foundation, my education is the framework, and my dreams are the vision. I believe that learning is not just about gathering facts, but about refining the soul; it is the process of turning our curiosity into a compass that helps us navigate the unknown. Every challenge I face is a lesson that upgrades my character, and every success is a tribute to those who supported me from the start. I code not just to build programs, but to build a future where my work leaves the world a little more functional, a little more connected, and a lot more meaningful than I found it</p>
                    </div>
                </div>
            </section>

            <section id="gallery" class="section">
                <h1>Gallery</h1>
                <div class="gallery-grid">
                    <div class="gallery-card">
                        <div class="gallery-image-wrapper">
                            <img src="childhood1.jpg" alt="Young Me">
                        </div>
                        <p class="quote">"Grown enough to know the simple things are the best things."</p>
                        <span class="gallery-label">My Image</span>
                    </div>
                    <div class="gallery-card">
                        <div class="gallery-image-wrapper">
                            <img src="childhood12345.jpg" alt="Finding joy in the little things.">
                        </div>
                        <p class="quote">"Living the moment."</p>
                        <span class="gallery-label">My Image</span>
                    </div>
            
                    <div id="family" class="gallery-card">
                        <div class="gallery-image-wrapper">
                            <img src="family.jpg" alt="Family">
                        </div>
                        <p class="quote">"The simplest days with them are always the loudest in my heart"</p>
                        <span class="gallery-label">My Family</span>
                    </div>
                </div>
            </section>

            <section id="dreams" class="section dark-section">
                <h1>Dreams</h1>
                <div class="profile-container" style="background: transparent;">
                    <img src="dream.jpg" alt="Coding Dream" style="width:400px">
                    <div>
                        <p>My dream is to walk across that stage, feeling the weight of a diploma that represents every late night and every line of code. I imagine a future where I am not just using technology, but mastering it as an IT professional who builds and protects. There will be days when the systems crash and the solutions seem impossible to find. In those moments of frustration, I will hold onto the truth that every failed script is just a blueprint for a better one.</p>
                        <p style="margin-top:15px;"> I want to earn a place in the tech world that allows me to provide for my family and build a life of stability. The complexity of the digital world doesn't scare me; it invites me to keep learning, growing, and adapting. I see every challenge in my studies as a necessary step toward the expert I am destined to become. With a steady heart and a focused mind, I will turn this vision into my reality.</p>
                    </div>
                </div>
            </section>

            <section id="interest" class="section dark-section" style="background-color: #1e5a7a;">
                <h1>Interest</h1>
                <div class="grid">
                    <div class="card">
                        <img src="mlbblogo.jpg" alt="Games">
                        <h3>ONLINE GAMES</h3>
                    </div>
                    <div class="card">
                        <img src="basketball.webp" alt="Basketball">
                        <h3>Basketball</h3>
                    </div>
                    <div class="card">
                        <img src="jogging.jpg" alt="Jogging">
                        <h3>Jogging</h3>
                    </div>
                </div>
                <p style="margin-top: 30px; font-style: italic;">Hobbies make my free time enjoyable and help me think creatively.</p>
            </section>

            <section id="about" class="section">
                <h1>About Me</h1>
                <div style="max-width: 800px; margin: 0 auto; text-align: left;">
                    <p>Hello! My name is <strong>Jordan Tianio</strong>, and I am a 2nd-year college student taking Bachelor of Science in Computer Science (BSCS).</p>
                    <p>I come from a big family with 8 siblings—5 girls and 3 boys—which has helped me become responsible, patient, and adaptable in different situations.</p>
                    <p>One of my favorite hobbies is playing basketball, as it keeps me active and teaches me teamwork and discipline. I completed my Grade 10 moving-up in 2022 at QNHS and graduated from ICF in Senior High School in 2024.</p>
                    <p>When I was a child, I dreamed of becoming a police officer, but as I grew older, I discovered my interest in technology, which led me to pursue BSCS. I am the kind of person who loves learning new things in life, always curious and eager to grow.</p>
                    <p>My parents have always guided me with important values. They taught me to be content with what I have and to always be thankful to God for all the blessings in life. These lessons continue to inspire me to stay humble, work hard, and appreciate every opportunity that comes my way.</p>
                </div>
            </section>

            <footer>
                &copy; 2026 Jordan Tianio Portfolio
            </footer>

            <script>
                // Smooth scroll for nav links
                document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                    anchor.addEventListener('click', function (e) {
                        e.preventDefault();
                        document.querySelector(this.getAttribute('href')).scrollIntoView({
                            behavior: 'smooth'
                        });
                    });
                });

                // --- SEARCH SCRIPT ---
                const searchBtn = document.getElementById('searchBtn');
                const searchInput = document.getElementById('searchInput');

                function performSearch() {
                    const query = searchInput.value.toLowerCase().trim();
                    if (query === "") return;

                    const sections = document.querySelectorAll('section');
                    let found = false;

                    sections.forEach(section => {
                        const text = section.innerText.toLowerCase();
                        if (text.includes(query)) {
                            section.scrollIntoView({ behavior: 'smooth', block: 'center' });
                            
                            // Add temporary highlight animation
                            section.classList.add('search-highlight');
                            setTimeout(() => {
                                section.classList.remove('search-highlight');
                            }, 3000);

                            found = true;
                        }
                    });

                    if (!found) {
                        alert("Sorry, no results found for '" + query + "'.");
                    }
                }

                searchBtn.addEventListener('click', performSearch);
                
                // Search when 'Enter' is pressed
                searchInput.addEventListener('keypress', function (e) {
                    if (e.key === 'Enter') {
                        performSearch();
                    }
                });
                // ---------------------
            </script>
        </body>
        </html>
