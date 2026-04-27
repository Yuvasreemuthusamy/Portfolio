# Ex01 Portfolio
## Date: 27/04/2026

## Name: Yuva Sree M
## Register Number: 212223230251


## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM

## index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Yuva Sree M | Data Analyst</title>
    <link rel="stylesheet" href="style.css">

    <!-- Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
</head>
<body>

<!-- HERO -->
<section class="hero">
    <h2>Hello 👋</h2>
    <h1>Welcome to My Portfolio</h1>
    <p>I am <span>Yuva Sree M</span></p>
    <p class="role">Aspiring Data Analyst</p>

    <div class="social-icons">
        <a href="https://github.com/Yuvasreemuthusamy" target="_blank">
            <i class="fab fa-github"></i>
        </a>
        <a href="https://www.linkedin.com/in/yuvasreem1556" target="_blank">
            <i class="fab fa-linkedin"></i>
        </a>
    </div>
</section>

<!-- ABOUT -->
<section id="about">
    <h2>About Me</h2>

    <div class="about-box">
        <p>
            I am a passionate and detail-oriented aspiring Data Analyst with a strong interest in
            transforming raw data into meaningful insights. I enjoy analyzing data, identifying trends,
            and solving real-world problems.
        </p>

        <p>
            I have hands-on knowledge in data cleaning, data manipulation, and data visualization.
            I am skilled in SQL, Advanced Excel, and Power BI, along with NumPy and Pandas.
        </p>

        <p>
            I also have a strong foundation in statistics and probability, helping me understand
            data behavior and make accurate decisions.
        </p>

        <p>
            I am a continuous learner who enjoys working on real-world projects and improving my
            analytical thinking. My goal is to become a professional Data Analyst.
        </p>
    </div>
</section>

<!-- SKILLS -->
<section id="skills">
    <h2>Skills</h2>

    <div class="skills-grid">
        <div class="skill"><i class="fas fa-file-excel"></i><p>Excel</p></div>
        <div class="skill"><i class="fas fa-database"></i><p>SQL</p></div>
        <div class="skill"><i class="fas fa-chart-bar"></i><p>Power BI</p></div>
        <div class="skill"><i class="fas fa-broom"></i><p>Cleaning</p></div>
        <div class="skill"><i class="fas fa-cogs"></i><p>Manipulation</p></div>
        <div class="skill"><i class="fas fa-chart-line"></i><p>Statistics</p></div>
        <div class="skill"><i class="fas fa-percentage"></i><p>Probability</p></div>
        <div class="skill"><i class="fab fa-python"></i><p>NumPy</p></div>
        <div class="skill"><i class="fab fa-python"></i><p>Pandas</p></div>
    </div>
</section>

<!-- PROJECTS -->
<section id="projects">
    <h2>Projects</h2>

    <div class="card">
        <h3>Sales Data Analysis using SQL</h3>
        <p>Analyzed sales data using SQL queries to find trends and insights.</p>
        <p><b>Tools:</b> SQL, MySQL</p>
        <div class="project-links">
            <a href="https://github.com/Yuvasreemuthusamy" target="_blank" class="btn">View on GitHub</a>
        </div>
    </div>

    <div class="card">
        <h3>Event Management Web Application</h3>
        <p>Created a web app for managing events and registrations.</p>
        <p><b>Tools:</b> HTML, CSS</p>
        <div class="project-links">
            <a href="https://github.com/Yuvasreemuthusamy" target="_blank" class="btn">View on GitHub</a>
        </div>
    </div>

    <div class="card">
        <h3>Excel Dashboard</h3>
        <p>Built dashboards to visualize KPIs and business performance.</p>
        <p><b>Tools:</b> Excel</p>
        <div class="project-links">
            <a href="https://github.com/Yuvasreemuthusamy" target="_blank" class="btn">View on GitHub</a>
        </div>
    </div>

   

</section>

<!-- CONTACT -->
<section id="contact">
    <h2>Contact</h2>

    <div class="contact-box">
        <p><b>Email:</b> yuvasree1556@gmail.com</p>
        <p><b>Phone:</b> +91 8668115413</p>

        <div class="social-icons dark">
            <a href="https://github.com/Yuvasreemuthusamy"><i class="fab fa-github"></i></a>
            <a href="https://www.linkedin.com/in/yuvasreem1556"><i class="fab fa-linkedin"></i></a>
        </div>

        <h3>Get in Touch</h3>

        <form>
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <textarea placeholder="Your Message" required></textarea>
            <button type="submit">Send Message</button>
        </form>
    </div>
</section>

<footer>
    <p>© 2026 Yuva Sree M | Data Analyst Portfolio</p>
</footer>

</body>
</html>
```

## style.css
```
/* ===== 3D BACKGROUND ===== */
body {
    margin: 0;
    font-family: 'Segoe UI', sans-serif;
    background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
    color: white;
    overflow-x: hidden;
}

/* Floating glow */
body::before, body::after {
    content: "";
    position: fixed;
    width: 350px;
    height: 350px;
    border-radius: 50%;
    filter: blur(120px);
    z-index: -1;
    animation: move 10s infinite alternate;
}

body::before {
    background: #00c6ff;
    top: -100px;
    left: -100px;
}

body::after {
    background: #ff6a00;
    bottom: -100px;
    right: -100px;
}

@keyframes move {
    from { transform: translate(0,0); }
    to { transform: translate(80px,50px); }
}

/* HERO */
.hero {
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

/* HEADINGS */
h2 {
    color: #00c6ff;
}

/* SECTION */
section {
    padding: 60px;
    text-align: center;
}

/* ABOUT */
.about-box {
    background: white;
    color: black;
    padding: 25px;
    width: 70%;
    margin: auto;
    border-radius: 15px;
}

/* SKILLS */
.skills-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 15px;
    max-width: 600px;
    margin: auto;
}

.skill {
    background: white;
    color: black;
    padding: 15px;
    border-radius: 15px;
}

/* PROJECT */
.card {
    background: white;
    color: black;
    padding: 20px;
    margin: 20px auto;
    width: 70%;
    border-radius: 15px;
}

/* BUTTON CENTER */
.project-links {
    display: flex;
    justify-content: center;
    margin-top: 10px;
}

.btn {
    background: #0072ff;
    color: white;
    padding: 8px 15px;
    border-radius: 6px;
    text-decoration: none;
}

/* CONTACT */
.contact-box {
    background: white;
    color: black;
    padding: 25px;
    width: 70%;
    margin: auto;
    border-radius: 15px;
}

/* FORM */
form input, form textarea {
    width: 80%;
    margin: 10px;
    padding: 10px;
    border-radius: 10px;
}

/* SOCIAL ICONS */
.social-icons a {
    font-size: 35px;
    margin: 10px;
    color: white;
}

.social-icons.dark a {
    color: black;
}

footer {
    text-align: center;   /* centers the text */
    padding: 15px;
}
```

## OUTPUT
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/609e43be-6732-4f7f-b366-f535e8f9d010" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/fae309c8-7464-446e-bb60-592965f6d1fb" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/62c1b08b-dc74-44c1-a15e-8b943a781009" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/16831fe0-539e-471b-9d76-4d8ae124d987" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/487ed6fb-d132-4e70-a400-2d5b1cabdedf" />



## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
