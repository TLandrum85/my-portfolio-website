<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tracey Landrum - Graphic Designer & Web Developer</title>
    <style>
        :root {
            --primary-color: #3498db;
            --secondary-color: #e74c3c;
            --accent-color: #f39c12;
            --background-color: #ecf0f1;
            --text-color: #2c3e50;
        }
        
        body {
            font-family: 'Roboto', sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            color: var(--text-color);
            background-color: var(--background-color);
        }
        
        header {
            background-color: var(--primary-color);
            color: white;
            text-align: center;
            padding: 2rem 0;
            position: relative;
            overflow: hidden;
        }
        
        header::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            height: 30px;
            background: linear-gradient(135deg, var(--background-color) 25%, transparent 25%) -50px 0,
                        linear-gradient(225deg, var(--background-color) 25%, transparent 25%) -50px 0,
                        linear-gradient(315deg, var(--background-color) 25%, transparent 25%),
                        linear-gradient(45deg, var(--background-color) 25%, transparent 25%);
            background-size: 100px 100px;
            background-color: var(--primary-color);
        }
        
        nav {
            background-color: var(--secondary-color);
            padding: 1rem 0;
            text-align: center;
        }
        
        nav ul {
            list-style-type: none;
            padding: 0;
            margin: 0;
        }
        
        nav ul li {
            display: inline;
            margin: 0 15px;
        }
        
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            transition: color 0.3s ease;
        }
        
        nav ul li a:hover {
            color: var(--accent-color);
        }
        
        .container {
            max-width: 1200px;
            margin: 2rem auto;
            padding: 0 20px;
        }
        
        .profile {
            display: flex;
            align-items: center;
            margin-bottom: 2rem;
        }
        
        .profile-img {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            object-fit: cover;
            border: 5px solid var(--secondary-color);
            margin-right: 2rem;
        }
        
        .profile-text h2 {
            color: var(--primary-color);
        }
        
        .skills {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            margin-bottom: 2rem;
        }
        
        .skill-item {
            background-color: white;
            border-radius: 8px;
            padding: 1rem;
            margin: 10px;
            text-align: center;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }
        
        .skill-item:hover {
            transform: translateY(-5px);
        }
        
        .portfolio {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
        }
        
        .portfolio-item {
            position: relative;
            overflow: hidden;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        
        .portfolio-item img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            transition: transform 0.3s ease;
        }
        
        .portfolio-item:hover img {
            transform: scale(1.1);
        }
        
        .portfolio-item .overlay {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background-color: rgba(0, 0, 0, 0.7);
            display: flex;
            align-items: center;
            justify-content: center;
            opacity: 0;
            transition: opacity 0.3s ease;
        }
        
        .portfolio-item:hover .overlay {
            opacity: 1;
        }
        
        .portfolio-item .overlay a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            background-color: var(--accent-color);
            padding: 10px 20px;
            border-radius: 5px;
        }
        
        footer {
            background-color: var(--primary-color);
            color: white;
            text-align: center;
            padding: 1rem 0;
            margin-top: 2rem;
        }
        
        @media (max-width: 768px) {
            .profile {
                flex-direction: column;
                text-align: center;
            }
            
            .profile-img {
                margin-right: 0;
                margin-bottom: 1rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Tracey Landrum</h1>
        <p>Graphic Designer & Web Developer</p>
    </header>
    
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#portfolio">Portfolio</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <div class="container">
        <section class="profile">
            <img src="https://via.placeholder.com/200" alt="Tracey Landrum" class="profile-img">
            <div class="profile-text">
                <h2>Welcome to My Creative World</h2>
                <p>Hello! I'm Tracey Landrum, a passionate graphic designer and web developer. I specialize in creating visually stunning and functional designs that bring ideas to life. With a keen eye for aesthetics and a love for clean code, I craft unique digital experiences that leave a lasting impression.</p>
            </div>
        </section>
        
        <section class="skills">
            <div class="skill-item">
                <h3>Graphic Design</h3>
                <p>Creating visually appealing designs</p>
            </div>
            <div class="skill-item">
                <h3>Web Development</h3>
                <p>Building responsive and interactive websites</p>
            </div>
            <div class="skill-item">
                <h3>UI/UX Design</h3>
                <p>Crafting intuitive user experiences</p>
            </div>
        </section>
        
        <h2>Featured Projects</h2>
        <section class="portfolio">
            <div class="portfolio-item">
                <img src="https://via.placeholder.com/300x250" alt="Project 1">
                <div class="overlay">
                    <a href="#">View Project</a>
                </div>
            </div>
            <div class="portfolio-item">
                <img src="https://via.placeholder.com/300x250" alt="Project 2">
                <div class="overlay">
                    <a href="#">View Project</a>
                </div>
            </div>
            <div class="portfolio-item">
                <img src="https://via.placeholder.com/300x250" alt="Project 3">
                <div class="overlay">
                    <a href="#">View Project</a>
                </div>
            </div>
        </section>
    </div>

    <footer>
        <p>&copy; 2024 Tracey Landrum. All rights reserved.</p>
    </footer>
</body>
</html>
