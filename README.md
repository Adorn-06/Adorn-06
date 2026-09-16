<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Adorn Cyriac Mathew | Cybersecurity Portfolio</title>

<meta name="description"
      content="Adorn Cyriac Mathew - Cybersecurity Researcher and Entry-Level SOC Analyst">

<!--
=========================================================
GOOGLE FONT
=========================================================
-->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap"
      rel="stylesheet">


<!--
=========================================================
ICON LIBRARY
=========================================================
-->
<link rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">


<style>

/* =========================================================
   GLOBAL
========================================================= */

:root {

    --background: #030914;
    --background2: #06111f;

    --card: rgba(7, 20, 35, 0.82);

    --blue: #19a7ff;
    --cyan: #35d5ff;

    --white: #f4f8fc;
    --text: #c9d7e5;
    --muted: #8497aa;

    --border: rgba(71, 174, 255, 0.16);

    --shadow:
        0 20px 60px rgba(0,0,0,.35);

    --max-width: 1180px;
}


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
        "Inter",
        Arial,
        sans-serif;

    background:
        radial-gradient(
            circle at 80% 15%,
            rgba(0, 139, 255, .12),
            transparent 32%
        ),

        radial-gradient(
            circle at 10% 30%,
            rgba(0, 217, 255, .05),
            transparent 30%
        ),

        var(--background);

    color: var(--white);

    line-height: 1.6;

    overflow-x: hidden;
}


/*
Cyber grid
*/

body::before {

    content: "";

    position: fixed;

    inset: 0;

    pointer-events: none;

    z-index: -5;

    background-image:

        linear-gradient(
            rgba(31, 166, 255, .025) 1px,
            transparent 1px
        ),

        linear-gradient(
            90deg,
            rgba(31, 166, 255, .025) 1px,
            transparent 1px
        );

    background-size: 65px 65px;
}


body::after {

    content: "";

    position: fixed;

    width: 550px;
    height: 550px;

    right: -180px;
    top: 100px;

    background:
        radial-gradient(
            circle,
            rgba(19, 153, 255, .08),
            transparent 70%
        );

    filter: blur(20px);

    pointer-events: none;

    z-index: -4;
}


a {
    text-decoration: none;
    color: inherit;
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
   NAVIGATION
========================================================= */

header {

    position: fixed;

    top: 0;
    left: 0;

    width: 100%;

    z-index: 1000;

    background:
        rgba(3, 9, 20, .72);

    backdrop-filter:
        blur(18px);

    border-bottom:
        1px solid transparent;

    transition:
        .3s ease;
}


header.scrolled {

    border-bottom-color:
        var(--border);

    background:
        rgba(3, 9, 20, .94);
}


.nav {

    height: 72px;

    display: flex;

    align-items: center;

    justify-content: space-between;
}


.logo {

    font-size: 20px;

    font-weight: 800;

    letter-spacing: -.5px;
}


.logo span {
    color: var(--cyan);
}


.nav-links {

    display: flex;

    gap: 28px;

    list-style: none;
}


.nav-links a {

    font-size: 13px;

    color: var(--muted);

    transition: .25s ease;
}


.nav-links a:hover {

    color: var(--cyan);
}


/* =========================================================
   HERO
========================================================= */

.hero {

    min-height: 100vh;

    padding-top: 100px;

    display: flex;

    align-items: center;

    position: relative;
}


.hero-grid {

    display: grid;

    grid-template-columns:
        1.15fr
        .85fr;

    align-items: center;

    gap: 70px;
}


/* =========================================================
   PROFILE PHOTO
========================================================= */

.profile-photo {

    width: 155px;
    height: 155px;

    object-fit: cover;

    border-radius: 50%;

    border:
        3px solid
        var(--cyan);

    padding: 4px;

    background:
        #071522;

    box-shadow:
        0 0 0 8px
        rgba(35, 193, 255, .04),

        0 0 45px
        rgba(0, 175, 255, .18);

    margin-bottom: 25px;
}


/*
If you don't have a profile photo yet,
the initials version will be used.
*/

.profile-placeholder {

    width: 155px;
    height: 155px;

    display: flex;

    align-items: center;
    justify-content: center;

    border-radius: 50%;

    border:
        3px solid
        var(--cyan);

    background:
        linear-gradient(
            145deg,
            #0b2136,
            #06101c
        );

    color: var(--cyan);

    font-size: 38px;

    font-weight: 800;

    box-shadow:
        0 0 45px
        rgba(0, 175, 255, .18);

    margin-bottom: 25px;
}


/* =========================================================
   HERO TEXT
========================================================= */

.hero-label {

    display: inline-flex;

    align-items: center;

    gap: 8px;

    color: #9feaff;

    font-size: 11px;

    letter-spacing: 3px;

    text-transform: uppercase;

    margin-bottom: 15px;
}


.hero-label::before {

    content: "";

    width: 45px;

    height: 2px;

    background:
        linear-gradient(
            90deg,
            var(--blue),
            transparent
        );
}


.hero h1 {

    font-size:
        clamp(
            44px,
            6vw,
            72px
        );

    line-height: 1.02;

    letter-spacing: -3px;

    margin-bottom: 12px;
}


.hero h1 .blue {
    color: var(--blue);
}


.hero-role {

    font-size:
        clamp(
            19px,
            3vw,
            27px
        );

    color: var(--text);

    margin-bottom: 20px;
}


.hero-role strong {
    color: var(--cyan);
}


.hero-description {

    max-width: 680px;

    color: var(--muted);

    font-size: 15px;

    line-height: 1.85;
}


/* =========================================================
   SOCIAL PLATFORMS
========================================================= */

.social-links {

    display: flex;

    align-items: center;

    gap: 11px;

    margin-top: 25px;
}


.social {

    width: 44px;
    height: 44px;

    display: flex;

    align-items: center;
    justify-content: center;

    border-radius: 9px;

    background:
        rgba(255,255,255,.035);

    border:
        1px solid
        rgba(120,180,220,.18);

    color: #c9d8e7;

    font-size: 18px;

    transition:
        .3s ease;

    position: relative;
}


.social:hover {

    color: white;

    transform:
        translateY(-5px);

    border-color:
        rgba(45,200,255,.55);

    box-shadow:
        0 10px 30px
        rgba(0,160,255,.15);
}


/*
Original platform-style colors appear on hover.
*/

.github:hover {
    background: #171717;
}

.linkedin:hover {
    background: #0a66c2;
}

.email:hover {
    background: #4338ca;
}


/* =========================================================
   BUTTONS
========================================================= */

.hero-buttons {

    display: flex;

    gap: 12px;

    margin-top: 28px;

    flex-wrap: wrap;
}


.btn {

    display: inline-flex;

    align-items: center;

    gap: 8px;

    padding:
        11px 17px;

    border-radius: 7px;

    font-size: 13px;

    font-weight: 600;

    transition: .3s ease;
}


.btn-primary {

    color: #03101b;

    background:
        linear-gradient(
            135deg,
            var(--cyan),
            var(--blue)
        );
}


.btn-primary:hover {

    transform:
        translateY(-3px);

    box-shadow:
        0 12px 30px
        rgba(0,170,255,.2);
}


.btn-outline {

    color: var(--text);

    border:
        1px solid
        var(--border);

    background:
        rgba(255,255,255,.025);
}


.btn-outline:hover {

    color: var(--cyan);

    border-color:
        rgba(40,190,255,.35);

    transform:
        translateY(-3px);
}


/* =========================================================
   HERO CYBER GRAPHIC
========================================================= */

.cyber-graphic {

    position: relative;

    height: 440px;

    display: flex;

    align-items: center;

    justify-content: center;
}


.cyber-circle {

    width: 290px;
    height: 290px;

    border-radius: 50%;

    border:
        1px solid
        rgba(32,181,255,.25);

    display: flex;

    align-items: center;
    justify-content: center;

    position: relative;

    animation:
        rotate 25s linear infinite;
}


.cyber-circle::before {

    content: "";

    position: absolute;

    inset: 25px;

    border-radius: 50%;

    border:
        1px dashed
        rgba(45,195,255,.25);
}


.cyber-circle::after {

    content: "";

    position: absolute;

    inset: -20px;

    border-radius: 50%;

    border:
        1px solid
        rgba(35,160,255,.08);
}


@keyframes rotate {

    from {
        transform: rotate(0deg);
    }

    to {
        transform: rotate(360deg);
    }
}


.shield {

    width: 145px;
    height: 175px;

    clip-path:
        polygon(
            50% 0,
            92% 17%,
            88% 67%,
            50% 100%,
            12% 67%,
            8% 17%
        );

    background:
        linear-gradient(
            145deg,
            #39d9ff,
            #087de7
        );

    display: flex;

    align-items: center;
    justify-content: center;

    box-shadow:
        0 0 70px
        rgba(0,175,255,.32);
}


.shield-inner {

    width: 125px;
    height: 153px;

    clip-path:
        polygon(
            50% 0,
            92% 17%,
            88% 67%,
            50% 100%,
            12% 67%,
            8% 17%
        );

    background:
        #061321;

    display: flex;

    align-items: center;
    justify-content: center;

    color: var(--cyan);

    font-size: 58px;
}


.signal {

    position: absolute;

    width: 100%;

    height: 1px;

    background:
        linear-gradient(
            90deg,
            transparent,
            rgba(29,188,255,.35),
            transparent
        );

    transform:
        rotate(-25deg);
}


.signal.two {

    transform:
        rotate(25deg);
}


/* =========================================================
   SECTIONS
========================================================= */

section {

    padding:
        100px 0;
}


.section-label {

    color:
        var(--cyan);

    font-size: 10px;

    letter-spacing: 3px;

    text-transform: uppercase;

    font-weight: 700;

    margin-bottom: 9px;
}


.section-title {

    font-size:
        clamp(
            30px,
            4vw,
            42px
        );

    letter-spacing:
        -1.5px;

    line-height:
        1.15;

    margin-bottom: 14px;
}


.section-title span {
    color: var(--blue);
}


.section-description {

    color:
        var(--muted);

    max-width: 700px;

    font-size: 14px;
}


/* =========================================================
   ABOUT
========================================================= */

.about-grid {

    display: grid;

    grid-template-columns:
        1.1fr
        .9fr;

    gap: 25px;

    margin-top: 38px;
}


.about-card {

    padding: 32px;

    background:
        var(--card);

    border:
        1px solid
        var(--border);

    border-radius: 13px;

    box-shadow:
        var(--shadow);
}


.about-card p {

    color:
        var(--text);

    opacity: .86;

    font-size: 14px;

    line-height: 1.9;
}


/* =========================================================
   FOCUS CARDS
========================================================= */

.focus-list {

    display: grid;

    gap: 12px;
}


.focus {

    display: flex;

    align-items: center;

    gap: 14px;

    padding: 15px;

    background:
        rgba(255,255,255,.018);

    border:
        1px solid
        var(--border);

    border-radius: 9px;

    transition: .3s ease;
}


.focus:hover {

    transform:
        translateX(5px);

    border-color:
        rgba(45,195,255,.35);
}


.focus-icon {

    width: 40px;
    height: 40px;

    flex-shrink: 0;

    display: flex;

    align-items: center;
    justify-content: center;

    border-radius: 8px;

    color:
        var(--cyan);

    background:
        rgba(0,160,255,.08);
}


.focus strong {

    display: block;

    font-size: 13px;
}


.focus span {

    color:
        var(--muted);

    font-size: 11px;
}


/* =========================================================
   SKILL CARDS
========================================================= */

.skills-grid {

    display: grid;

    grid-template-columns:
        repeat(3,1fr);

    gap: 16px;

    margin-top: 40px;
}


.skill-card {

    padding: 25px;

    background:
        var(--card);

    border:
        1px solid
        var(--border);

    border-radius: 12px;

    transition:
        .3s ease;
}


.skill-card:hover {

    transform:
        translateY(-6px);

    border-color:
        rgba(45,195,255,.3);

    box-shadow:
        var(--shadow);
}


.skill-icon {

    width: 44px;
    height: 44px;

    display: flex;

    align-items: center;
    justify-content: center;

    border-radius: 9px;

    background:
        rgba(0,160,255,.07);

    color:
        var(--cyan);

    font-size: 18px;

    margin-bottom: 15px;
}


.skill-card h3 {

    font-size: 15px;

    margin-bottom: 7px;
}


.skill-card p {

    color:
        var(--muted);

    font-size: 11px;

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

    font-size: 10px;

    color:
        #b7c9d9;

    background:
        rgba(255,255,255,.025);

    border:
        1px solid
        rgba(120,170,210,.12);

    transition:
        .2s ease;
}


.tag:hover {

    color:
        var(--cyan);

    border-color:
        rgba(40,195,255,.35);
}


/* =========================================================
   TOOL LOGOS
========================================================= */

.tools-grid {

    display: grid;

    grid-template-columns:
        repeat(6,1fr);

    gap: 12px;

    margin-top: 35px;
}


.tool {

    min-height: 92px;

    display: flex;

    flex-direction: column;

    align-items: center;

    justify-content: center;

    gap: 9px;

    border:
        1px solid
        var(--border);

    background:
        rgba(255,255,255,.015);

    border-radius: 9px;

    transition:
        .3s ease;
}


.tool:hover {

    transform:
        translateY(-5px);

    background:
        rgba(15,100,160,.07);

    border-color:
        rgba(40,190,255,.3);
}


.tool i {

    font-size: 25px;

    color:
        var(--cyan);
}


.tool span {

    color:
        var(--muted);

    font-size: 10px;

    text-align: center;
}


/* =========================================================
   PROJECTS
========================================================= */

.projects {

    display: grid;

    grid-template-columns:
        repeat(2,1fr);

    gap: 20px;

    margin-top: 40px;
}


.project {

    padding: 30px;

    background:
        linear-gradient(
            145deg,
            rgba(10,28,47,.92),
            rgba(4,15,27,.85)
        );

    border:
        1px solid
        var(--border);

    border-radius: 13px;

    position: relative;

    overflow: hidden;

    transition:
        .3s ease;
}


.project::before {

    content: "";

    position: absolute;

    width: 180px;
    height: 180px;

    right: -110px;
    top: -110px;

    background:
        rgba(0,180,255,.07);

    border-radius: 50%;

    filter: blur(10px);
}


.project:hover {

    transform:
        translateY(-6px);

    border-color:
        rgba(40,190,255,.3);

    box-shadow:
        var(--shadow);
}


.project-number {

    color:
        var(--cyan);

    font-family:
        monospace;

    font-size: 10px;

    letter-spacing: 2px;
}


.project h3 {

    font-size: 20px;

    margin:
        16px 0 10px;
}


.project p {

    color:
        var(--muted);

    font-size: 12px;

    line-height: 1.8;

    margin-bottom: 17px;
}


.project-list {

    list-style: none;

    display: grid;

    gap: 8px;

    margin-bottom: 20px;
}


.project-list li {

    color:
        #aebfd0;

    font-size: 11px;

    padding-left: 15px;

    position: relative;
}


.project-list li::before {

    content: "›";

    color:
        var(--cyan);

    position: absolute;

    left: 0;
}


/* =========================================================
   CERTIFICATIONS
========================================================= */

.cert-grid {

    display: grid;

    grid-template-columns:
        repeat(3,1fr);

    gap: 17px;

    margin-top: 40px;
}


.cert {

    padding: 26px;

    background:
        var(--card);

    border:
        1px solid
        var(--border);

    border-radius: 12px;

    transition:
        .3s ease;
}


.cert:hover {

    transform:
        translateY(-5px);

    border-color:
        rgba(40,190,255,.3);
}


.cert-icon {

    width: 45px;
    height: 45px;

    display: flex;

    align-items: center;
    justify-content: center;

    border-radius: 9px;

    background:
        rgba(0,160,255,.08);

    color:
        var(--cyan);

    margin-bottom: 15px;
}


.cert h3 {

    font-size: 14px;

    margin-bottom: 7px;
}


.cert p {

    color:
        var(--muted);

    font-size: 11px;

    line-height: 1.7;
}


/* =========================================================
   EDUCATION
========================================================= */

.education-card {

    margin-top: 35px;

    padding: 28px;

    display: flex;

    align-items: center;

    gap: 20px;

    background:
        var(--card);

    border:
        1px solid
        var(--border);

    border-radius: 12px;
}


.education-icon {

    width: 55px;
    height: 55px;

    display: flex;

    align-items: center;
    justify-content: center;

    flex-shrink: 0;

    border-radius: 10px;

    background:
        rgba(0,160,255,.08);

    color:
        var(--cyan);

    font-size: 22px;
}


.education-card h3 {

    font-size: 17px;

    margin-bottom: 4px;
}


.education-card p {

    color:
        var(--muted);

    font-size: 12px;
}


/* =========================================================
   CAREER
========================================================= */

.career-box {

    margin-top: 35px;

    padding: 35px;

    border:
        1px solid
        rgba(30,180,255,.18);

    background:
        linear-gradient(
            135deg,
            rgba(10,48,75,.4),
            rgba(4,17,30,.65)
        );

    border-radius: 13px;
}


.career-box p {

    color:
        var(--text);

    font-size: 14px;

    line-height: 1.9;
}


/* =========================================================
   CONTACT
========================================================= */

.contact {

    text-align: center;
}


.contact-box {

    padding:
        65px 25px;

    background:
        linear-gradient(
            145deg,
            rgba(9,31,51,.88),
            rgba(4,15,27,.9)
        );

    border:
        1px solid
        var(--border);

    border-radius: 15px;

    position: relative;

    overflow: hidden;
}


.contact-box::before {

    content: "";

    position: absolute;

    width: 300px;
    height: 300px;

    top: -220px;

    left: 50%;

    transform:
        translateX(-50%);

    background:
        rgba(0,170,255,.09);

    border-radius: 50%;

    filter: blur(20px);
}


.contact-box h2 {

    position: relative;

    font-size:
        clamp(
            30px,
            5vw,
            45px
        );

    margin-bottom: 10px;
}


.contact-box p {

    position: relative;

    color:
        var(--muted);

    max-width: 650px;

    margin:
        0 auto 25px;

    font-size: 13px;
}


.contact .social-links {

    justify-content:
        center;

    position: relative;
}


/* =========================================================
   FOOTER
========================================================= */

footer {

    border-top:
        1px solid
        var(--border);

    padding:
        25px 0;

    text-align:
        center;

    color:
        var(--muted);

    font-size: 10px;
}


/* =========================================================
   REVEAL ANIMATION
========================================================= */

.reveal {

    opacity: 0;

    transform:
        translateY(25px);

    transition:
        opacity .7s ease,
        transform .7s ease;
}


.reveal.active {

    opacity: 1;

    transform:
        translateY(0);
}


/* =========================================================
   MOBILE
========================================================= */

@media (max-width: 1000px) {

    .hero-grid {

        grid-template-columns: 1fr;

        gap: 30px;
    }


    .cyber-graphic {

        height: 350px;
    }


    .skills-grid {

        grid-template-columns:
            repeat(2,1fr);
    }


    .tools-grid {

        grid-template-columns:
            repeat(4,1fr);
    }


    .cert-grid {

        grid-template-columns:
            repeat(2,1fr);
    }
}


@media (max-width: 700px) {

    .nav-links {

        display: none;
    }


    .hero {

        padding-top: 120px;
    }


    .hero h1 {

        letter-spacing:
            -2px;
    }


    .about-grid {

        grid-template-columns: 1fr;
    }


    .skills-grid,
    .projects,
    .cert-grid {

        grid-template-columns: 1fr;
    }


    .tools-grid {

        grid-template-columns:
            repeat(3,1fr);
    }


    section {

        padding:
            75px 0;
    }


    .cyber-graphic {

        height: 310px;
    }


    .cyber-circle {

        width: 230px;
        height: 230px;
    }


    .shield {

        width: 115px;
        height: 140px;
    }


    .shield-inner {

        width: 99px;
        height: 121px;
    }
}


@media (max-width: 430px) {

    .tools-grid {

        grid-template-columns:
            repeat(2,1fr);
    }


    .profile-photo,
    .profile-placeholder {

        width: 125px;
        height: 125px;
    }


    .hero-buttons {

        width: 100%;
    }


    .btn {

        flex: 1;
    }


    .about-card,
    .project,
    .cert {

        padding: 22px;
    }
}

</style>
</head>


<body>


<!-- =========================================================
     NAVIGATION
========================================================= -->

<header id="header">

<div class="container nav">

    <a href="#home" class="logo">
        Adorn<span>.</span>
    </a>


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
            <a href="#contact">
                Contact
            </a>
        </li>

    </ul>

</div>

</header>



<!-- =========================================================
     HERO
========================================================= -->

<section class="hero" id="home">

<div class="container hero-grid">


    <!-- LEFT -->

    <div class="reveal">


        <!--
        =====================================================
        PROFILE PHOTO

        Put your image in the repository as:

        profile.jpg

        Then replace the placeholder below with:

        <img src="profile.jpg"
             class="profile-photo"
             alt="Adorn Cyriac Mathew">

        =====================================================
        -->

        <div class="profile-placeholder">
            AC
        </div>


        <div class="hero-label">

            SECURITY /
            MONITOR /
            INVESTIGATE /
            PROTECT

        </div>


        <h1>

            Adorn
            <span class="blue">
                Cyriac Mathew
            </span>

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
            network security and the MITRE ATT&CK framework.

        </p>


        <!-- SOCIAL PLATFORMS -->

        <div class="social-links">


            <!-- GitHub -->

            <a
                href="https://github.com/Adorn-06"
                target="_blank"
                rel="noopener noreferrer"
                class="social github"
                aria-label="GitHub">

                <i class="fa-brands fa-github"></i>

            </a>


            <!-- LinkedIn -->

            <!--
            Replace YOUR-LINKEDIN-USERNAME
            with your actual LinkedIn username.
            -->

            <a
                href="https://www.linkedin.com/in/YOUR-LINKEDIN-USERNAME/"
                target="_blank"
                rel="noopener noreferrer"
                class="social linkedin"
                aria-label="LinkedIn">

                <i class="fa-brands fa-linkedin-in"></i>

            </a>


            <!-- Email -->

            <a
                href="mailto:YOUR-EMAIL@example.com"
                class="social email"
                aria-label="Email">

                <i class="fa-solid fa-envelope"></i>

            </a>


        </div>


        <div class="hero-buttons">

            <a
                href="#projects"
                class="btn btn-primary">

                <i class="fa-solid fa-shield-halved"></i>

                View Projects

            </a>


            <a
                href="#contact"
                class="btn btn-outline">

                Connect With Me

            </a>

        </div>

    </div>



    <!-- RIGHT CYBER GRAPHIC -->

    <div class="cyber-graphic reveal">


        <div class="signal"></div>

        <div class="signal two"></div>


        <div class="cyber-circle">

            <div class="shield">

                <div class="shield-inner">

                    <i class="fa-solid fa-lock"></i>

                </div>

            </div>

        </div>

    </div>


</div>

</section>



<!-- =========================================================
     ABOUT ME
========================================================= -->

<section id="about">

<div class="container">


    <div class="section-label reveal">
        About Me
    </div>


    <h2 class="section-title reveal">

        Building practical
        <span>
            Blue Team skills.
        </span>

    </h2>


    <p class="section-description reveal">

        My cybersecurity learning is centered around
        security monitoring, threat detection and
        investigation.

    </p>


    <div class="about-grid">


        <div class="about-card reveal">

            <p>

                I am a BCA graduate and EC-Council Certified
                SOC Analyst (C|CSA) focused on developing
                practical skills in Security Operations,
                SIEM monitoring, threat detection, log analysis
                and incident investigation.

            </p>

            <br>

            <p>

                I build hands-on cybersecurity labs to strengthen
                my understanding of Blue Team operations,
                Windows security telemetry, security event
                analysis and the MITRE ATT&CK framework.

            </p>

            <br>

            <p>

                My goal is to contribute as an entry-level
                SOC Analyst while continuing to develop my
                skills in security monitoring, threat detection
                and incident investigation.

            </p>

        </div>



        <div class="focus-list reveal">


            <div class="focus">

                <div class="focus-icon">
                    <i class="fa-solid fa-chart-line"></i>
                </div>

                <div>

                    <strong>
                        SIEM Monitoring
                    </strong>

                    <span>
                        Wazuh, Microsoft Sentinel and Splunk
                    </span>

                </div>

            </div>


            <div class="focus">

                <div class="focus-icon">
                    <i class="fa-solid fa-magnifying-glass"></i>
                </div>

                <div>

                    <strong>
                        Log Analysis
                    </strong>

                    <span>
                        Windows security events and event correlation
                    </span>

                </div>

            </div>


            <div class="focus">

                <div class="focus-icon">
                    <i class="fa-solid fa-bug"></i>
                </div>

                <div>

                    <strong>
                        Threat Detection
                    </strong>

                    <span>
                        Detection and investigation of suspicious activity
                    </span>

                </div>

            </div>


            <div class="focus">

                <div class="focus-icon">
                    <i class="fa-solid fa-triangle-exclamation"></i>
                </div>

                <div>

                    <strong>
                        Alert Investigation
                    </strong>

                    <span>
                        Alert monitoring and security analysis
                    </span>

                </div>

            </div>


            <div class="focus">

                <div class="focus-icon">
                    <i class="fa-solid fa-shield-halved"></i>
                </div>

                <div>

                    <strong>
                        MITRE ATT&CK
                    </strong>

                    <span>
                        Understanding attacker techniques
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


    <div class="section-label reveal">
        Skills & Technologies
    </div>


    <h2 class="section-title reveal">

        Security tools &
        <span>
            technologies.
        </span>

    </h2>


    <p class="section-description reveal">

        Technologies and concepts practiced through
        cybersecurity labs and projects.

    </p>


    <div class="skills-grid">


        <!-- SIEM -->

        <div class="skill-card reveal">

            <div class="skill-icon">

                <i class="fa-solid fa-server"></i>

            </div>

            <h3>
                SIEM & Security Monitoring
            </h3>

            <p>
                Security monitoring and event analysis.
            </p>

            <div class="tags">

                <span class="tag">Wazuh</span>

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

            <div class="skill-icon">

                <i class="fa-solid fa-shield-halved"></i>

            </div>

            <h3>
                SOC Operations
            </h3>

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

            <div class="skill-icon">

                <i class="fa-solid fa-network-wired"></i>

            </div>

            <h3>
                Networking & Security
            </h3>

            <p>
                Networking fundamentals for security analysis.
            </p>

            <div class="tags">

                <span class="tag">TCP/IP</span>

                <span class="tag">OSI Model</span>

                <span class="tag">DNS</span>

                <span class="tag">HTTP/HTTPS</span>

                <span class="tag">Firewall</span>

                <span class="tag">VPN</span>

                <span class="tag">Packet Analysis</span>

            </div>

        </div>



        <!-- SECURITY TOOLS -->

        <div class="skill-card reveal">

            <div class="skill-icon">

                <i class="fa-solid fa-screwdriver-wrench"></i>

            </div>

            <h3>
                Security Tools
            </h3>

            <p>
                Security testing and network analysis.
            </p>

            <div class="tags">

                <span class="tag">Wireshark</span>

                <span class="tag">Nmap</span>

                <span class="tag">Burp Suite</span>

                <span class="tag">Metasploit</span>

                <span class="tag">Nikto</span>

                <span class="tag">SQLMap</span>

                <span class="tag">Gobuster</span>

                <span class="tag">Hydra</span>

            </div>

        </div>



        <!-- OS -->

        <div class="skill-card reveal">

            <div class="skill-icon">

                <i class="fa-solid fa-desktop"></i>

            </div>

            <h3>
                Operating Systems
            </h3>

            <p>
                Environments used for security labs.
            </p>

            <div class="tags">

                <span class="tag">Windows</span>

                <span class="tag">Kali Linux</span>

                <span class="tag">VMware</span>

                <span class="tag">VirtualBox</span>

            </div>

        </div>



        <!-- LANGUAGES -->

        <div class="skill-card reveal">

            <div class="skill-icon">

                <i class="fa-solid fa-code"></i>

            </div>

            <h3>
                Languages & Query Languages
            </h3>

            <p>
                Programming and security query languages.
            </p>

            <div class="tags">

                <span class="tag">Python</span>

                <span class="tag">C</span>

                <span class="tag">PowerShell</span>

                <span class="tag">SQL</span>

                <span class="tag">SPL</span>

                <span class="tag">KQL</span>

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


    <div class="section-label reveal">
        Security Toolkit
    </div>


    <h2 class="section-title reveal">

        Tools used in my
        <span>
            cybersecurity labs.
        </span>

    </h2>


    <div class="tools-grid">


        <div class="tool reveal">

            <i class="fa-solid fa-shield"></i>

            <span>Wazuh</span>

        </div>


        <div class="tool reveal">

            <i class="fa-brands fa-microsoft"></i>

            <span>
                Microsoft Sentinel
            </span>

        </div>


        <div class="tool reveal">

            <i class="fa-solid fa-chart-column"></i>

            <span>Splunk</span>

        </div>


        <div class="tool reveal">

            <i class="fa-solid fa-wave-square"></i>

            <span>Sysmon</span>

        </div>


        <div class="tool reveal">

            <i class="fa-solid fa-globe"></i>

            <span>Wireshark</span>

        </div>


        <div class="tool reveal">

            <i class="fa-solid fa-network-wired"></i>

            <span>Nmap</span>

        </div>


        <div class="tool reveal">

            <i class="fa-solid fa-bug"></i>

            <span>Burp Suite</span>

        </div>


        <div class="tool reveal">

            <i class="fa-solid fa-skull-crossbones"></i>

            <span>Metasploit</span>

        </div>


        <div class="tool reveal">

            <i class="fa-brands fa-windows"></i>

            <span>Windows</span>

        </div>


        <div class="tool reveal">

            <i class="fa-brands fa-linux"></i>

            <span>Kali Linux</span>

        </div>


        <div class="tool reveal">

            <i class="fa-brands fa-python"></i>

            <span>Python</span>

        </div>


        <div class="tool reveal">

            <i class="fa-solid fa-terminal"></i>

            <span>PowerShell</span>

        </div>


        <div class="tool reveal">

            <i class="fa-solid fa-database"></i>

            <span>SQL</span>

        </div>


        <div class="tool reveal">

            <i class="fa-solid fa-code"></i>

            <span>KQL</span>

        </div>


        <div class="tool reveal">

            <i class="fa-solid fa-crosshairs"></i>

            <span>MITRE ATT&CK</span>

        </div>


        <div class="tool reveal">

            <i class="fa-solid fa-server"></i>

            <span>VMware</span>

        </div>


    </div>

</div>

</section>



<!-- =========================================================
     PROJECTS
========================================================= -->

<section id="projects">

<div class="container">


    <div class="section-label reveal">
        Projects
    </div>


    <h2 class="section-title reveal">

        Hands-on
        <span>
            cybersecurity labs.
        </span>

    </h2>


    <p class="section-description reveal">

        Practical projects focused on SIEM monitoring,
        security events, threat detection and investigation.

    </p>


    <div class="projects">


        <!-- WAZUH -->

        <article class="project reveal">

            <div class="project-number">
                PROJECT / 01
            </div>


            <h3>
                Wazuh SIEM Monitoring Lab
            </h3>


            <p>

                Hands-on SIEM monitoring project using Wazuh
                and Sysmon for security event monitoring,
                log analysis and threat detection.

            </p>


            <ul class="project-list">

                <li>
                    Wazuh SIEM security monitoring
                </li>

                <li>
                    Sysmon endpoint telemetry
                </li>

                <li>
                    Windows security event analysis
                </li>

                <li>
                    Brute-force detection
                </li>

                <li>
                    Discovery activity investigation
                </li>

                <li>
                    File Integrity Monitoring
                </li>

                <li>
                    PowerShell security testing
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

            <div class="project-number">
                PROJECT / 02
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
                    Microsoft Sentinel security monitoring
                </li>

                <li>
                    Scheduled analytics rules
                </li>

                <li>
                    Windows security events
                </li>

                <li>
                    KQL-based investigation
                </li>

                <li>
                    Security alert analysis
                </li>

                <li>
                    MITRE ATT&CK mapping
                </li>

            </ul>


            <div class="tags">

                <span class="tag">
                    Microsoft Sentinel
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



        <!-- NETWORK SECURITY -->

        <article class="project reveal">

            <div class="project-number">
                PROJECT / 03
            </div>


            <h3>
                Network Security Analysis Lab
            </h3>


            <p>

                Practical security exercises involving
                network reconnaissance, packet analysis
                and network security fundamentals.

            </p>


            <ul class="project-list">

                <li>
                    Network reconnaissance using Nmap
                </li>

                <li>
                    Packet analysis using Wireshark
                </li>

                <li>
                    TCP/IP analysis
                </li>

                <li>
                    Network protocol investigation
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

            <div class="project-number">
                PROJECT / 04
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
                    Windows Security Event analysis
                </li>

                <li>
                    Failed authentication investigation
                </li>

                <li>
                    Process creation telemetry
                </li>

                <li>
                    Command execution analysis
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


    <div class="section-label reveal">
        Certifications
    </div>


    <h2 class="section-title reveal">

        Certifications &
        <span>
            training.
        </span>

    </h2>


    <div class="cert-grid">


        <div class="cert reveal">

            <div class="cert-icon">

                <i class="fa-solid fa-certificate"></i>

            </div>


            <h3>
                EC-Council Certified SOC Analyst (C|CSA)
            </h3>


            <p>

                Certification focused on SOC operations,
                SIEM, monitoring, threat detection and
                incident response.

            </p>

        </div>



        <div class="cert reveal">

            <div class="cert-icon">

                <i class="fa-solid fa-shield-halved"></i>

            </div>


            <h3>
                CICSA
            </h3>


            <p>

                Cybersecurity training and practical
                learning supporting defensive security
                skills.

            </p>

        </div>



        <div class="cert reveal">

            <div class="cert-icon">

                <i class="fa-brands fa-microsoft"></i>

            </div>


            <h3>
                Microsoft Sentinel Training
            </h3>


            <p>

                Training focused on Microsoft Sentinel,
                KQL, analytics rules and security monitoring.

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


    <div class="section-label reveal">
        Education
    </div>


    <h2 class="section-title reveal">

        Academic
        <span>
            foundation.
        </span>

    </h2>


    <div class="education-card reveal">


        <div class="education-icon">

            <i class="fa-solid fa-graduation-cap"></i>

        </div>


        <div>

            <h3>
                Bachelor of Computer Applications (BCA)
            </h3>

            <p>

                Academic foundation in computer applications,
                programming, networking and information technology.

            </p>

        </div>


    </div>

</div>

</section>



<!-- =========================================================
     CAREER GOAL
========================================================= -->

<section>

<div class="container">


    <div class="section-label reveal">
        Career Goal
    </div>


    <h2 class="section-title reveal">

        Beginning my journey in
        <span>
            Security Operations.
        </span>

    </h2>


    <div class="career-box reveal">

        <p>

            Seeking to contribute as an
            <strong>
                entry-level SOC Analyst
            </strong>
            and continue developing expertise in
            security monitoring, threat detection,
            incident investigation and Blue Team operations.

        </p>

    </div>

</div>

</section>



<!-- =========================================================
     CONTACT
========================================================= -->

<section id="contact" class="contact">

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
            and Blue Team opportunities. Connect with me
            through the platforms below.

        </p>


        <div class="social-links">


            <!-- GitHub -->

            <a
                href="https://github.com/Adorn-06"
                target="_blank"
                rel="noopener noreferrer"
                class="social github">

                <i class="fa-brands fa-github"></i>

            </a>


            <!-- LinkedIn -->

            <a
                href="https://www.linkedin.com/in/YOUR-LINKEDIN-USERNAME/"
                target="_blank"
                rel="noopener noreferrer"
                class="social linkedin">

                <i class="fa-brands fa-linkedin-in"></i>

            </a>


            <!-- Email -->

            <a
                href="mailto:YOUR-EMAIL@example.com"
                class="social email">

                <i class="fa-solid fa-envelope"></i>

            </a>


        </div>

    </div>

</div>

</section>



<!-- =========================================================
     FOOTER
========================================================= -->

<footer>

<div class="container">

    © 2026 Adorn Cyriac Mathew

    <br>

    Cybersecurity Researcher
    •
    Entry-Level SOC Analyst

</div>

</footer>



<!-- =========================================================
     JAVASCRIPT
========================================================= -->

<script>


/* =========================================================
   NAVBAR SCROLL
========================================================= */

const header =
    document.getElementById("header");


window.addEventListener(
    "scroll",
    () => {

        if (window.scrollY > 40) {

            header.classList.add("scrolled");

        } else {

            header.classList.remove("scrolled");

        }

    }
);


/* =========================================================
   SCROLL REVEAL
========================================================= */

const elements =
    document.querySelectorAll(".reveal");


const observer =
    new IntersectionObserver(

        entries => {

            entries.forEach(
                entry => {

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


elements.forEach(
    element => {

        observer.observe(element);

    }
);


</script>


</body>
</html>
