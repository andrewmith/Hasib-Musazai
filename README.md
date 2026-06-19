# Hasib-Musazai
Portfolio
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Hasibullah Musazai | Portfolio</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<style>
:root{
    --bg:#0b1220;
    --card:#111827;
    --primary:#38bdf8;
    --text:#f8fafc;
    --muted:#94a3b8;
}

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Poppins;
    scroll-behavior:smooth;
}

body{
    background:var(--bg);
    color:var(--text);
}

/* NAV */
nav{
    position:fixed;
    top:0;
    width:100%;
    background:#0b1220ee;
    backdrop-filter:blur(10px);
    display:flex;
    justify-content:space-between;
    padding:18px 8%;
    z-index:1000;
    border-bottom:1px solid #1f2937;
}

nav h2{
    color:var(--primary);
}

nav a{
    color:var(--text);
    margin:0 12px;
    text-decoration:none;
    font-size:14px;
}

nav a:hover{
    color:var(--primary);
}

/* HERO */
.hero{
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:140px 8% 80px;
    gap:40px;
}

.hero img{
    width:320px;
    border-radius:20px;
    border:2px solid #1f2937;
}

.hero h1{
    font-size:42px;
}

.hero h3{
    color:var(--primary);
    margin-top:10px;
}

.hero p{
    margin-top:15px;
    color:var(--muted);
    max-width:600px;
}

.btn{
    display:inline-block;
    margin-top:20px;
    padding:12px 20px;
    border-radius:10px;
    background:var(--primary);
    color:black;
    text-decoration:none;
    font-weight:600;
}

/* SECTION */
section{
    padding:80px 8%;
}

.title{
    font-size:28px;
    margin-bottom:30px;
    color:var(--primary);
}

/* GRID */
.grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:20px;
}

.card{
    background:var(--card);
    padding:20px;
    border-radius:15px;
    border:1px solid #1f2937;
}

/* EXPERIENCE */
.timeline{
    border-left:2px solid var(--primary);
    padding-left:20px;
}

.item{
    margin-bottom:20px;
}

/* CONTACT */
.contact{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:20px;
}

input,textarea{
    width:100%;
    padding:12px;
    margin-top:10px;
    border-radius:8px;
    border:none;
    background:#0f172a;
    color:white;
}

footer{
    text-align:center;
    padding:30px;
    border-top:1px solid #1f2937;
    color:var(--muted);
}

/* RESPONSIVE */
@media(max-width:768px){
.hero{
    flex-direction:column;
    text-align:center;
}
.hero img{
    width:250px;
}
}
</style>
</head>

<body>

<nav>
<h2>Hasib Musazai</h2>
<div>
<a href="#about">About</a>
<a href="#skills">Skills</a>
<a href="#projects">Projects</a>
<a href="#experience">Experience</a>
<a href="#contact">Contact</a>
</div>
</nav>

<!-- HERO -->
<div class="hero">
<div>
<h1>Hasibullah Musazai</h1>
<h3>Structural Engineer • PMP® • Business Development Manager</h3>
<p>
Senior Engineering & Business Development professional with 10+ years of experience in construction,
project management, UNGM tenders, US Government contracts, and infrastructure development.
</p>
<a class="btn" href="https://www.linkedin.com/in/hasib-musazai-aa717828a">LinkedIn Profile</a>
</div>

<img src="/mnt/data/599.jpg" alt="Profile Photo">
</div>

<!-- ABOUT -->
<section id="about">
<h2 class="title">About Me</h2>
<div class="card">
Results-driven Senior Engineering & Business Development Manager with extensive experience in construction,
project management, proposal writing, contract management, and international government projects.
</div>
</section>

<!-- SKILLS -->
<section id="skills">
<h2 class="title">Core Skills</h2>
<div class="grid">

<div class="card">Structural Engineering</div>
<div class="card">Project Management</div>
<div class="card">Business Development</div>
<div class="card">UNGM Tendering</div>
<div class="card">Cost Estimation</div>
<div class="card">Contract Management</div>

</div>
</section>

<!-- PROJECTS -->
<section id="projects">
<h2 class="title">Featured Projects</h2>
<div class="grid">

<div class="card">
<h3>US Government Projects</h3>
<p>Managed execution, planning and reporting for government contracts.</p>
</div>

<div class="card">
<h3>Infrastructure Development</h3>
<p>Construction supervision, planning and delivery of infrastructure works.</p>
</div>

<div class="card">
<h3>UNGM Tender Projects</h3>
<p>Prepared technical and financial proposals for international tenders.</p>
</div>

</div>
</section>

<!-- EXPERIENCE -->
<section id="experience">
<h2 class="title">Experience</h2>
<div class="timeline">

<div class="item">Concepta Management LLC — Business Development Officer (2025-Present)</div>
<div class="item">Invest Master Construction — Construction Manager (2024-2025)</div>
<div class="item">Ural Group LLC — General Manager (2023-2025)</div>
<div class="item">Zerdic Communications — Project Manager (2023-2024)</div>
<div class="item">Fardad Logistics — Project Manager (2022-2023)</div>

</div>
</section>

<!-- CONTACT -->
<section id="contact">
<h2 class="title">Contact</h2>

<div class="contact">

<div class="card">
<p>Email: h47816mz@gmail.com</p>
<p>Phone: +93 787 088 141</p>
<p>Location: Kabul, Afghanistan</p>
<p><a href="https://www.linkedin.com/in/hasib-musazai-aa717828a">LinkedIn</a></p>
</div>

<div class="card">
<input placeholder="Your Name">
<input placeholder="Your Email">
<textarea rows="5" placeholder="Message"></textarea>
</div>

</div>
</section>

<footer>
© 2026 Hasibullah Musazai | Portfolio
</footer>

</body>
</html>
