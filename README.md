<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Explore GAZZ'S UEFN ODYSSEY, showcasing upcoming UEFN Fortnite projects with progress updates.">
    <title>GAZZ'S UEFN ODYSSEY</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        *{box-sizing:border-box;margin:0;padding:0}
        body{font-family:'Montserrat',sans-serif;line-height:1.6;background:linear-gradient(45deg,#0a1a2a,#4a0080,#0a1a2a);background-size:200% 200%;animation:gradientBG 15s ease infinite;color:#fff;scroll-behavior:smooth}
        .light-mode{background:#f0f0f0;color:#333}
        nav{background-color:#001020;padding:1rem;position:sticky;top:0;z-index:100;box-shadow:0 2px 10px rgba(0,183,255,0.3);display:flex;justify-content:center;align-items:center}
        .light-mode nav{background:#fff}
        nav ul{list-style:none;display:flex}
        nav ul li{margin:0 1.5rem}
        nav ul li a{color:#fff;text-decoration:none;font-weight:700;font-size:1.1rem;transition:color 0.3s ease}
        .light-mode nav ul li a{color:#333}
        nav ul li a:hover{color:#ff6600}
        #theme-toggle{background:none;border:none;color:#fff;font-size:1.5rem;cursor:pointer;transition:color 0.3s ease}
        .light-mode #theme-toggle{color:#333}
        .hero{padding:5rem 2rem;text-align:center;background:url('fortnite-background.jpg') no-repeat center center/cover;position:relative;overflow:hidden}
        .hero::before{content:'';position:absolute;top:0;left:0;width:100%;height:100%;background:rgba(0,16,32,0.5);z-index:1}
        .hero h1,.hero p,.hero a{position:relative;z-index:2}
        .hero h1{font-size:3.5rem;font-weight:700}
        .hero p{font-size:1.3rem;margin:1rem 0}
        .hero .cta-btn{display:inline-block;padding:0.75rem 1.5rem;background-color:#ff6600;color:#fff;text-decoration:none;border-radius:5px;font-weight:700;transition:background-color 0.3s ease}
        .hero .cta-btn:hover{background-color:#ff3300}
        .progress-overview,.roadmap,.newsletter,.search-bar{padding:3rem 2rem;text-align:center}
        .progress-overview h2,.roadmap h2,.newsletter h2{font-size:2.8rem;font-weight:700;margin-bottom:1rem}
        .project-cards{display:flex;justify-content:center;flex-wrap:wrap;gap:1.5rem}
        .project-card{background-color:#001020;padding:1.5rem;border-radius:10px;box-shadow:0 4px 15px rgba(0,183,255,0.2);transition:all 0.3s ease;width:220px;color:#fff}
        .project-card:hover{transform:scale(1.05);box-shadow:0 0 20px rgba(0,183,255,0.5)}
        .progress-container{position:relative}
        .progress-bar{width:100%;background-color:#0a1a2a;height:12px;border-radius:6px;overflow:hidden}
        .progress-fill{height:100%;background-color:#00b7ff;width:0;transition:width 1.5s ease-in-out}
        .timeline{position:relative;max-width:900px;margin:0 auto}
        .timeline::before{content:'';position:absolute;top:0;bottom:0;left:50%;width:3px;background-color:#00b7ff}
        .timeline-item{position:relative;width:50%;padding:1.5rem;opacity:0;animation:fadeIn 0.5s ease-in forwards}
        .timeline-item.left{left:0}
        .timeline-item.right{left:50%}
        .timeline-item .content{background-color:#001020;padding:1.5rem;border-radius:10px;box-shadow:0 4px 15px rgba(0,183,255,0.2)}
        .search-container{position:relative;display:inline-block}
        .search-container input{width:320px;padding:0.75rem;border-radius:5px;border:1px solid #555;background-color:#001020;color:#fff}
        .search-container i{position:absolute;right:15px;top:50%;transform:translateY(-50%);color:#aaa;cursor:pointer}
        .newsletter form{max-width:600px;margin:0 auto;display:flex;gap:0.5rem}
        .newsletter input{flex:1;padding:0.75rem;border-radius:5px;border:1px solid #555;background-color:#0a1a2a;color:#fff}
        .newsletter button{background-color:#ff6600;color:#fff;padding:0.75rem 1.5rem;border:none;border-radius:5px;font-weight:700;cursor:pointer}
        .newsletter button:hover{background-color:#ff3300}
        footer{background-color:#001020;padding:1.5rem;text-align:center;color:#fff}
        .back-to-top{position:fixed;bottom:30px;right:30px;background-color:#ff6600;color:#fff;padding:0.75rem 1.5rem;border-radius:5px;text-decoration:none;font-weight:700;display:none;box-shadow:0 2px 10px rgba(255,102,0,0.5);transition:all 0.3s ease}
        .back-to-top:hover{background-color:#ff3300;transform:translateY(-5px)}
        @keyframes fadeIn{from{opacity:0;transform:translateY(20px)}to{opacity:1;transform:translateY(0)}}
        @media (max-width:768px){nav ul{flex-direction:column;align-items:center}nav ul li{margin:0.5rem 0}.project-card{width:90%}}
    </style>
</head>
<body>
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#progress-overview">Progress Overview</a></li>
            <li><a href="#roadmap">Roadmap</a></li>
        </ul>
        <button id="theme-toggle" aria-label="Toggle theme"><i class="fas fa-moon"></i></button>
    </nav>

    <section id="home" class="hero">
        <h1>GAZZ'S UEFN ODYSSEY</h1>
        <p>Embark on a journey through upcoming UEFN Fortnite projects!</p>
        <a href="#progress-overview" class="cta-btn">Explore Now</a>
    </section>

    <section id="progress-overview" class="progress-overview">
        <h2>Project Progress Overview</h2>
        <p>Check out the latest updates on our UEFN Fortnite projects. Click a card to dive into the details!</p>
        <div class="project-cards">
            <a href="#project1" class="project-card" data-progress="15">
                <h3>GAZZ 1V1 BUILD FIGHTS</h3>
                <div class="progress-container">
                    <div class="progress-bar">
                        <div class="progress-fill" data-width="15%"></div>
                    </div>
                </div>
            </a>
            <a href="#project2" class="project-card" data-progress="45">
                <h3>DUBAI CHOCOLATE PILLARS</h3>
                <div class="progress-container">
                    <div class="progress-bar">
                        <div class="progress-fill" data-width="45%"></div>
                    </div>
                </div>
            </a>
            <a href="#project3" class="project-card" data-progress="10">
                <h3>TWDU RICK VS NEGAN RED VS BLUE</h3>
                <div class="progress-container">
                    <div class="progress-bar">
                        <div class="progress-fill" data-width="10%"></div>
                    </div>
                </div>
            </a>
            <a href="#project4" class="project-card" data-progress="5">
                <h3>COMING SOON 👀</h3>
                <div class="progress-container">
                    <div class="progress-bar">
                        <div class="progress-fill" data-width="5%"></div>
                    </div>
                </div>
            </a>
        </div>
    </section>

    <section class="search-bar">
        <div class="search-container">
            <input type="text" id="search" placeholder="Search projects..." onkeyup="searchProjects()" aria-label="Search projects">
            <i class="fas fa-search" onclick="clearSearch()"></i>
        </div>
    </section>

    <section id="roadmap" class="roadmap">
        <h2>Roadmap</h2>
        <div class="timeline">
            <div class="timeline-item left" id="project1">
                <div class="content">
                    <h3>GAZZ 1V1 BUILD FIGHTS</h3>
                    <p>Challenge your friends or foes in intense 1v1 build battles. Show off your skills in a fast-paced arena designed for the ultimate showdown.</p>
                    <span class="date">Expected Release: April 2025</span>
                </div>
            </div>
            <div class="timeline-item right" id="project2">
                <div class="content">
                    <h3>DUBAI CHOCOLATE PILLARS</h3>
                    <p>Start on your own chocolate pillar in a luxurious Dubai-inspired landscape. Build bridges or eliminate opponents to be the last one standing.</p>
                    <span class="date">Expected Release: April 2025</span>
                </div>
            </div>
            <div class="timeline-item left" id="project3">
                <div class="content">
                    <h3>TWDU RICK VS NEGAN RED VS BLUE</h3>
                    <p>Join the fight in a post-apocalyptic world where Rick and Negan lead their teams in a red vs. blue battle. Choose your side and strategize to victory.</p>
                    <span class="date">Expected Release: May 2025</span>
                </div>
            </div>
            <div class="timeline-item right" id="project4">
                <div class="content">
                    <h3>COMING SOON 👀</h3>
                    <p>Exciting projects on the horizon. Stay tuned for more details!</p>
                    <span class="date">Expected Release: 2025</span>
                </div>
            </div>
        </div>
    </section>

    <section class="newsletter">
        <h2>Stay Updated</h2>
        <form action="#" method="post" onsubmit="subscribe(event)">
            <input type="email" name="email" placeholder="Enter your email" required>
            <button type="submit">Subscribe</button>
        </form>
    </section>

    <footer>
        <p>© 2024 GAZZ'S UEFN ODYSSEY. All rights reserved.</p>
        <div class="socials">
            <a href="#"><i class="fab fa-twitter"></i></a>
            <a href="#"><i class="fab fa-discord"></i></a>
        </div>
    </footer>

    <a href="#" class="back-to-top">Back to Top</a>

    <script>
        // Theme Toggle
        const themeToggle = document.getElementById('theme-toggle');
        themeToggle.addEventListener('click', () => {
            document.body.classList.toggle('light-mode');
            themeToggle.innerHTML = document.body.classList.contains('light-mode') ? '<i class="fas fa-sun"></i>' : '<i class="fas fa-moon"></i>';
        });

        // Back to Top Button
        window.addEventListener('scroll', () => {
            document.querySelector('.back-to-top').style.display = window.scrollY > 300 ? 'block' : 'none';
        });

        // Progress Bar Animation
        document.addEventListener('DOMContentLoaded', () => {
            document.querySelectorAll('.progress-fill').forEach(fill => {
                fill.style.width = fill.getAttribute('data-width');
            });
        });

        // Search Functionality
        function searchProjects() {
            const input = document.getElementById('search').value.toLowerCase();
            const items = document.querySelectorAll('.timeline-item');
            items.forEach(item => {
                const title = item.querySelector('h3').textContent.toLowerCase();
                const description = item.querySelector('p').textContent.toLowerCase();
                if (title.includes(input) || description.includes(input)) {
                    item.style.display = 'block';
                } else {
                    item.style.display = 'none';
                }
            });
        }

        // Clear Search
        function clearSearch() {
            document.getElementById('search').value = '';
            searchProjects();
        }

        // Newsletter Subscription (Placeholder)
        function subscribe(event) {
            event.preventDefault();
            alert('Thanks for subscribing! Stay tuned for updates.');
            event.target.reset();
        }
    </script>
</body>
</html>
