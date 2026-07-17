
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Frontend Page</title>
    <style>
        /* CSS Reset & Variables */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        :root {
            --primary-color: #4f46e5;
            --secondary-color: #1e1b4b;
            --bg-color: #f8fafc;
            --text-color: #334155;
            --card-bg: #ffffff;
        }

        /* Base Styles */
        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
            background-color: var(--bg-color);
            color: var(--text-color);
            line-height: 1.6;
        }

        /* Navigation Bar */
        nav {
            background-color: var(--card-bg);
            box-shadow: 0 1px 3px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        .nav-container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .logo {
            font-size: 1.25rem;
            font-weight: 700;
            color: var(--primary-color);
        }
        .nav-links {
            list-style: none;
            display: flex;
            gap: 1.5rem;
        }
        .nav-links a {
            text-decoration: none;
            color: var(--text-color);
            font-weight: 500;
            transition: color 0.2s;
        }
        .nav-links a:hover {
            color: var(--primary-color);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #e0e7ff 0%, #ffffff 100%);
            padding: 5rem 2rem;
            text-align: center;
        }
        .hero-container {
            max-width: 800px;
            margin: 0 auto;
        }
        .hero h1 {
            font-size: 2.5rem;
            color: var(--secondary-color);
            margin-bottom: 1rem;
        }
        .hero p {
            font-size: 1.1rem;
            margin-bottom: 2rem;
            color: #64748b;
        }
        .btn {
            display: inline-block;
            background-color: var(--primary-color);
            color: white;
            padding: 0.75rem 1.5rem;
            border-radius: 0.375rem;
            text-decoration: none;
            font-weight: 500;
            border: none;
            cursor: pointer;
            transition: background-color 0.2s;
        }
        .btn:hover {
            background-color: #4338ca;
        }

        /* Features Section */
        .features {
            max-width: 1100px;
            margin: 4rem auto;
            padding: 0 2rem;
        }
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }
        .card {
            background-color: var(--card-bg);
            padding: 2rem;
            border-radius: 0.5rem;
            box-shadow: 0 4px 6px -1px rgba(0,0,0,0.05);
            border: 1px solid #e2e8f0;
        }
        .card h3 {
            margin-bottom: 0.5rem;
            color: var(--secondary-color);
        }

        /* Footer */
        footer {
            background-color: var(--secondary-color);
            color: #94a3b8;
            text-align: center;
            padding: 2rem;
            margin-top: 4rem;
        }
    </style>
</head>
<body>

    <!-- Navigation Bar -->
    <nav>
        <div class="nav-container">
            <div class="logo">MyBrand</div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#features">Features</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </div>
    </nav>

    <!-- Main Content Area -->
    <main>
        <!-- Hero Section -->
        <section class="hero" id="home">
            <div class="hero-container">
                <h1>Welcome to Your New Frontend</h1>
                <p>A clean, responsive, and modern layout built using semantic HTML5 tags and flexible CSS grids.</p>
                <button class="btn" id="action-btn">Click For Magic</button>
            </div>
        </section>

        <!-- Features Section -->
        <section class="features" id="features">
            <div class="grid">
                <div class="card">
                    <h3>⚡ Modern Stack</h3>
                    <p>Clean code base configured natively inside a single document block.</p>
                </div>
                <div class="card">
                    <h3>📱 Fully Responsive</h3>
                    <p>Adapts automatically to layout environments like tablets and mobile viewports.</p>
                </div>
                <div class="card">
                    <h3>🎨 Clean Styling</h3>
                    <p>Utilizes system typography and CSS variable parameters for easy design changes.</p>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer Area -->
    <footer>
        <p>&copy; 2026 MyBrand Frontend Page. All rights reserved.</p>
    </footer>

    <!-- JavaScript Interactivity -->
    <script>
        const alertButton = document.getElementById('action-btn');
        alertButton.addEventListener('click', () => {
            alert('Hello! This alert proves your JavaScript integration is working successfully.');
        });
    </script>
</body>
</html>
