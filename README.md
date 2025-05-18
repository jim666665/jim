<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Students' Helper - Smart Learning & Wellness Platform</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root {
            --primary: #3F51B5;
            --secondary: #00BCD4;
            --accent: #FF9800;
        }

        body {
            font-family: 'Roboto', sans-serif;
            line-height: 1.6;
            margin: 0;
            background: #f5f5f5;
        }

        .header {
            background: var(--primary);
            color: white;
            padding: 2rem;
            text-align: center;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }

        .nav {
            display: flex;
            justify-content: center;
            gap: 2rem;
            padding: 1rem;
            background: white;
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .nav a {
            color: var(--primary);
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s;
        }

        .nav a:hover {
            color: var(--accent);
        }

        .section {
            padding: 4rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .card-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .card {
            background: white;
            border-radius: 12px;
            padding: 1.5rem;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
            transition: transform 0.3s;
            cursor: pointer;
            position: relative;
            overflow: hidden;
        }

        .card::after {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            border: 2px solid var(--secondary);
            opacity: 0;
            transition: opacity 0.3s;
        }

        .card:hover {
            transform: translateY(-5px);
        }

        .card:hover::after {
            opacity: 1;
        }

        .card a {
            text-decoration: none;
            color: inherit;
            display: block;
        }

        .feature-icon {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 1rem;
        }

        .hero {
            background: linear-gradient(rgba(63, 81, 181, 0.9), rgba(0, 188, 212, 0.9)),
                        url('https://images.unsplash.com/photo-1524995997946-a1c2e315a42f') center/cover;
            color: white;
            text-align: center;
            padding: 6rem 2rem;
        }

        .tech-badge {
            background: var(--secondary);
            color: white;
            padding: 0.5rem 1.5rem;
            border-radius: 20px;
            display: inline-block;
            margin: 0.5rem;
            font-size: 0.9rem;
        }

        .footer {
            background: #263238;
            color: white;
            padding: 2rem;
            text-align: center;
        }

        @media (max-width: 768px) {
            .nav {
                flex-direction: column;
                text-align: center;
                gap: 1rem;
            }
        }
    </style>
</head>
<body>
    <header class="header">
        <h1>Students' Helper</h1>
        <p>Your Intelligent Learning & Wellness Companion</p>
    </header>

    <nav class="nav">
        <a href="#learn">Learning Tools</a>
        <a href="#wellness">Wellness Support</a>
        <a href="#finance">Financial Tools</a>
    </nav>

    <div class="hero">
        <h2>Empowering Smarter Learning & Balanced Life</h2>
        <p>AI-powered solutions for academic success and mental wellness</p>
    </div>

    <!-- Learning Tools Section -->
    <section id="learn" class="section">
        <h2><i class="fas fa-graduation-cap feature-icon"></i> Smart Learning Tools</h2>
        <div class="card-grid">
            <div class="card" onclick="window.open('https://chat.deepseek.com/', '_blank')">
                <a href="https://chat.deepseek.com/" target="_blank">
                    <h3>AI Homework Solver</h3>
                    <p>Snap or type questions to receive step-by-step solutions with detailed explanations</p>
                </a>
            </div>

            <div class="card" onclick="window.open('https://app.reclaim.ai/planner', '_blank')">
                <a href="https://app.reclaim.ai/planner" target="_blank">
                    <h3>Smart Study Planner</h3>
                    <p>Automated schedule generation based on your courses and academic goals</p>
                </a>
            </div>

            <div class="card" onclick="window.open('https://notegpt.io/workspace/home', '_blank')">
                <a href="https://notegpt.io/workspace/home" target="_blank">
                    <h3>Flashcard Generator</h3>
                    <p>Automatic creation of study cards from your course materials</p>
                </a>
            </div>
        </div>
    </section>

    <!-- Wellness Support Section -->
    <section id="wellness" class="section" style="background: #fff;">
        <h2><i class="fas fa-heartbeat feature-icon"></i> Wellness Support System</h2>
        <div class="card-grid">
            <div class="card" onclick="window.open('https://www.qzxqai.com/', '_blank')">
                <a href="https://www.qzxqai.com/" target="_blank">
                    <h3>CBT Therapy Chat</h3>
                    <p>AI-powered cognitive behavioral therapy sessions</p>
                </a>
            </div>

            <div class="card" onclick="window.open('https://play.google.com/store/apps/details?id=moodtracker.selfcare.habittracker.mentalhealth', '_blank')">
                <a href="https://play.google.com/store/apps/details?id=moodtracker.selfcare.habittracker.mentalhealth" target="_blank">
                    <h3>Mood Tracker</h3>
                    <p>Daily emotional analysis and personalized reports</p>
                </a>
            </div>

            <div class="card" onclick="window.open('https://www.headspace.com/', '_blank')">
                <a href="https://www.headspace.com/" target="_blank">
                    <h3>Sleep Assistant</h3>
                    <p>Guided meditation and breathing exercises for better sleep</p>
                </a>
            </div>
        </div>
    </section>

    <!-- Financial Tools Section -->
    <section id="finance" class="section">
        <h2><i class="fas fa-coins feature-icon"></i> Financial Empowerment</h2>
        <div class="card-grid">
            <div class="card" onclick="window.open('https://www.creditkarma.com/', '_blank')">
                <a href="https://www.creditkarma.com/" target="_blank">
                    <h3>Smart Savings Planner</h3>
                    <p>AI-generated financial plans for your personal goals</p>
                </a>
            </div>

            <div class="card" onclick="window.open('https://preply.com/en/online/english-tutors', '_blank')">
                <a href="https://preply.com/en/online/english-tutors" target="_blank">
                    <h3>Tutoring Platform</h3>
                    <p>Monetize your academic skills through 1-on-1 tutoring</p>
                </a>
            </div>
        </div>
    </section>

    <footer class="footer">
        <p>© 2024 Students' Helper - Transforming Student Success</p>
        <p>Contact: support@studentshelper.com | Help Center</p>
    </footer>
</body>
</html>
