<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Portfolio of Raji Quadri (ADETUNJI), AI nerd, vibe coder, and freelancer.">
    <meta name="keywords" content="Raji Quadri, ADETUNJI, AI freelancer, machine learning, web development, vibe coder">
    <meta name="author" content="Raji Quadri">
    <title>Raji Quadri | AI Nerd & Vibe Coder</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Inter', sans-serif;
        }

        body {
            background: #1A1A1A;
            color: #FFFFFF;
        }

        nav {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(26, 26, 26, 0.9);
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            z-index: 1000;
        }

        nav a {
            color: #36A2EB;
            text-decoration: none;
            margin: 0 1rem;
            font-weight: 600;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #FF6384;
        }

        section {
            padding: 5rem 2rem;
            scroll-margin-top: 80px;
        }

        #hero {
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            background: linear-gradient(45deg, #1A1A1A, #2A2A2A);
        }

        #hero h1 {
            font-size: 3rem;
            color: #36A2EB;
        }

        #hero p {
            font-size: 1.5rem;
            margin: 1rem 0;
        }

        .cta-button {
            background: #FF6384;
            color: #FFFFFF;
            padding: 0.75rem 1.5rem;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 600;
            transition: background 0.3s;
        }

        .cta-button:hover {
            background: #CC4B67;
        }

        #about, #skills, #projects, #contact {
            max-width: 1200px;
            margin: 0 auto;
        }

        h2 {
            font-size: 2.5rem;
            color: #36A2EB;
            margin-bottom: 1rem;
        }

        #about p {
            line-height: 1.6;
            margin-bottom: 1rem;
        }

        #skills canvas {
            max-width: 600px;
            margin: 2rem auto;
        }

        .project-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .project-card {
            background: #2A2A2A;
            padding: 1.5rem;
            border-radius: 10px;
            transition: transform 0.3s;
        }

        .project-card:hover {
            transform: translateY(-5px);
        }

        .project-card h3 {
            color: #36A2EB;
            margin-bottom: 0.5rem;
        }

        #contact form {
            display: flex;
            flex-direction: column;
            gap: 1rem;
            max-width: 500px;
            margin: 2rem auto;
        }

        #contact input, #contact textarea {
            padding: 0.75rem;
            border: none;
            border-radius: 5px;
            background: #3A3A3A;
            color: #FFFFFF;
        }

        #contact button {
            background: #FF6384;
            color: #FFFFFF;
            padding: 0.75rem;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s;
        }

        #contact button:hover {
            background: #CC4B67;
        }

        .social-links a {
            color: #36A2EB;
            margin: 0 1rem;
            font-size: 1.2rem;
            text-decoration: none;
        }

        .social-links a:hover {
            color: #FF6384;
        }

        footer {
            text-align: center;
            padding: 2rem;
            background: #2A2A2A;
        }

        @media (max-width: 768px) {
            #hero h1 {
                font-size: 2rem;
            }

            #hero p {
                font-size: 1.2rem;
            }

            nav a {
                margin: 0 0.5rem;
                font-size: 0.9rem;
            }
        }
    </style>
</head>
<body>
    <nav>
        <div>Raji Quadri</div>
        <div>
            <a href="#hero">Home</a>
            <a href="#about">About</a>
            <a href="#skills">Skills</a>
            <a href="#projects">Projects</a>
            <a href="#contact">Contact</a>
        </div>
    </nav>

    <section id="hero">
        <h1>Raji Quadri</h1>
        <p>AI Nerd | Vibe Coder | Freelancer</p>
        <a href="#contact" class="cta-button">Let's Collaborate</a>
    </section>

    <section id="about">
        <h2>About Me</h2>
        <p>They say the future is now, and I’m building it, one line of code and one intelligent algorithm at a time. My name is Raji Quadri, and I’m not just a coder; I'm an AI nerd with a relentless curiosity for how machines can learn, adapt, and create. From the bustling streets of Nigeria, I operate as a freelancer, translating complex ideas into elegant, AI-powered solutions.</p>
        <p>Whether it's crafting intelligent chatbots, developing predictive models, or building seamless web applications, I thrive on bringing innovative concepts to life. My journey is fueled by a passion for continuous learning and a commitment to delivering work that exceeds expectations, all while maintaining that perfect coding "vibe."</p>
    </section>

    <section id="skills">
        <h2>My Skills</h2>
        <canvas id="skillsChart"></canvas>
    </section>

    <section id="projects">
        <h2>Featured Projects</h2>
        <div class="project-grid">
            <div class="project-card">
                <h3>AI-Powered Chatbot for E-commerce</h3>
                <p>Enhanced customer support with a conversational AI, reducing response time by 40% and increasing leads by 15%.</p>
                <p><strong>Tools:</strong> Python, NLTK, Flask</p>
            </div>
            <div class="project-card">
                <h3>Predictive Analytics Dashboard</h3>
                <p>Built a tool for Nigerian businesses to forecast sales, reducing waste by 10% and boosting profits by 5%.</p>
                <p><strong>Tools:</strong> Python, Pandas, Django</p>
            </div>
            <div class="project-card">
                <h3>Responsive Web App for Learning</h3>
                <p>Created an intuitive platform for youth to learn coding and AI, improving retention by 80%.</p>
                <p><strong>Tools:</strong> React.js, Node.js, MongoDB</p>
                <a href="https://github.com/Boykvsh/githubTest" target="_blank">View on GitHub</a>
            </div>
        </div>
    </section>

    <section id="contact">
        <h2>Connect & Collaborate</h2>
        <form>
            <input type="text" placeholder="Name" required>
            <input type="email" placeholder="Email" required>
            <textarea placeholder="Your Message" rows="5" required></textarea>
            <button type="submit">Send Message</button>
        </form>
        <div class="social-links">
            <a href="mailto:rajiquadri92@gmail.com">Email</a>
            <a href="https://linkedin.com/in/rajiquadriAI" target="_blank">LinkedIn</a>
            <a href="https://github.com/Boykvsh" target="_blank">GitHub</a>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 Raji Quadri. Building the future with AI.</p>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <script>
        // Smooth scrolling for nav links
        document.querySelectorAll('nav a').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Skills Chart
        const ctx = document.getElementById('skillsChart').getContext('2d');
        new Chart(ctx, {
            type: 'bar',
            data: {
                labels: ['Python', 'Machine Learning', 'Web Development', 'Data Analysis', 'AI Ethics'],
                datasets: [{
                    label: 'Skill Proficiency (%)',
                    data: [85, 70, 65, 60, 50],
                    backgroundColor: ['#36A2EB', '#FF6384', '#4BC0C0', '#FFCE56', '#9966FF'],
                    borderColor: ['#2A80B9', '#CC4B67', '#3A9C9C', '#CCA33F', '#7A52CC'],
                    borderWidth: 1
                }]
            },
            options: {
                scales: {
                    y: {
                        beginAtZero: true,
                        max: 100,
                        title: {
                            display: true,
                            text: 'Proficiency (%)'
                        }
                    },
                    x: {
                        title: {
                            display: true,
                            text: 'Skills'
                        }
                    }
                },
                plugins: {
                    legend: {
                        display: false
                    },
                    title: {
                        display: true,
                        text: 'My Self-Learned Skills'
                    }
                }
            }
        });
    </script>
</body>
</html>