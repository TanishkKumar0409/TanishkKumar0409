<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tanishk Kumar - Web Developer</title>
    <!-- Font Awesome CDN -->
    <script src="https://kit.fontawesome.com/87f0afa689.js" crossorigin="anonymous"></script>
    <style>
        /* Typing animation */
        @keyframes typing {
            from { width: 0; }
            to { width: 100%; }
        }

        @keyframes blink-caret {
            50% { border-color: transparent; }
        }

        /* General styling */
        body {
            margin: 0;
            padding: 0;
            font-family: 'Arial', sans-serif;
            background: linear-gradient(135deg, #1d4b99, #e94560);
            color: #ffffff;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            text-align: center;
            overflow-x: hidden;
        }

        header {
            margin-bottom: 40px;
        }

        .typing-container {
            display: inline-block;
            font-size: 2.5rem;
            white-space: nowrap;
            overflow: hidden;
            border-right: 3px solid #ffffff;
            width: 0;
            animation: typing 3.5s steps(40, end) forwards, blink-caret 0.7s step-end infinite;
        }

        h2 {
            font-size: 1.5rem;
            color: #ffd700;
            margin-top: 10px;
        }

        /* Section styling */
        section {
            max-width: 1100px;
            margin: 20px auto;
            padding: 20px;
            background-color: #181818;
            border-radius: 10px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.8);
            opacity: 0;
            transform: translateY(30px);
            transition: opacity 1s, transform 1s;
        }

        section.visible {
            opacity: 1;
            transform: translateY(0);
        }

        section h3 {
            color: #ffd700;
            margin-bottom: 20px;
        }

        /* Known Languages & Tools */
        .tools-list {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            list-style-type: none;
            padding: 0;
            gap: 20px; /* Add spacing between items */
        }

        .tools-list li {
            background-color: #333;
            color: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
            transition: transform 0.3s ease, background-color 0.3s ease;
            text-align: center; /* Center-align text and icon */
            width: 150px; /* Fixed width */
        }

        .tools-list li i {
            font-size: 3rem; /* Increase icon size */
            display: block;
            margin-bottom: 10px; /* Space between icon and text */
        }

        .tools-list li:hover {
            background-color: #1d4b99;
            transform: translateY(-10px);
        }

        /* Contact Info */
        .contact-info {
            background-color: #222;
            padding: 20px;
            border-radius: 8px;
            transition: background-color 0.5s ease;
        }

        .contact-info:hover {
            background-color: #1d4b99;
        }

        /* Fun Fact */
        .fun-fact {
            color: #e94560;
            font-size: 1.3rem;
            margin-top: 20px;
        }

        footer {
            text-align: center;
            padding: 15px;
            background-color: #1d1d1d;
            margin-top: 20px;
            width: 100%;
            border-top: 2px solid #1d4b99;
        }

        /* Media Queries */
        @media (max-width: 768px) {
            .tools-list li {
                width: 120px; /* Adjust width for smaller screens */
                text-align: center;
            }

            h1 {
                font-size: 2rem;
            }

            h2 {
                font-size: 1.2rem;
            }
        }

        /* Scroll animations */
        .fade-in {
            opacity: 0;
            transform: translateY(20px);
            transition: all 0.6s ease-out;
        }

        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }
    </style>
</head>
<body>

    <header>
        <div class="typing-container">
            Hi there 👋, I'm Tanishk Kumar!
        </div>
        <h2>Passionate Web Developer | Dark Themes | Animation Enthusiast</h2>
    </header>

    <section class="fade-in">
        <h3><i class="fas fa-code"></i> 🔧 Known Languages & Tools</h3>
        <ul class="tools-list">
            <li><i class="fab fa-html5"></i> HTML</li>
            <li><i class="fab fa-css3-alt"></i> CSS</li>
            <li><i class="fab fa-sass"></i> SCSS</li>
            <li><i class="fas fa-database"></i> MySQL</li>
            <li><i class="fab fa-java"></i> Java</li>
            <li><i class="fab fa-bootstrap"></i> Bootstrap</li>
            <li><i class="fab fa-figma"></i> Figma</li>
            <li><i class="fab fa-git"></i> Git</li>
            <li><i class="fab fa-github"></i> GitHub</li>
            <li><i class="fas fa-file-alt"></i> MS Office</li> <!-- Added MS Office -->
        </ul>
    </section>

    <section class="fade-in">
        <h3><i class="fas fa-project-diagram"></i> 🚀 What I'm Working On</h3>
        <p>Improving designs for interactive elements such as carousels, accordions, and navigations using JavaScript, Tailwind CSS, and Bootstrap.</p>
    </section>

    <section class="fade-in">
        <h3><i class="fas fa-laptop-code"></i> 🌱 Learning & Growth</h3>
        <p>Exploring new ways to incorporate Tailwind CSS for efficient and scalable design and enhancing my skills in UI/UX design to create more engaging user experiences.</p>
    </section>

    <section class="fade-in">
        <h3><i class="fas fa-briefcase"></i> 💼 Experience</h3>
        <p>Completed a 3-month web development internship at Offbeat Pixels, working on four projects, honing my web design and development skills.</p>
    </section>

    <section class="fade-in contact-info">
        <h3><i class="fas fa-envelope"></i> 📫 How to Reach Me</h3>
        <p>Contact No.: 95576213131</p>
        <p>Email: tanishkk60@gmail.com</p>
    </section>

    <section class="fade-in">
        <h3><i class="fas fa-smile"></i> ⚡ Fun Fact</h3>
        <p class="fun-fact">I love experimenting with dark color schemes and finding new ways to add a touch of creativity to my web designs!</p>
    </section>

    <footer>
        <p>Made with ❤️ by Tanishk Kumar</p>
    </footer>

    <script>
        // Scroll animation - add 'visible' class when the section enters the viewport
        const fadeIns = document.querySelectorAll('.fade-in');

        const appearOnScroll = new IntersectionObserver(function(entries, observer) {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                    observer.unobserve(entry.target); // Stop observing once it appears
                }
            });
        }, { threshold: 0.2 });

        fadeIns.forEach(fadeIn => {
            appearOnScroll.observe(fadeIn);
        });
    </script>
</body>
</html>
