<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
    <title>Marsh Monster – The Return of Alex Atwell | Psychological Thriller</title>
    <meta name="description" content="Official website for Marsh Monster, a psychological thriller written by Kevin B. Young. After sixteen years on the run, a guilt‑ridden fisherman returns home to face a monster who has been waiting in the marsh.">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,600;14..32,700&family=Playfair+Display:ital,wght@0,400;0,500;0,600;1,400&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: #0a0c0f;
            color: #e5e7eb;
            font-family: 'Inter', sans-serif;
            line-height: 1.5;
            scroll-behavior: smooth;
        }

        /* custom scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #1e1f22;
        }
        ::-webkit-scrollbar-thumb {
            background: #4a5b3b;
            border-radius: 4px;
        }

        /* container */
        .container {
            max-width: 1280px;
            margin: 0 auto;
            padding: 0 2rem;
        }

        /* typography */
        h1, h2, h3, .logo, .logline {
            font-family: 'Playfair Display', serif;
        }

        h2 {
            font-size: 2rem;
            letter-spacing: -0.02em;
            margin-bottom: 1.5rem;
            border-left: 4px solid #6a8a4c;
            padding-left: 1rem;
        }

        .section {
            padding: 5rem 0;
            border-bottom: 1px solid rgba(106, 138, 76, 0.2);
        }

        .section:last-of-type {
            border-bottom: none;
        }

        /* header / navbar */
        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.5rem 0;
            flex-wrap: wrap;
            gap: 1rem;
        }

        .logo {
            font-size: 1.6rem;
            font-weight: 600;
            letter-spacing: -0.01em;
            color: #c3d9a3;
        }
        .logo span {
            font-weight: 400;
            color: #9aa8b3;
        }

        .nav-links {
            display: flex;
            gap: 2rem;
        }
        .nav-links a {
            color: #e5e7eb;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.2s;
        }
        .nav-links a:hover {
            color: #c3d9a3;
        }

        /* hero */
        .hero {
            display: flex;
            flex-direction: column;
            justify-content: center;
            min-height: 80vh;
            padding: 4rem 0;
            background: radial-gradient(circle at 10% 20%, rgba(20, 30, 15, 0.6), #0a0c0f), url('data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxMDAlIiBoZWlnaHQ9IjEwMCUiPjxkZWZzPjxwYXR0ZXJuIGlkPSJhIiB3aWR0aD0iNjAiIGhlaWdodD0iNjAiIHBhdHRlcm5Vbml0cz0idXNlclNwYWNlT25Vc2UiIHBhdHRlcm5UcmFuc2Zvcm09InJvdGF0ZSgzMCkiPjxwYXRoIGQ9Ik0zMCAwIDYwIDMwIDMwIDYwIDAgMzB6IiBmaWxsPSJub25lIiBzdHJva2U9IiMyMjI4MjAiIHN0cm9rZS13aWR0aD0iMSIvPjwvcGF0dGVybj48L2RlZnM+PHJlY3Qgd2lkdGg9IjEwMCUiIGhlaWdodD0iMTAwJSIgZmlsbD0idXJsKCNhKSIvPjwvc3ZnPg==');
            background-repeat: repeat;
            background-blend-mode: overlay;
        }

        .hero-content {
            max-width: 700px;
        }

        .logline {
            font-size: 1.3rem;
            font-weight: 400;
            font-style: italic;
            margin-bottom: 1.5rem;
            color: #c3d9a3;
            border-left: 3px solid #6a8a4c;
            padding-left: 1.2rem;
        }

        .hero h1 {
            font-size: 3.8rem;
            font-weight: 600;
            line-height: 1.2;
            margin-bottom: 1rem;
        }

        .hero p {
            font-size: 1.15rem;
            color: #b9c2cc;
            margin-bottom: 2rem;
        }

        .btn {
            display: inline-block;
            background: #6a8a4c;
            color: #0a0c0f;
            padding: 0.8rem 2rem;
            border-radius: 40px;
            font-weight: 600;
            text-decoration: none;
            transition: 0.2s;
            border: none;
            cursor: pointer;
            font-family: 'Inter', sans-serif;
        }
        .btn:hover {
            background: #8aac68;
            transform: scale(1.02);
        }
        .btn-outline {
            background: transparent;
            border: 1px solid #6a8a4c;
            color: #c3d9a3;
            margin-left: 1rem;
        }
        .btn-outline:hover {
            background: #6a8a4c20;
            color: #e5e7eb;
        }

        /* two column layout */
        .two-col {
            display: flex;
            gap: 3rem;
            flex-wrap: wrap;
        }
        .col {
            flex: 1;
            min-width: 260px;
        }

        .character-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 2rem;
            margin-top: 1.5rem;
        }
        .character-card {
            background: #111316;
            border-radius: 20px;
            padding: 1.5rem;
            border-left: 3px solid #6a8a4c;
            transition: 0.2s;
        }
        .character-card h3 {
            font-size: 1.5rem;
            margin-bottom: 0.5rem;
        }
        .character-card p {
            color: #b9c2cc;
            font-size: 0.9rem;
        }

        .poster-placeholder {
            background: #1e2125;
            border-radius: 24px;
            padding: 2rem;
            text-align: center;
            border: 1px dashed #4a5b3b;
        }
        .poster-placeholder i {
            font-size: 3rem;
            display: block;
            margin-bottom: 1rem;
        }

        footer {
            padding: 2rem 0;
            text-align: center;
            font-size: 0.85rem;
            color: #6e7a8a;
            border-top: 1px solid #1e1f22;
        }

        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.4rem;
            }
            .logline {
                font-size: 1rem;
            }
            .navbar {
                flex-direction: column;
                text-align: center;
            }
            .section {
                padding: 3rem 0;
            }
            .container {
                padding: 0 1.5rem;
            }
        }
    </style>
</head>
<body>

    <div class="container">
        <nav class="navbar">
            <div class="logo">MARSH MONSTER <span>// The Return of Alex Atwell</span></div>
            <div class="nav-links">
                <a href="#story">Story</a>
                <a href="#characters">Characters</a>
                <a href="#filmmaker">Filmmaker</a>
                <a href="#contact">Contact</a>
            </div>
        </nav>
    </div>

    <section class="hero">
        <div class="container hero-content">
            <div class="logline">“After sixteen years on the run, a guilt‑ridden fisherman returns home for his mother’s funeral, finds the woman he loved and the daughter he never knew – and realizes the monster he thought he’d escaped is still waiting for him in the marsh.”</div>
            <h1>Marsh Monster<br><span style="font-size: 1.8rem;">The Return of Alex Atwell</span></h1>
            <p>A psychological thriller that blends the emotional devastation of <em>Manchester by the Sea</em> with the relentless suspense of <em>Prisoners</em>. Nicholl Fellowship recommended read.</p>
            <div>
                <a href="#contact" class="btn">Request Script</a>
                <a href="#story" class="btn btn-outline">Learn More</a>
            </div>
        </div>
    </section>

    <main>
        <!-- Story / Synopsis -->
        <section id="story" class="section">
            <div class="container">
                <h2>The Story</h2>
                <div class="two-col">
                    <div class="col">
                        <p>Alex Atwell fled his Florida hometown twenty‑five years ago after a violent blackout fight left a man dead — or so he believed. Now a hardened commercial fisherman in Alaska, he returns to Palatka for his mother’s funeral. What awaits him is more than grief.</p>
                        <p>He discovers he has a fifteen‑year‑old daughter, Alexis, and the woman he left behind, Cheyenne. As fragments of that forgotten night resurface, Alex learns the truth: he didn’t kill the man — he killed the man’s brother. And Billy Urban, the surviving brother, has spent decades living in the marsh, waiting for Alex to come home.</p>
                        <p>When Billy abducts Alexis to draw Alex into his hunting grounds, a father must recover his buried memory, confront his own guilt, and fight not just a predator — but the man he was afraid he’d become.</p>
                    </div>
                    <div class="col">
                        <div class="poster-placeholder">
                            <i>🎬</i>
                            <p style="margin-top: 0.5rem;">Poster / key art coming soon</p>
                            <small style="color:#6a7c8a;">(Replace with your film imagery)</small>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Characters -->
        <section id="characters" class="section">
            <div class="container">
                <h2>Key Characters</h2>
                <div class="character-grid">
                    <div class="character-card">
                        <h3>Alex Atwell</h3>
                        <p>Rugged, emotionally closed off. A former football star running from trauma. Arc: from self‑loathing fugitive to protective father.</p>
                    </div>
                    <div class="character-card">
                        <h3>Billy Urban</h3>
                        <p>Feral, patient, tragic. Raised in an abusive household, he hunts to fulfill a promise to his dead brother. He keeps his family’s jarred heads in a closet.</p>
                    </div>
                    <div class="character-card">
                        <h3>Alexis Robinson</h3>
                        <p>Fifteen, guarded, funny. She is not a passive victim — she fights back. Arc: from fortress to trust.</p>
                    </div>
                    <div class="character-card">
                        <h3>Cheyenne Robinson</h3>
                        <p>Fierce, resilient, hurt. Torn between protecting her daughter and lingering love for Alex.</p>
                    </div>
                    <div class="character-card">
                        <h3>Jeffrey Butts</h3>
                        <p>Police chief and childhood friend. Arc: from suspicion to belief, from cop to ally.</p>
                    </div>
                    <div class="character-card">
                        <h3>Bishop</h3>
                        <p>Therapist and keeper of a promise. Once Kirk’s fishing partner, he helps Alex recover the truth.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- filmmaker / why me -->
        <section id="filmmaker" class="section">
            <div class="container">
                <h2>About the Writer</h2>
                <div class="two-col">
                    <div class="col">
                        <p><strong>Kevin B. Young</strong> wrote <em>Marsh Monster – The Return of Alex Atwell</em> as a deeply personal psychological thriller. The story is inspired by something he witnessed in the Virginia woods forty years ago — an image that stayed with him until he finally gave it a shape and a purpose.</p>
                        <p>With a background that connects him to the atmosphere of rural Florida and the working‑class life of commercial fishing, Kevin brings authenticity and emotional weight to every page. The script has been a Nicholl Fellowship recommended read and is competition‑ready for Austin, PAGE, and Final Draft Big Break.</p>
                    </div>
                    <div class="col">
                        <blockquote style="border-left: 3px solid #6a8a4c; padding-left: 1.2rem; font-style: italic; color: #b9c2cc;">
                            “This story is inspired by something I witnessed forty years ago in the woods of Virginia. That image stayed with me until I finally gave it a shape and a purpose.”
                        </blockquote>
                    </div>
                </div>
            </div>
        </section>

        <!-- contact / representation -->
        <section id="contact" class="section">
            <div class="container">
                <h2>Contact & Representation</h2>
                <div class="two-col">
                    <div class="col">
                        <p>For script requests, producer inquiries, or festival submissions, please reach out directly.</p>
                        <p style="margin-top: 1rem;"><strong>Kevin B. Young</strong><br>
                        <a href="mailto:kevin@marshmonsterfilm.com" style="color:#c3d9a3;">kevin@marshmonsterfilm.com</a><br>
                        *replace with your real email*</p>
                        <p style="margin-top: 0.5rem;"><small>All rights reserved. © 2025 Kevin B. Young</small></p>
                    </div>
                    <div class="col">
                        <p><strong>Logline for quick pitch:</strong><br>
                        <em>After sixteen years on the run, a guilt‑ridden fisherman returns home for his mother's funeral, finds the woman he loved and the daughter he never knew – and realizes the monster he thought he'd escaped is still waiting for him in the marsh.</em></p>
                        <p style="margin-top: 1rem;"><strong>Script status:</strong> Final draft, Nicholl recommended, ready for producers and competitions.</p>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <footer>
        <div class="container">
            <p>© 2025 Kevin B. Young — MARSH MONSTER: THE RETURN OF ALEX ATWELL. All intellectual property rights reserved.</p>
            <p style="margin-top: 0.5rem;">Website designed for the film project. For inquiries, contact above.</p>
        </div>
    </footer>

    <!-- optional smooth scroll -->
    <script>
        document.querySelectorAll('.nav-links a, .btn[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                const href = this.getAttribute('href');
                if (href && href !== '#') {
                    const target = document.querySelector(href);
                    if (target) {
                        e.preventDefault();
                        target.scrollIntoView({ behavior: 'smooth' });
                    }
                }
            });
        });
    </script>
</body>
</html>
