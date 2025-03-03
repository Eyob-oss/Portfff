<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Eyob Tesfaye's Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* General Styles */
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #f5f7fa, #c3cfe2);
            color: #333;
            animation: backgroundAnimation 10s infinite alternate;
        }

        @keyframes backgroundAnimation {
            0% { background: linear-gradient(135deg, #f5f7fa, #c3cfe2); }
            100% { background: linear-gradient(135deg, #c3cfe2, #f5f7fa); }
        }

        /* Header Section */
        header {
            text-align: center;
            padding: 50px;
            background: #4a90e2;
            color: white;
            position: relative;
            overflow: hidden;
        }

        h1 {
            font-size: 3em;
            margin: 0;
            animation: fadeInDown 2s ease-in-out;
        }

        .contact-info {
            margin: 20px 0;
            animation: fadeInUp 2s ease-in-out;
        }

        .contact-info a {
            text-decoration: none;
            color: white;
            font-size: 1.5em;
            margin: 0 15px;
            display: inline-flex;
            align-items: center;
        }

        .icon {
            width: 30px;
            margin-right: 10px;
        }

        /* Animation Keyframes */
        @keyframes fadeInDown {
            from { opacity: 0; transform: translateY(-50px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(50px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* About Section */
        section.about {
            padding: 50px;
            text-align: center;
            background: rgba(255, 255, 255, 0.9);
            border-radius: 20px;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
            margin: 20px;
            animation: slideInLeft 2s ease-in-out;
        }

        section.about p {
            font-size: 1.2em;
            line-height: 1.6;
        }

        @keyframes slideInLeft {
            from { opacity: 0; transform: translateX(-100px); }
            to { opacity: 1; transform: translateX(0); }
        }

        /* Skills Section */
        section.skills {
            padding: 50px;
            background: #f5f7fa;
            text-align: center;
            animation: slideInRight 2s ease-in-out;
        }

        .skills-list {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 20px;
        }

        .skill-item {
            background: #ffffff;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            padding: 20px;
            width: 200px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            animation: pulse 2s infinite;
        }

        .skill-item:hover {
            transform: scale(1.1);
            box-shadow: 0 8px 12px rgba(0, 0, 0, 0.2);
        }

        .skill-item h3 {
            font-size: 1.5em;
            margin-bottom: 10px;
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.05); }
        }

        /* Projects Section */
        section.projects {
            padding: 50px;
            text-align: center;
            background: rgba(255, 255, 255, 0.9);
            border-radius: 20px;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
            margin: 20px;
            animation: fadeIn 2s ease-in-out;
        }

        .project-list {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 20px;
        }

        .project-item {
            background: #ffffff;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            padding: 20px;
            width: 300px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .project-item:hover {
            transform: scale(1.1);
            box-shadow: 0 8px 12px rgba(0, 0, 0, 0.2);
        }

        .project-item h3 {
            font-size: 1.5em;
            margin-bottom: 10px;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        /* Contact Section */
        section.contact {
            padding: 50px;
            background: #4a90e2;
            color: white;
            text-align: center;
            animation: slideInUp 2s ease-in-out;
        }

        form {
            display: flex;
            flex-direction: column;
            max-width: 500px;
            margin: 0 auto;
        }

        input, textarea {
            padding: 10px;
            margin: 10px 0;
            border: none;
            border-radius: 5px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }

        button {
            padding: 10px;
            background: #ffffff;
            color: #4a90e2;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s ease, transform 0.3s ease;
        }

        button:hover {
            background: #4a90e2;
            color: white;
            transform: scale(1.1);
        }

        @keyframes slideInUp {
            from { opacity: 0; transform: translateY(100px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Footer Section */
        footer {
            text-align: center;
            padding: 20px;
            background-color: #4a90e2;
            color: white;
            animation: fadeIn 2s ease-in-out;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .skills-list, .project-list {
                flex-direction: column;
                align-items: center;
            }
        }
    </style>
</head>
<body>
    <!-- Header Section -->
    <header>
        <h1>Eyob Tesfaye</h1>
        <div class="contact-info">
            <a href="mailto:eyob0081@gmail.com">
                <img src="https://img.icons8.com/material-outlined/24/ffffff/email.png" class="icon" alt="Email Icon"> 
                eyob0081@gmail.com
            </a>
            <a href="tel:+251985754689">
                <img src="https://img.icons8.com/material-outlined/24/ffffff/phone.png" class="icon" alt="Phone Icon"> 
                +251985754689
            </a>
            <a href="https://www.tiktok.com/@softrum_01">
                <img src="https://img.icons8.com/material-outlined/24/ffffff/tiktok.png" class="icon" alt="TikTok Icon"> 
                @softrum_01
            </a>
            <a href="https://t.me/softrum_01">
                <img src="https://img.icons8.com/material-outlined/24/ffffff/telegram-app.png" class="icon" alt="Telegram Icon"> 
                t.me/softrum_01
            </a>
        </div>
    </header>

    <!-- About Section -->
    <section class="about">
        <h2>About Me</h2>
        <p>
            Hi, I'm Eyob Tesfaye, a passionate developer and digital creator. I specialize in web development and creating engaging content for platforms like TikTok and Telegram. My goal is to build innovative solutions that make a difference.
        </p>
    </section>

    <!-- Skills Section -->
    <section class="skills">
        <h2>My Skills</h2>
        <div class="skills-list">
            <div class="skill-item">
                <h3>Web Development</h3>
                <p>HTML, CSS, JavaScript, React</p>
            </div>
            <div class="skill-item">
                <h3>Content Creation</h3>
                <p>TikTok, Telegram, Social Media</p>
            </div>
            <div class="skill-item">
                <h3>Graphic Design</h3>
                <p>Adobe Photoshop, Illustrator</p>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section class="projects">
        <h2>My Projects</h2>
        <div class="project-list">
            <div class="project-item">
                <h3>Project 1</h3>
                <p>A brief description of your first project.</p>
            </div>
            <div class="project-item">
                <h3>Project 2</h3>
                <p>A brief description of your second project.</p>
            </div>
            <div class="project-item">
                <h3>Project 3</h3>
                <p>A brief description of your third project.</p>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact">
        <h2>Contact Me</h2>
        <form>
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <textarea placeholder="Your Message" required></textarea>
            <button type="submit">Send Message</button>
        </form>
    </section>

    <!-- Footer Section -->
    <footer>
        <p>&copy; 2023 Eyob Tesfaye. All rights reserved.</p>
    </footer>
</body>
</html>
