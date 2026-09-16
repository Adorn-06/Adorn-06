<!DOCTYPE html>
<html lang="en">

<head>

    <meta charset="UTF-8">

    <meta name="viewport"
          content="width=device-width, initial-scale=1.0">

    <meta name="description"
          content="Adorn Cyriac Mathew - Cybersecurity Researcher and Entry-Level SOC Analyst">

    <meta name="author"
          content="Adorn Cyriac Mathew">

    <title>
        Adorn Cyriac Mathew |
    </title>


    <style>

        /* =========================================================
           ROOT
        ========================================================= */

        :root {

            --bg: #060b14;
            --bg-soft: #0b1220;
            --card: #0d1726;
            --card-hover: #111f32;

            --primary: #38bdf8;
            --primary-dark: #0ea5e9;
            --secondary: #60a5fa;

            --green: #34d399;

            --text: #f1f5f9;
            --text-soft: #cbd5e1;
            --muted: #8fa2b8;

            --border: rgba(148,163,184,0.15);

            --shadow:
                0 20px 60px rgba(0,0,0,0.30);

            --max-width: 1180px;
        }


        /* =========================================================
           RESET
        ========================================================= */

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }


        html {
            scroll-behavior: smooth;
        }


        body {

            font-family:
                Inter,
                -apple-system,
                BlinkMacSystemFont,
                "Segoe UI",
                Roboto,
                Arial,
                sans-serif;

            color: var(--text);

            background:
                radial-gradient(
                    circle at 15% 15%,
                    rgba(56,189,248,0.08),
                    transparent 30%
                ),

                radial-gradient(
                    circle at 85% 20%,
                    rgba(96,165,250,0.06),
                    transparent 28%
                ),

                var(--bg);

            line-height: 1.6;

            overflow-x: hidden;
        }


        body::before {

            content: "";

            position: fixed;

            inset: 0;

            z-index: -2;

            background-image:

                linear-gradient(
                    rgba(56,189,248,0.025) 1px,
                    transparent 1px
                ),

                linear-gradient(
                    90deg,
                    rgba(56,189,248,0.025) 1px,
                    transparent 1px
                );

            background-size: 70px 70px;

            mask-image:
                linear-gradient(
                    to bottom,
                    black,
                    transparent 80%
                );

            pointer-events: none;
        }


        a {
            color: inherit;
            text-decoration: none;
        }


        img {
            max-width: 100%;
        }


        .container {

            width:
                min(
                    var(--max-width),
                    92%
                );

            margin: auto;
        }


        /* =========================================================
           SCROLL BAR
        ========================================================= */

        ::-webkit-scrollbar {
            width: 8px;
        }

        ::-webkit-scrollbar-track {
            background: var(--bg);
        }

        ::-webkit-scrollbar-thumb {

            background:
                rgba(56,189,248,0.35);

            border-radius: 20px;
        }


        /* =========================================================
           NAVIGATION
        ========================================================= */

        header {

            position: fixed;

            top: 0;
            left: 0;

            width: 100%;

            z-index: 1000;

            background:
                rgba(6,11,20,0.72);

            backdrop-filter:
                blur(18px);

            border-bottom:
                1px solid transparent;

            transition:
                0.3s ease;
        }


        header.scrolled {

            background:
                rgba(6,11,20,0.94);

            border-color:
                var(--border);

            box-shadow:
                0 10px 35px
                rgba(0,0,0,0.2);
        }


        .nav {

            height: 74px;

            display: flex;

            align-items: center;

            justify-content: space-between;
        }


        .logo {

            font-size: 21px;

            font-weight: 800;

            letter-spacing: -0.5px;
        }


        .logo span {
            color: var(--primary);
        }


        .nav-links {

            display: flex;

            align-items: center;

            gap: 28px;

            list-style: none;
        }


        .nav-links a {

            color: var(--muted);

            font-size: 14px;

            font-weight: 500;

            transition:
                0.25s ease;
        }


        .nav-links a:hover {

            color: var(--primary);
        }


        .nav-contact {

            padding:
                8px 14px;

            border:
                1px solid
                rgba(56,189,248,0.28);

            border-radius: 7px;

            color:
                var(--primary) !important;

            background:
                rgba(56,189,248,0.05);
        }


        /* =========================================================
           HERO
        ========================================================= */

        .hero {

            min-height: 100vh;

            display: flex;

            align-items: center;

            padding-top: 90px;

            position: relative;
        }


        .hero-grid {

            display: grid;

            grid-template-columns:
                1.15fr
                0.85fr;

            gap: 65px;

            align-items: center;
        }


        .availability {

            display: inline-flex;

            align-items: center;

            gap: 9px;

            padding:
                7px 13px;

            border-radius: 30px;

            color:
                #9be7c6;

            background:
                rgba(52,211,153,0.06);

            border:
                1px solid
                rgba(52,211,153,0.18);

            font-size: 12px;

            margin-bottom: 23px;
        }


        .status-dot {

            width: 7px;
            height: 7px;

            background:
                var(--green);

            border-radius: 50%;

            box-shadow:
                0 0 10px
                rgba(52,211,153,0.8);

            animation:
                pulse 2s infinite;
        }


        @keyframes pulse {

            0%,
            100% {
                opacity: 1;
            }

            50% {
                opacity: 0.45;
            }
        }


        .hero h1 {

            font-size:
                clamp(
                    43px,
                    6vw,
                    72px
                );

            line-height: 1.04;

            letter-spacing:
                -3px;

            margin-bottom: 17px;
        }


        .hero h1 span {
            color: var(--primary);
        }


        .hero-role {

            font-size:
                clamp(
                    21px,
                    3vw,
                    29px
                );

            color:
                var(--text-soft);

            margin-bottom: 20px;
        }


        .hero-role strong {
            color: var(--primary);
        }


        .hero-description {

            max-width: 690px;

            color:
                var(--muted);

            font-size: 16px;

            line-height: 1.85;
        }


        .hero-buttons {

            display: flex;

            flex-wrap: wrap;

            gap: 12px;

            margin-top: 30px;
        }


        .btn {

            display: inline-flex;

            align-items: center;

            justify-content: center;

            gap: 8px;

            padding:
                12px 19px;

            border-radius: 7px;

            font-size: 14px;

            font-weight: 600;

            transition:
                0.25s ease;
        }


        .btn-primary {

            background:
                linear-gradient(
                    135deg,
                    var(--primary),
                    var(--secondary)
                );

            color:
                #06101c;

            box-shadow:
                0 10px 30px
                rgba(56,189,248,0.12);
        }


        .btn-primary:hover {

            transform:
                translateY(-3px);

            box-shadow:
                0 15px 35px
                rgba(56,189,248,0.2);
        }


        .btn-secondary {

            border:
                1px solid var(--border);

            background:
                rgba(255,255,255,0.025);

            color:
                var(--text-soft);
        }


        .btn-secondary:hover {

            border-color:
                rgba(56,189,248,0.35);

            color:
                var(--primary);

            transform:
                translateY(-3px);
        }


        /* =========================================================
           HERO PROFILE CARD
        ========================================================= */

        .profile-card {

            position: relative;

            padding: 28px;

            border:
                1px solid var(--border);

            border-radius: 16px;

            background:
                linear-gradient(
                    145deg,
                    rgba(16,31,51,0.92),
                    rgba(9,20,35,0.82)
                );

            box-shadow:
                var(--shadow);

            overflow: hidden;

            animation:
                cardFloat 6s ease-in-out infinite;
        }


        @keyframes cardFloat {

            0%,
            100% {
                transform: translateY(0);
            }

            50% {
                transform: translateY(-7px);
            }
        }


        .profile-card::before {

            content: "";

            position: absolute;

            width: 220px;
            height: 220px;

            right: -120px;
            top: -120px;

            border-radius: 50%;

            background:
                rgba(56,189,248,0.08);

            filter:
                blur(10px);
        }


        .profile-top {

            display: flex;

            align-items: center;

            gap: 14px;

            padding-bottom: 20px;

            border-bottom:
                1px solid var(--border);

            margin-bottom: 20px;
        }


        .profile-icon {

            width: 52px;
            height: 52px;

            display: flex;

            align-items: center;
            justify-content: center;

            border-radius: 12px;

            background:
                rgba(56,189,248,0.09);

            border:
                1px solid
                rgba(56,189,248,0.15);

            color:
                var(--primary);

            font-size: 20px;

            font-weight: 800;
        }


        .profile-name {

            font-size: 16px;

            font-weight: 700;
        }


        .profile-role {

            font-size: 12px;

            color:
                var(--muted);
        }


        .profile-details {

            display: grid;

            gap: 14px;
        }


        .profile-row {

            display: flex;

            justify-content: space-between;

            gap: 20px;

            font-size: 13px;
        }


        .profile-row span:first-child {

            color:
                var(--muted);
        }


        .profile-row span:last-child {

            color:
                var(--text-soft);

            text-align: right;
        }


        .profile-status {

            color:
                var(--green) !important;
        }


        /* =========================================================
           SECTIONS
        ========================================================= */

        section {
            padding: 105px 0;
        }


        .section-heading {

            max-width: 720px;

            margin-bottom: 45px;
        }


        .section-label {

            color:
                var(--primary);

            text-transform:
                uppercase;

            letter-spacing:
                2px;

            font-size: 11px;

            font-weight: 700;

            margin-bottom: 10px;
        }


        .section-title {

            font-size:
                clamp(
                    30px,
                    4vw,
                    42px
                );

            line-height: 1.15;

            letter-spacing:
                -1.2px;

            margin-bottom: 13px;
        }


        .section-title span {
            color: var(--primary);
        }


        .section-description {

            color:
                var(--muted);

            max-width: 700px;
        }


        /* =========================================================
           STATS
        ========================================================= */

        .stats {

            display: grid;

            grid-template-columns:
                repeat(4,1fr);

            gap: 15px;

            margin-top: 35px;
        }


        .stat {

            padding: 23px;

            background:
                rgba(255,255,255,0.018);

            border:
                1px solid var(--border);

            border-radius: 10px;

            transition:
                0.25s ease;
        }


        .stat:hover {

            transform:
                translateY(-4px);

            border-color:
                rgba(56,189,248,0.25);
        }


        .stat-number {

            font-size: 28px;

            font-weight: 800;

            color:
                var(--primary);

            margin-bottom: 2px;
        }


        .stat-label {

            font-size: 12px;

            color:
                var(--muted);
        }


        /* =========================================================
           ABOUT
        ========================================================= */

        .about-grid {

            display: grid;

            grid-template-columns:
                1.1fr
                0.9fr;

            gap: 25px;
        }


        .about-card {

            padding: 31px;

            background:
                var(--card);

            border:
                1px solid var(--border);

            border-radius: 13px;

            box-shadow:
                var(--shadow);
        }


        .about-card p {

            color:
                var(--muted);

            line-height:
                1.85;
        }


        .focus-list {

            display: grid;

            gap: 12px;
        }


        .focus {

            display: flex;

            align-items: flex-start;

            gap: 13px;

            padding: 15px;

            background:
                rgba(255,255,255,0.018);

            border:
                1px solid var(--border);

            border-radius: 9px;

            transition:
                0.25s ease;
        }


        .focus:hover {

            border-color:
                rgba(56,189,248,0.25);

            transform:
                translateX(4px);
        }


        .focus-icon {

            width: 35px;
            height: 35px;

            display: flex;

            align-items: center;
            justify-content: center;

            flex-shrink: 0;

            border-radius: 8px;

            color:
                var(--primary);

            background:
                rgba(56,189,248,0.07);

            font-size: 12px;

            font-weight: 700;
        }


        .focus strong {

            display: block;

            font-size: 14px;

            margin-bottom: 2px;
        }


        .focus span {

            color:
                var(--muted);

            font-size: 12px;
        }


        /* =========================================================
           SKILLS
        ========================================================= */

        .skills-grid {

            display: grid;

            grid-template-columns:
                repeat(3,1fr);

            gap: 17px;
        }


        .skill-card {

            padding: 25px;

            background:
                var(--card);

            border:
                1px solid var(--border);

            border-radius: 12px;

            transition:
                0.3s ease;

            position: relative;

            overflow: hidden;
        }


        .skill-card:hover {

            transform:
                translateY(-6px);

            background:
                var(--card-hover);

            border-color:
                rgba(56,189,248,0.25);
        }


        .skill-header {

            display: flex;

            align-items: center;

            gap: 12px;

            margin-bottom: 15px;
        }


        .skill-logo {

            width: 39px;
            height: 39px;

            display: flex;

            align-items: center;
            justify-content: center;

            border-radius: 8px;

            background:
                rgba(56,189,248,0.07);

            color:
                var(--primary);

            font-size: 11px;

            font-weight: 800;

            border:
                1px solid
                rgba(56,189,248,0.12);
        }


        .skill-card h3 {

            font-size: 15px;
        }


        .skill-card p {

            color:
                var(--muted);

            font-size: 12px;

            margin-bottom: 15px;
        }


        .tags {

            display: flex;

            flex-wrap: wrap;

            gap: 7px;
        }


        .tag {

            padding:
                5px 8px;

            border-radius: 5px;

            background:
                rgba(56,189,248,0.045);

            border:
                1px solid
                rgba(56,189,248,0.11);

            color:
                #b8c8da;

            font-size: 10px;

            transition:
                0.2s ease;
        }


        .tag:hover {

            color:
                var(--primary);

            border-color:
                rgba(56,189,248,0.3);
        }


        /* =========================================================
           PROJECTS
        ========================================================= */

        .projects {

            display: grid;

            grid-template-columns:
                repeat(2,1fr);

            gap: 22px;
        }


        .project {

            padding: 29px;

            background:
                linear-gradient(
                    145deg,
                    rgba(14,29,48,0.92),
                    rgba(8,20,34,0.82)
                );

            border:
                1px solid var(--border);

            border-radius: 13px;

            position: relative;

            overflow: hidden;

            transition:
                0.3s ease;
        }


        .project:hover {

            transform:
                translateY(-6px);

            border-color:
                rgba(56,189,248,0.3);

            box-shadow:
                0 20px 50px
                rgba(0,0,0,0.22);
        }


        .project-top {

            display: flex;

            justify-content: space-between;

            align-items: center;

            margin-bottom: 20px;
        }


        .project-number {

            font-family:
                monospace;

            color:
                var(--primary);

            font-size: 11px;
        }


        .project-type {

            font-size: 10px;

            color:
                var(--muted);

            padding:
                4px 8px;

            border:
                1px solid var(--border);

            border-radius: 5px;
        }


        .project h3 {

            font-size: 21px;

            margin-bottom: 11px;
        }


        .project > p {

            color:
                var(--muted);

            font-size: 13px;

            line-height:
                1.75;

            margin-bottom: 18px;
        }


        .project-list {

            display: grid;

            gap: 8px;

            margin-bottom: 19px;
        }


        .project-list li {

            position: relative;

            padding-left: 16px;

            color:
                #aebdce;

            font-size: 12px;
        }


        .project-list li::before {

            content: "→";

            position: absolute;

            left: 0;

            color:
                var(--primary);
        }


        /* =========================================================
           TOOL SHOWCASE
        ========================================================= */

        .tool-showcase {

            display: grid;

            grid-template-columns:
                repeat(6,1fr);

            gap: 12px;

            margin-top: 30px;
        }


        .tool {

            min-height: 90px;

            display: flex;

            flex-direction: column;

            align-items: center;

            justify-content: center;

            gap: 8px;

            background:
                rgba(255,255,255,0.018);

            border:
                1px solid var(--border);

            border-radius: 9px;

            transition:
                0.25s ease;
        }


        .tool:hover {

            transform:
                translateY(-5px);

            border-color:
                rgba(56,189,248,0.3);

            background:
                rgba(56,189,248,0.035);
        }


        .tool-logo {

            width: 38px;
            height: 38px;

            display: flex;

            align-items: center;
            justify-content: center;

            color:
                var(--primary);

            background:
                rgba(56,189,248,0.07);

            border-radius: 8px;

            font-size: 10px;

            font-weight: 800;
        }


        .tool-name {

            color:
                var(--muted);

            font-size: 10px;

            text-align: center;
        }


        /* =========================================================
           CERTIFICATIONS
        ========================================================= */

        .cert-grid {

            display: grid;

            grid-template-columns:
                repeat(3,1fr);

            gap: 18px;
        }


        .cert {

            padding: 26px;

            background:
                var(--card);

            border:
                1px solid var(--border);

            border-radius: 12px;

            transition:
                0.3s ease;
        }


        .cert:hover {

            transform:
                translateY(-5px);

            border-color:
                rgba(56,189,248,0.25);
        }


        .cert-icon {

            width: 45px;
            height: 45px;

            display: flex;

            align-items: center;
            justify-content: center;

            border-radius: 9px;

            background:
                rgba(56,189,248,0.08);

            border:
                1px solid
                rgba(56,189,248,0.14);

            color:
                var(--primary);

            font-size: 12px;

            font-weight: 800;

            margin-bottom: 17px;
        }


        .cert h3 {

            font-size: 15px;

            margin-bottom: 7px;
        }


        .cert p {

            color:
                var(--muted);

            font-size: 12px;
        }


        /* =========================================================
           EDUCATION
        ========================================================= */

        .education {

            max-width: 850px;
        }


        .education-item {

            display: flex;

            gap: 20px;

            position: relative;

            padding-bottom: 35px;
        }


        .education-line {

            width: 2px;

            background:
                linear-gradient(
                    var(--primary),
                    rgba(56,189,248,0)
                );

            position: absolute;

            left: 6px;

            top: 15px;

            bottom: 0;
        }


        .education-dot {

            width: 14px;
            height: 14px;

            flex-shrink: 0;

            margin-top: 3px;

            border-radius: 50%;

            background:
                var(--bg);

            border:
                2px solid var(--primary);

            box-shadow:
                0 0 0 5px
                rgba(56,189,248,0.06);

            z-index: 2;
        }


        .education-content {

            padding:
                21px 23px;

            border:
                1px solid var(--border);

            border-radius: 10px;

            background:
                var(--card);

            flex: 1;
        }


        .education-content h3 {

            font-size: 17px;

            margin-bottom: 4px;
        }


        .education-content p {

            color:
                var(--muted);

            font-size: 13px;
        }


        /* =========================================================
           SOCIAL / CONTACT
        ========================================================= */

        .contact-box {

            text-align: center;

            padding:
                65px 25px;

            background:
                linear-gradient(
                    145deg,
                    rgba(15,31,51,0.9),
                    rgba(8,20,34,0.82)
                );

            border:
                1px solid var(--border);

            border-radius: 15px;

            overflow: hidden;

            position: relative;
        }


        .contact-box::before {

            content: "";

            position: absolute;

            width: 350px;
            height: 350px;

            top: -280px;
            left: 50%;

            transform:
                translateX(-50%);

            background:
                rgba(56,189,248,0.08);

            border-radius: 50%;

            filter:
                blur(30px);
        }


        .contact-box > * {

            position: relative;
        }


        .contact-box h2 {

            font-size:
                clamp(
                    30px,
                    4vw,
                    43px
                );

            margin-bottom: 12px;
        }


        .contact-box p {

            max-width: 650px;

            margin:
                0 auto 25px;

            color:
                var(--muted);
        }


        .social-links {

            display: flex;

            justify-content: center;

            flex-wrap: wrap;

            gap: 12px;
        }


        .social {

            display: inline-flex;

            align-items: center;

            gap: 9px;

            padding:
                10px 15px;

            border:
                1px solid var(--border);

            border-radius: 7px;

            color:
                var(--text-soft);

            font-size: 12px;

            transition:
                0.25s ease;
        }


        .social svg {

            width: 17px;
            height: 17px;

            fill:
                currentColor;
        }


        .social:hover {

            color:
                var(--primary);

            border-color:
                rgba(56,189,248,0.3);

            transform:
                translateY(-3px);
        }


        /* =========================================================
           FOOTER
        ========================================================= */

        footer {

            border-top:
                1px solid var(--border);

            padding:
                27px 0;

            text-align:
                center;

            color:
                var(--muted);

            font-size: 11px;
        }


        /* =========================================================
           REVEAL ANIMATION
        ========================================================= */

        .reveal {

            opacity: 0;

            transform:
                translateY(25px);

            transition:
                opacity 0.7s ease,
                transform 0.7s ease;
        }


        .reveal.active {

            opacity: 1;

            transform:
                translateY(0);
        }


        /* =========================================================
           RESPONSIVE
        ========================================================= */

        @media (max-width: 1000px) {

            .hero-grid,
            .about-grid {

                grid-template-columns: 1fr;
            }


            .profile-card {

                max-width: 650px;
            }


            .skills-grid {

                grid-template-columns:
                    repeat(2,1fr);
            }


            .tool-showcase {

                grid-template-columns:
                    repeat(3,1fr);
            }


            .cert-grid {

                grid-template-columns:
                    repeat(2,1fr);
            }
        }


        @media (max-width: 720px) {

            .nav-links {

                display: none;
            }


            .hero {

                padding-top: 120px;
            }


            .hero h1 {

                letter-spacing:
                    -1.8px;
            }


            .stats {

                grid-template-columns:
                    repeat(2,1fr);
            }


            .skills-grid,
            .projects,
            .cert-grid {

                grid-template-columns: 1fr;
            }


            .tool-showcase {

                grid-template-columns:
                    repeat(3,1fr);
            }


            section {

                padding:
                    75px 0;
            }
        }


        @media (max-width: 450px) {

            .stats {

                grid-template-columns: 1fr;
            }


            .tool-showcase {

                grid-template-columns:
                    repeat(2,1fr);
            }


            .hero-buttons {

                width: 100%;
            }


            .btn {

                flex: 1;
            }


            .profile-card,
            .about-card,
            .project,
            .cert {

                padding:
                    22px;
            }
        }

    </style>

</head>


<body>


<!-- =========================================================
     NAVIGATION
========================================================= -->

<header id="navbar">

    <div class="container nav">

        <a href="#home" class="logo">
            Adorn<span>.</span>
        </a>


        <nav>

            <ul class="nav-links">

                <li>
                    <a href="#about">
                        About
                    </a>
                </li>

                <li>
                    <a href="#skills">
                        Skills
                    </a>
                </li>

                <li>
                    <a href="#projects">
                        Projects
                    </a>
                </li>

                <li>
                    <a href="#certifications">
                        Certifications
                    </a>
                </li>

                <li>
                    <a href="#contact"
                       class="nav-contact">
                        Contact
                    </a>
                </li>

            </ul>

        </nav>

    </div>

</header>



<!-- =========================================================
     HERO
========================================================= -->

<main id="home">

<section class="hero">

    <div class="container hero-grid">


        <div class="reveal">

            <div class="availability">

                <span class="status-dot"></span>

                Open to Entry-Level SOC Opportunities

            </div>


            <h1>

                Adorn Cyriac
                <span>Mathew</span>

            </h1>


            <div class="hero-role">

                Cybersecurity Researcher
                <br>

                <strong>
                    Entry-Level SOC Analyst
                </strong>

            </div>


            <p class="hero-description">

                I am a cybersecurity researcher focused on
                Security Operations, SIEM monitoring, threat
                detection, log analysis and incident investigation.

                I develop practical cybersecurity skills through
                hands-on security labs involving Wazuh,
                Microsoft Sentinel, Windows security events,
                network analysis and MITRE ATT&CK.

            </p>


            <div class="hero-buttons">

                <a href="#projects"
                   class="btn btn-primary">

                    View Projects
                    →

                </a>


                <a href="#contact"
                   class="btn btn-secondary">

                    Connect With Me

                </a>

            </div>

        </div>



        <!-- PROFILE CARD -->

        <div class="profile-card reveal">


            <div class="profile-top">

                <div class="profile-icon">
                    AC
                </div>

                <div>

                    <div class="profile-name">
                        Adorn Cyriac Mathew
                    </div>

                    <div class="profile-role">
                        Cybersecurity Researcher
                    </div>

                </div>

            </div>


            <div class="profile-details">


                <div class="profile-row">

                    <span>
                        Focus
                    </span>

                    <span>
                        Security Operations
                    </span>

                </div>


                <div class="profile-row">

                    <span>
                        SIEM
                    </span>

                    <span>
                        Wazuh / Sentinel
                    </span>

                </div>


                <div class="profile-row">

                    <span>
                        OS
                    </span>

                    <span>
                        Windows / Kali Linux
                    </span>

                </div>


                <div class="profile-row">

                    <span>
                        Framework
                    </span>

                    <span>
                        MITRE ATT&CK
                    </span>

                </div>


                <div class="profile-row">

                    <span>
                        Certification
                    </span>

                    <span>
                        C|CSA
                    </span>

                </div>


                <div class="profile-row">

                    <span>
                        Status
                    </span>

                    <span class="profile-status">
                        Learning & Building
                    </span>

                </div>


            </div>

        </div>

    </div>

</section>



<!-- =========================================================
     STATS
========================================================= -->

<section style="padding-top:20px;">

    <div class="container">

        <div class="stats reveal">


            <div class="stat">

                <div class="stat-number">
                    02+
                </div>

                <div class="stat-label">
                    SIEM Projects
                </div>

            </div>


            <div class="stat">

                <div class="stat-number">
                    10+
                </div>

                <div class="stat-label">
                    Security Tools
                </div>

            </div>


            <div class="stat">

                <div class="stat-number">
                    03
                </div>

                <div class="stat-label">
                    Core Security Areas
                </div>

            </div>


            <div class="stat">

                <div class="stat-number">
                    C|CSA
                </div>

                <div class="stat-label">
                    SOC Certification
                </div>

            </div>


        </div>

    </div>

</section>



<!-- =========================================================
     ABOUT
========================================================= -->

<section id="about">

    <div class="container">


        <div class="section-heading reveal">

            <div class="section-label">
                About Me
            </div>

            <h2 class="section-title">

                Focused on building
                <span>
                    practical blue-team skills.
                </span>

            </h2>

            <p class="section-description">

                My cybersecurity learning is centered around
                understanding security monitoring, detecting
                suspicious activity and investigating security
                events through hands-on practice.

            </p>

        </div>



        <div class="about-grid">


            <div class="about-card reveal">

                <p>

                    I am a cybersecurity researcher focused on
                    Security Operations, SIEM monitoring, threat
                    detection, log analysis and incident
                    investigation.

                </p>

                <br>

                <p>

                    I am developing practical cybersecurity
                    skills through hands-on security labs and
                    projects involving Wazuh, Microsoft Sentinel,
                    Windows security events, network security
                    and the MITRE ATT&CK framework.

                </p>

                <br>

                <p>

                    My goal is to start my career in a SOC
                    environment where I can contribute to
                    security monitoring and continue developing
                    my Blue Team capabilities.

                </p>

            </div>



            <div class="focus-list reveal">


                <div class="focus">

                    <div class="focus-icon">
                        SIEM
                    </div>

                    <div>

                        <strong>
                            SIEM Monitoring
                        </strong>

                        <span>
                            Wazuh, Microsoft Sentinel,
                            Splunk and security logs.
                        </span>

                    </div>

                </div>


                <div class="focus">

                    <div class="focus-icon">
                        LOG
                    </div>

                    <div>

                        <strong>
                            Log Analysis
                        </strong>

                        <span>
                            Security event analysis and
                            event correlation.
                        </span>

                    </div>

                </div>


                <div class="focus">

                    <div class="focus-icon">
                        TD
                    </div>

                    <div>

                        <strong>
                            Threat Detection
                        </strong>

                        <span>
                            Identifying suspicious activity
                            and security alerts.
                        </span>

                    </div>

                </div>


                <div class="focus">

                    <div class="focus-icon">
                        IR
                    </div>

                    <div>

                        <strong>
                            Incident Investigation
                        </strong>

                        <span>
                            Alert investigation and
                            security analysis.
                        </span>

                    </div>

                </div>


                <div class="focus">

                    <div class="focus-icon">
                        AT
                    </div>

                    <div>

                        <strong>
                            MITRE ATT&CK
                        </strong>

                        <span>
                            Understanding attacker techniques
                            and defensive detection.
                        </span>

                    </div>

                </div>


            </div>

        </div>

    </div>

</section>



<!-- =========================================================
     SKILLS
========================================================= -->

<section id="skills">

    <div class="container">


        <div class="section-heading reveal">

            <div class="section-label">
                Skills & Technologies
            </div>

            <h2 class="section-title">

                Security tools and
                <span>
                    technologies.
                </span>

            </h2>

            <p class="section-description">

                Technologies I have studied and practiced
                through cybersecurity projects and labs.

            </p>

        </div>



        <div class="skills-grid">


            <!-- SIEM -->

            <div class="skill-card reveal">

                <div class="skill-header">

                    <div class="skill-logo">
                        SI
                    </div>

                    <h3>
                        SIEM & Monitoring
                    </h3>

                </div>

                <p>
                    Security monitoring and event analysis.
                </p>

                <div class="tags">

                    <span class="tag">
                        Wazuh
                    </span>

                    <span class="tag">
                        Microsoft Sentinel
                    </span>

                    <span class="tag">
                        Splunk
                    </span>

                    <span class="tag">
                        Sysmon
                    </span>

                    <span class="tag">
                        Windows Event Logs
                    </span>

                </div>

            </div>



            <!-- SOC -->

            <div class="skill-card reveal">

                <div class="skill-header">

                    <div class="skill-logo">
                        SOC
                    </div>

                    <h3>
                        SOC Operations
                    </h3>

                </div>

                <p>
                    Security operations and detection concepts.
                </p>

                <div class="tags">

                    <span class="tag">
                        Alert Triage
                    </span>

                    <span class="tag">
                        Alert Monitoring
                    </span>

                    <span class="tag">
                        Threat Detection
                    </span>

                    <span class="tag">
                        Incident Response
                    </span>

                    <span class="tag">
                        Event Correlation
                    </span>

                </div>

            </div>



            <!-- NETWORKING -->

            <div class="skill-card reveal">

                <div class="skill-header">

                    <div class="skill-logo">
                        NET
                    </div>

                    <h3>
                        Networking & Security
                    </h3>

                </div>

                <p>
                    Networking fundamentals used in SOC analysis.
                </p>

                <div class="tags">

                    <span class="tag">
                        TCP/IP
                    </span>

                    <span class="tag">
                        OSI Model
                    </span>

                    <span class="tag">
                        DNS
                    </span>

                    <span class="tag">
                        HTTP/HTTPS
                    </span>

                    <span class="tag">
                        Firewall
                    </span>

                    <span class="tag">
                        VPN
                    </span>

                </div>

            </div>



            <!-- TOOLS -->

            <div class="skill-card reveal">

                <div class="skill-header">

                    <div class="skill-logo">
                        SEC
                    </div>

                    <h3>
                        Security Tools
                    </h3>

                </div>

                <p>
                    Network analysis and security testing tools.
                </p>

                <div class="tags">

                    <span class="tag">
                        Wireshark
                    </span>

                    <span class="tag">
                        Nmap
                    </span>

                    <span class="tag">
                        Burp Suite
                    </span>

                    <span class="tag">
                        Metasploit
                    </span>

                    <span class="tag">
                        Nikto
                    </span>

                    <span class="tag">
                        SQLMap
                    </span>

                    <span class="tag">
                        Gobuster
                    </span>

                </div>

            </div>



            <!-- OS -->

            <div class="skill-card reveal">

                <div class="skill-header">

                    <div class="skill-logo">
                        OS
                    </div>

                    <h3>
                        Operating Systems
                    </h3>

                </div>

                <p>
                    Environments used for security labs.
                </p>

                <div class="tags">

                    <span class="tag">
                        Windows
                    </span>

                    <span class="tag">
                        Kali Linux
                    </span>

                    <span class="tag">
                        VMware
                    </span>

                    <span class="tag">
                        VirtualBox
                    </span>

                </div>

            </div>



            <!-- LANGUAGES -->

            <div class="skill-card reveal">

                <div class="skill-header">

                    <div class="skill-logo">
                        CODE
                    </div>

                    <h3>
                        Languages & Queries
                    </h3>

                </div>

                <p>
                    Programming and security query languages.
                </p>

                <div class="tags">

                    <span class="tag">
                        Python
                    </span>

                    <span class="tag">
                        C
                    </span>

                    <span class="tag">
                        SPL
                    </span>

                    <span class="tag">
                        KQL
                    </span>

                    <span class="tag">
                        SQL
                    </span>

                    <span class="tag">
                        PowerShell
                    </span>

                </div>

            </div>


        </div>

    </div>

</section>



<!-- =========================================================
     TOOL SHOWCASE
========================================================= -->

<section>

    <div class="container">


        <div class="section-heading reveal">

            <div class="section-label">
                Security Toolkit
            </div>

            <h2 class="section-title">

                Tools I work with
                <span>
                    in my labs.
                </span>

            </h2>

        </div>



        <div class="tool-showcase">


            <div class="tool reveal">

                <div class="tool-logo">
                    WZ
                </div>

                <div class="tool-name">
                    Wazuh
                </div>

            </div>


            <div class="tool reveal">

                <div class="tool-logo">
                    MS
                </div>

                <div class="tool-name">
                    Sentinel
                </div>

            </div>


            <div class="tool reveal">

                <div class="tool-logo">
                    SP
                </div>

                <div class="tool-name">
                    Splunk
                </div>

            </div>


            <div class="tool reveal">

                <div class="tool-logo">
                    SY
                </div>

                <div class="tool-name">
                    Sysmon
                </div>

            </div>


            <div class="tool reveal">

                <div class="tool-logo">
                    WS
                </div>

                <div class="tool-name">
                    Wireshark
                </div>

            </div>


            <div class="tool reveal">

                <div class="tool-logo">
                    NM
                </div>

                <div class="tool-name">
                    Nmap
                </div>

            </div>


            <div class="tool reveal">

                <div class="tool-logo">
                    BS
                </div>

                <div class="tool-name">
                    Burp Suite
                </div>

            </div>


            <div class="tool reveal">

                <div class="tool-logo">
                    MSF
                </div>

                <div class="tool-name">
                    Metasploit
                </div>

            </div>


            <div class="tool reveal">

                <div class="tool-logo">
                    PS
                </div>

                <div class="tool-name">
                    PowerShell
                </div>

            </div>


            <div class="tool reveal">

                <div class="tool-logo">
                    KL
                </div>

                <div class="tool-name">
                    Kali Linux
                </div>

            </div>


            <div class="tool reveal">

                <div class="tool-logo">
                    KQL
                </div>

                <div class="tool-name">
                    KQL
                </div>

            </div>


            <div class="tool reveal">

                <div class="tool-logo">
                    MITRE
                </div>

                <div class="tool-name">
                    ATT&CK
                </div>

            </div>


        </div>

    </div>

</section>



<!-- =========================================================
     PROJECTS
========================================================= -->

<section id="projects">

    <div class="container">


        <div class="section-heading reveal">

            <div class="section-label">
                Projects
            </div>

            <h2 class="section-title">

                Hands-on
                <span>
                    cybersecurity projects.
                </span>

            </h2>

            <p class="section-description">

                Practical labs focused on security monitoring,
                SIEM, threat detection and investigation.

            </p>

        </div>



        <div class="projects">


            <!-- WAZUH -->

            <article class="project reveal">


                <div class="project-top">

                    <span class="project-number">
                        PROJECT / 01
                    </span>

                    <span class="project-type">
                        SIEM
                    </span>

                </div>


                <h3>
                    Wazuh SIEM Monitoring Lab
                </h3>


                <p>

                    Hands-on SIEM monitoring project using
                    Wazuh and Sysmon for security event
                    monitoring, log analysis and threat detection.

                </p>


                <ul class="project-list">

                    <li>
                        Configured Wazuh for security monitoring.
                    </li>

                    <li>
                        Used Sysmon and Windows security events
                        for endpoint visibility.
                    </li>

                    <li>
                        Investigated brute-force and discovery
                        activity.
                    </li>

                    <li>
                        Implemented File Integrity Monitoring.
                    </li>

                    <li>
                        Used PowerShell for security testing
                        and telemetry generation.
                    </li>

                </ul>


                <div class="tags">

                    <span class="tag">
                        Wazuh
                    </span>

                    <span class="tag">
                        Sysmon
                    </span>

                    <span class="tag">
                        Windows
                    </span>

                    <span class="tag">
                        Kali Linux
                    </span>

                    <span class="tag">
                        FIM
                    </span>

                </div>

            </article>



            <!-- SENTINEL -->

            <article class="project reveal">


                <div class="project-top">

                    <span class="project-number">
                        PROJECT / 02
                    </span>

                    <span class="project-type">
                        CLOUD SIEM
                    </span>

                </div>


                <h3>
                    Microsoft Sentinel SOC Lab
                </h3>


                <p>

                    Microsoft Sentinel SOC laboratory focused
                    on scheduled analytics rules, Windows
                    security events, KQL-based investigation
                    and threat detection.

                </p>


                <ul class="project-list">

                    <li>
                        Configured Microsoft Sentinel for
                        security monitoring.
                    </li>

                    <li>
                        Created scheduled analytics rules.
                    </li>

                    <li>
                        Investigated Windows security events.
                    </li>

                    <li>
                        Used KQL for security event analysis.
                    </li>

                    <li>
                        Studied observed activity using
                        MITRE ATT&CK.
                    </li>

                </ul>


                <div class="tags">

                    <span class="tag">
                        Sentinel
                    </span>

                    <span class="tag">
                        KQL
                    </span>

                    <span class="tag">
                        Windows
                    </span>

                    <span class="tag">
                        Analytics Rules
                    </span>

                    <span class="tag">
                        MITRE ATT&CK
                    </span>

                </div>

            </article>



            <!-- NETWORK -->

            <article class="project reveal">


                <div class="project-top">

                    <span class="project-number">
                        PROJECT / 03
                    </span>

                    <span class="project-type">
                        NETWORK SECURITY
                    </span>

                </div>


                <h3>
                    Network Security Analysis Lab
                </h3>


                <p>

                    Practical security exercises focused on
                    network reconnaissance, packet analysis
                    and understanding common security activity.

                </p>


                <ul class="project-list">

                    <li>
                        Performed network reconnaissance with Nmap.
                    </li>

                    <li>
                        Analyzed traffic using Wireshark.
                    </li>

                    <li>
                        Studied TCP/IP and network protocols.
                    </li>

                    <li>
                        Explored security activity in isolated
                        lab environments.
                    </li>

                </ul>


                <div class="tags">

                    <span class="tag">
                        Nmap
                    </span>

                    <span class="tag">
                        Wireshark
                    </span>

                    <span class="tag">
                        TCP/IP
                    </span>

                    <span class="tag">
                        Network Security
                    </span>

                </div>

            </article>



            <!-- WINDOWS -->

            <article class="project reveal">


                <div class="project-top">

                    <span class="project-number">
                        PROJECT / 04
                    </span>

                    <span class="project-type">
                        LOG ANALYSIS
                    </span>

                </div>


                <h3>
                    Windows Security Event Analysis
                </h3>


                <p>

                    Practical analysis of Windows security
                    telemetry to understand authentication,
                    process creation and suspicious activity.

                </p>


                <ul class="project-list">

                    <li>
                        Analyzed Windows Security Event IDs.
                    </li>

                    <li>
                        Investigated failed authentication events.
                    </li>

                    <li>
                        Examined process creation telemetry.
                    </li>

                    <li>
                        Studied command execution patterns.
                    </li>

                </ul>


                <div class="tags">

                    <span class="tag">
                        Windows
                    </span>

                    <span class="tag">
                        Event Logs
                    </span>

                    <span class="tag">
                        Sysmon
                    </span>

                    <span class="tag">
                        Event Analysis
                    </span>

                </div>

            </article>


        </div>

    </div>

</section>



<!-- =========================================================
     CERTIFICATIONS
========================================================= -->

<section id="certifications">

    <div class="container">


        <div class="section-heading reveal">

            <div class="section-label">
                Certifications
            </div>

            <h2 class="section-title">

                Certifications &
                <span>
                    cybersecurity learning.
                </span>

            </h2>

        </div>



        <div class="cert-grid">


            <div class="cert reveal">

                <div class="cert-icon">
                    C|S
                </div>

                <h3>
                    EC-Council Certified SOC Analyst
                    (C|CSA)
                </h3>

                <p>

                    Professional cybersecurity certification
                    focused on SOC operations, SIEM, monitoring,
                    threat detection and incident response.

                </p>

            </div>



            <div class="cert reveal">

                <div class="cert-icon">
                    CI
                </div>

                <h3>
                    CICSA
                </h3>

                <p>

                    Cybersecurity training and practical
                    learning supporting security operations
                    and defensive security skills.

                </p>

            </div>



            <div class="cert reveal">

                <div class="cert-icon">
                    MS
                </div>

                <h3>
                    Microsoft Sentinel Training
                </h3>

                <p>

                    Hands-on learning covering Microsoft
                    Sentinel, KQL, analytics rules and
                    security monitoring.

                </p>

            </div>


        </div>

    </div>

</section>



<!-- =========================================================
     EDUCATION
========================================================= -->

<section>

    <div class="container">


        <div class="section-heading reveal">

            <div class="section-label">
                Education
            </div>

            <h2 class="section-title">

                Academic
                <span>
                    foundation.
                </span>

            </h2>

        </div>



        <div class="education">


            <div class="education-item reveal">

                <div class="education-dot"></div>

                <div class="education-line"></div>

                <div class="education-content">

                    <h3>
                        Bachelor of Computer Applications
                        (BCA)
                    </h3>

                    <p>

                        Academic foundation in computer
                        applications, programming, networking
                        and information technology.

                    </p>

                </div>

            </div>


        </div>

    </div>

</section>



<!-- =========================================================
     CAREER GOAL
========================================================= -->

<section>

    <div class="container">


        <div class="section-heading reveal">

            <div class="section-label">
                Career Goal
            </div>

            <h2 class="section-title">

                Starting a career in
                <span>
                    Security Operations.
                </span>

            </h2>

        </div>


        <div class="about-card reveal">

            <p>

                Seeking to contribute as an entry-level SOC
                Analyst and continue developing expertise in
                security monitoring, threat detection, incident
                investigation and Blue Team operations.

            </p>

        </div>

    </div>

</section>



<!-- =========================================================
     CONTACT
========================================================= -->

<section id="contact">

    <div class="container">


        <div class="contact-box reveal">


            <div class="section-label">
                Connect
            </div>


            <h2>

                Let's connect.

            </h2>


            <p>

                Interested in cybersecurity, SOC operations
                and Blue Team opportunities. Feel free to
                connect with me through the platforms below.

            </p>


            <div class="social-links">


                <!-- GITHUB -->

                <a
                    href="https://github.com/Adorn-06"
                    target="_blank"
                    class="social">

                    <svg viewBox="0 0 24 24">

                        <path d="M12 .5C5.65.5.5 5.65.5 12c0 5.09 3.29 9.4 7.86 10.92.58.1.79-.25.79-.56v-2.17c-3.2.7-3.87-1.54-3.87-1.54-.53-1.33-1.28-1.68-1.28-1.68-1.05-.72.08-.71.08-.71 1.16.08 1.77 1.19 1.77 1.19 1.03 1.77 2.7 1.26 3.36.96.1-.75.4-1.26.73-1.55-2.55-.29-5.24-1.28-5.24-5.7 0-1.26.45-2.29 1.19-3.1-.12-.29-.52-1.46.11-3.05 0 0 .97-.31 3.18 1.18a11 11 0 0 1 5.8 0c2.2-1.49 3.17-1.18 3.17-1.18.63 1.59.23 2.76.11 3.05.74.81 1.19 1.84 1.19 3.1 0 4.43-2.7 5.41-5.26 5.69.41.36.78 1.08.78 2.18v3.23c0 .31.21.67.8.56A11.51 11.51 0 0 0 23.5 12C23.5 5.65 18.35.5 12 .5Z"/>

                    </svg>

                    GitHub

                </a>



                <!-- LINKEDIN -->

                <!-- Replace the href below with your exact LinkedIn URL -->

                <a
                    href="https://www.linkedin.com/in/YOUR-LINKEDIN-USERNAME/"
                    target="_blank"
                    class="social">

                    <svg viewBox="0 0 24 24">

                        <path d="M20.45 20.45h-3.56v-5.58c0-1.33-.03-3.04-1.85-3.04-1.85 0-2.13 1.45-2.13 2.94v5.68H9.35V8.99h3.42v1.56h.05c.48-.9 1.64-1.85 3.37-1.85 3.61 0 4.28 2.38 4.28 5.48v6.27ZM5.34 7.43a2.06 2.06 0 1 1 0-4.12 2.06 2.06 0 0 1 0 4.12ZM3.56 20.45h3.57V8.99H3.56v11.46ZM22.23 0H1.77C.79 0 0 .77 0 1.72v20.56C0 23.23.79 24 1.77 24h20.46c.98 0 1.77-.77 1.77-1.72V1.72C24 .77 23.21 0 22.23 0Z"/>

                    </svg>

                    LinkedIn

                </a>


            </div>

        </div>

    </div>

</section>


</main>



<!-- =========================================================
     FOOTER
========================================================= -->

<footer>

    <div class="container">

        © 2026 Adorn Cyriac Mathew

        <br>

        Cybersecurity Researcher • Entry-Level SOC Analyst

    </div>

</footer>



<!-- =========================================================
     JAVASCRIPT
========================================================= -->

<script>


    /* =========================================================
       NAVBAR
    ========================================================= */

    const navbar =
        document.getElementById("navbar");


    window.addEventListener(
        "scroll",
        function() {

            if (window.scrollY > 40) {

                navbar.classList.add("scrolled");

            } else {

                navbar.classList.remove("scrolled");

            }

        }
    );



    /* =========================================================
       SCROLL REVEAL
    ========================================================= */

    const revealElements =
        document.querySelectorAll(".reveal");


    const observer =
        new IntersectionObserver(

            function(entries) {

                entries.forEach(
                    function(entry) {

                        if (
                            entry.isIntersecting
                        ) {

                            entry.target.classList.add(
                                "active"
                            );

                            observer.unobserve(
                                entry.target
                            );

                        }

                    }
                );

            },

            {
                threshold: 0.12
            }

        );


    revealElements.forEach(
        function(element) {

            observer.observe(element);

        }
    );


</script>


</body>

</html>
