# Ganeshuuu
This is my website
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Portfolio</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0; /* Light gray background color */
        }
        header {
            background-color: #333;
            color: #fff;
            padding: 20px;
            text-align: center;
        }
        nav {
            background-color: #666;
            padding: 10px 0;
            text-align: center;
        }
        nav a {
            color: #fff;
            text-decoration: none;
            padding: 10px 20px;
        }
        section {
            padding: 20px;
            background-color: #fff; /* White background color */
            margin-bottom: 20px; /* Add some spacing between sections */
            border-radius: 5px; /* Add rounded corners to sections */
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* Add shadow effect */
        }
        footer {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 10px 0;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
        /* CSS for small profile picture */
        .profile-picture {
            width: 100px; /* Adjust the size of the image */
            height: auto;
            display: block; /* Ensures the image is centered */
            margin: 0 auto; /* Centers the image */
            border-radius: 50%; /* Make the image round */
        }
        /* Colors for headings */
        h1 {
            color: #ffcc00; /* Yellow */
        }
        h2 {
            color: #007bff; /* Blue */
        }
        h3 {
            color: #28a745; /* Green */
        }
        /* Color for links */
        a {
            color: #007bff; /* Blue */
        }
        /* Hover effect for links */
        a:hover {
            text-decoration: underline;
        }
        /* Hide sections by default */
        .hidden {
            display: none;
        }
    </style>
</head>
<body>
    <header>
        <h1>GANESH SIRLA</h1>
        <p>Web Developer</p>
    </header>
    <nav>
        <button onclick="toggleSection('about')">About</button>
        <button onclick="toggleSection('projects')">Projects</button>
        <button onclick="toggleSection('contact')">Contact</button>
    </nav>
    <section id="about">
        <h2>About Me</h2>
        <p>I'm an Information Technology student at JNTUGV Vizianagaram. My roll number is 23VV1A1249. I come from a supportive family. My father, Sirla Bhagavan, is a farmer, and my mother, Sirla Chinnammudu, is a homemaker. I have a younger sister, Sirlayamani, who is currently in 10th grade at ZPHS School, Urlam. My long-term goal is to become a Navy Officer.</p>
        <!-- Small image added below -->
        <img class="profile-picture" src="https://r2.easyimg.io/kr0a0clan/img_20240309_161440.jpg" alt="Profile Picture">
    </section>
    <section id="projects" class="hidden">
        <h2>Projects</h2>
        <div>
            <h3>Project 1</h3>
            <p>My Portfolio</p>
        </div>
        <div>
            <h3>Project 2</h3>
            <p>Basics of C</p>
        </div>
        <!-- Add more project sections as needed -->
    </section>
    <section id="contact" class="hidden">
        <h2>Contact Me</h2>
        <p>Email: ganeshsirla87@gmail.com</p>
        <p>Phone: 9381063100</p>
        <a href="https://www.instagram.com/ganesh_.sirla?utm_source=qr&igsh=MWE1MHg2eHl2bTVkdw==">Visit Example</a>
        
    </section>
    <footer>
        &copy; 2024 GANESH SIRLA
    </footer>
    
    <script>
        // Function to toggle section visibility
        function toggleSection(sectionId) {
            // Hide all sections
            document.querySelectorAll('section').forEach(section => {
                section.classList.add('hidden');
            });
            // Show the selected section
            document.getElementById(sectionId).classList.remove('hidden');
        }
    </script>
</body>
</html>
