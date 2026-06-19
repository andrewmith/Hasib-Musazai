# Hasib-Musazai
Portfolio
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hasibullah Musazai | Portfolio</title>
    <!-- FontAwesome for professional icons -->
    <link rel="stylesheet" href="https://cloudflare.com">
    <style>
        :root {
            --bg: #0b1220;
            --card: #111827;
            --primary: #38bdf8;
            --text: #1f2937;
            --text-light: #f8fafc;
            --muted: #94a3b8;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
            scroll-behavior: smooth;
        }

        body {
            background-color: var(--bg);
            color: var(--text-light);
            line-height: 1.6;
        }

        /* NAVBAR SECTION */
        nav {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(11, 18, 32, 0.8);
            backdrop-filter: blur(10px);
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 18px 8%;
            z-index: 1000;
            border-bottom: 1px solid #1f2937;
        }

        nav h2 {
            color: var(--text-light);
            font-size: 20px;
            font-weight: 600;
        }

        nav h2 span {
            color: var(--primary);
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 30px;
        }

        nav a {
            color: var(--muted);
            text-decoration: none;
            font-size: 14px;
            font-weight: 500;
            transition: 0.3s;
        }

        nav a:hover, nav a.active {
            color: var(--primary);
        }

        /* HERO SECTION */
        .hero {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 160px 8% 80px 8%;
            gap: 40px;
            min-height: 90vh;
        }

        .hero-content {
            max-width: 600px;
        }

        .hero h3 {
            color: var(--primary);
            font-size: 18px;
            font-weight: 500;
            margin-bottom: 10px;
        }

        .hero h1 {
            font-size: 48px;
            font-weight: 700;
            line-height: 1.2;
            margin-bottom: 10px;
        }

        .hero h4 {
            font-size: 22px;
            color: var(--muted);
            font-weight: 500;
            margin-bottom: 20px;
        }

        .hero p {
            color: var(--muted);
            margin-bottom: 30px;
            font-size: 16px;
        }

        .btn-container {
            display: flex;
            gap: 15px;
        }

        .btn {
            display: inline-block;
            padding: 12px 28px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 500;
            font-size: 15px;
            transition: 0.3s;
        }

        .btn-primary {
            background: var(--primary);
            color: #000;
        }

        .btn-primary:hover {
            background: #7dd3fc;
            box-shadow: 0 0 15px rgba(56, 189, 248, 0.4);
        }

        .btn-outline {
            border: 2px solid var(--primary);
            color: var(--primary);
        }

        .btn-outline:hover {
            background: rgba(56, 189, 248, 0.1);
        }

        .hero-img-container {
            position: relative;
        }

        .hero img {
            width: 340px;
            height: 340px;
            border-radius: 50%;
            object-fit: cover;
            border: 4px solid var(--primary);
            box-shadow: 0 0 25px rgba(56, 189, 248, 0.2);
        }

        /* GENERAL SECTION STYLING */
        section {
            padding: 90px 8%;
        }

        .section-title {
            text-align: center;
            margin-bottom: 50px;
        }

        .section-title p {
            color: var(--primary);
            font-size: 14px;
            text-transform: uppercase;
            letter-spacing: 2px;
            margin-bottom: 5px;
        }

        .section-title h2 {
            font-size: 32px;
            font-weight: 700;
        }

        /* ABOUT SECTION & COUNTERS */
        .about-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 40px;
        }

        .about-text {
            text-align: center;
            max-width: 800px;
            font-size: 16px;
            color: var(--muted);
        }

        .counter-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
            width: 100%;
            max-width: 800px;
            margin-top: 20px;
        }

        .counter-card {
            background: var(--card);
            border: 1px solid #1f2937;
            border-radius: 12px;
            padding: 25px;
            text-align: center;
        }

        .counter-card h3 {
            color: var(--primary);
            font-size: 32px;
            margin-bottom: 5px;
        }

        .counter-card p {
            color: var(--muted);
            font-size: 14px;
        }

        /* SKILLS GRID */
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
        }

        .card {
            background: var(--card);
            border: 1px solid #1f2937;
            border-radius: 12px;
            padding: 30px 25px;
            transition: 0.3s;
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        .card:hover {
            transform: translateY(-5px);
            border-color: var(--primary);
        }

        .card-icon {
            font-size: 35px;
            color: var(--primary);
        }

        .card h3 {
            font-size: 20px;
            font-weight: 600;
        }

        .card p {
            color: var(--muted);
            font-size: 14px;
        }

        .badge {
            align-self: flex-start;
            background: rgba(56, 189, 248, 0.1);
            color: var(--primary);
            padding: 4px 12px;
            border-radius: 20px;
            font-size: 12px;
            font-weight: 500;
        }

        /* PROJECTS SECTION */
        .project-card {
            background: var(--card);
            border: 1px solid #1f2937;
            border-radius: 12px;
            overflow: hidden;
            transition: 0.3s;
        }

        .project-card:hover {
            transform: translateY(-5px);
            border-color: var(--primary);
        }

        .project-img {
            width: 100%;
            height: 200px;
            background: #1e293b;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #475569;
            font-size: 40px;
        }

        .project-info {
            padding: 25px;
        }

        .project-info h3 {
            font-size: 19px;
            margin-bottom: 10px;
        }

        .project-info p {
            color: var(--muted);
            font-size: 14px;
            margin-bottom: 15px;
        }

        .tag-container {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }

        .tag {
            background: #1e293b;
            color: #94a3b8;
            padding: 3px 10px;
            border-radius: 4px;
            font-size: 11px;
        }

        /* CONTACT SECTION */
        .contact-info-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
            margin-bottom: 40px;
        }

        .contact-box {
            background: var(--card);
            border: 1px solid #1f2937;
            border-radius: 12px;
            padding: 25px;
            text-align: center;
        }

        .contact-box i {
            font-size: 24px;
            color: var(--primary);
            margin-bottom: 10px;
        }

        .contact-box h4 {
            margin-bottom: 5px;
            font-size: 16px;
        }

        .contact-box p {
            color: var(--muted);
            font-size: 14px;
        }

        form {
            display: flex;
            flex-direction: column;
            gap: 15px;
            max-width: 700px;
            margin: 0 auto;
        }

        input, textarea {
            width: 100%;
            padding: 14px;
            background: var(--card);
            border: 1px solid #1f2937;
            border-radius: 8px;
            color: var(--text-light);
            font-size: 15px;
            outline: none;
        }

        input:focus, textarea:focus {
            border-color: var(--primary);
        }

        form .btn-submit {
            background: var(--primary);
            color: #000;
            border: none;
            cursor: pointer;
            font-weight: 600;
            padding: 14px;
            border-radius: 8px;
            transition: 0.3s;
        }

        form .btn-submit:hover {
            background: #7dd3fc;
        }

        /* FOOTER */
        footer {
            border-top: 1px solid #1f2937;
            padding: 40px 8% 20px 8%;
            background: #090f1a;
        }

        .footer-content {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
            gap: 30px;
            margin-bottom: 30px;
        }

        .footer-brand {
            max-width: 300px;
        }

        .footer-brand h3 {
            margin-bottom: 10px;
        }

        .footer-brand p {
            color: var(--muted);
            font-size: 14px;
        }


</html>
