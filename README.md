<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>★ Xx_MUSIC_UPDATES_2006_xX ★</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Courier+Prime:ital,wght@0,400;0,700;1,400;1,700&family=Syne:wght@700;800&display=swap" rel="stylesheet">
    
    <style>
        /* --- Y2K MYSPACE RESET & VARIABLES --- */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        :root {
            --hot-pink: #ff007f;
            --neon-pink: #ff66b2;
            --dark-black: #0d0d0d;
            --goth-black: #1a1a1a;
            --silver-stud: #cccccc;
            --silver-dark: #777777;
        }

        body {
            background-color: var(--dark-black);
            /* Retro Y2K Vector Flourish / Grid Inspired Background Pattern */
            background-image: 
                linear-gradient(90deg, rgba(255, 0, 127, 0.05) 1px, transparent 1px),
                linear-gradient(rgba(255, 0, 127, 0.05) 1px, transparent 1px),
                radial-gradient(circle at 20% 20%, var(--goth-black) 0%, transparent 40%),
                radial-gradient(circle at 80% 80%, rgba(255, 0, 127, 0.15) 0%, transparent 50%);
            background-size: 20px 20px, 20px 20px, 100% 100%, 100% 100%;
            font-family: 'Courier Prime', monospace;
            color: #ffffff;
            padding: 10px;
            overflow-x: hidden;
        }

        /* --- CUSTOM STUDDED BORDER UTILITY --- */
        .studded-box {
            background: var(--goth-black);
            border: 4px solid var(--hot-pink);
            /* Dotted outline mimicking a row of silver studs/rhinestones */
            outline: 3px dotted var(--silver-stud);
            outline-offset: 2px;
            box-shadow: 0px 0px 15px var(--hot-pink);
            margin-bottom: 25px;
            padding: 20px;
            position: relative;
        }

        /* Decorative Vector Flourish Corners (CSS Simulated) */
        .studded-box::before, .studded-box::after {
            content: "❦";
            position: absolute;
            color: var(--hot-pink);
            font-size: 1.5rem;
            opacity: 0.7;
        }
        .studded-box::before { top: 5px; left: 5px; }
        .studded-box::after { bottom: 5px; right: 5px; }

        /* --- HEADER SECTION --- */
        header {
            text-align: center;
            padding: 30px 10px;
            background: linear-gradient(180deg, var(--dark-black) 0%, #260013 100%);
        }

        header h1 {
            font-family: 'Syne', sans-serif;
            font-weight: 800;
            font-size: 2.8rem;
            color: #ffffff;
            text-transform: uppercase;
            text-shadow: 3px 3px 0px var(--hot-pink), -1px -1px 0px var(--silver-stud);
            letter-spacing: -1px;
            margin-bottom: 10px;
        }

        header p {
            color: var(--neon-pink);
            font-weight: bold;
            font-size: 1.1rem;
            text-shadow: 1px 1px 0px #000;
        }

        /* --- BLING BLING MARQUEE --- */
        .ticker {
            background: var(--hot-pink);
            color: #000;
            font-weight: bold;
            padding: 5px 0;
            margin-bottom: 25px;
            border-top: 2px solid var(--silver-stud);
            border-bottom: 2px solid var(--silver-stud);
        }

        /* --- LAYOUT CONTAINER --- */
        .container {
            max-width: 1000px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 1fr;
            gap: 20px;
        }

        @media (min-width: 768px) {
            .container {
                grid-template-columns: 2fr 1fr;
            }
        }

        /* --- MAIN SECTION (UPDATES) --- */
        .main-content h2 {
            font-family: 'Syne', sans-serif;
            font-size: 1.8rem;
            color: #000;
            background: var(--hot-pink);
            padding: 5px 10px;
            margin-top: -20px;
            margin-left: -20px;
            margin-right: -20px;
            margin-bottom: 20px;
            border-bottom: 3px solid var(--silver-stud);
            display: flex;
            justify-content: space-between;
        }

        .news-post {
            border-bottom: 2px dashed rgba(255, 0, 127, 0.4);
            padding-bottom: 20px;
            margin-bottom: 20px;
        }

        .news-post:last-child {
            border-bottom: none;
            margin-bottom: 0;
            padding-bottom: 0;
        }

        .news-post h3 {
            color: var(--neon-pink);
            font-size: 1.4rem;
            margin-bottom: 5px;
        }

        .date {
            font-size: 0.8rem;
            color: var(--silver-stud);
            margin-bottom: 12px;
            display: block;
        }

        .news-post p {
            line-height: 1.6;
            font-size: 0.95rem;
        }

        /* --- SIDEBAR / SMALLER SECTIONS --- */
        .sidebar h3 {
            font-family: 'Syne', sans-serif;
            font-size: 1.3rem;
            color: var(--hot-pink);
            border-bottom: 2px solid var(--silver-stud);
            padding-bottom: 5px;
            margin-bottom: 15px;
        }

        /* Playlist / Top 8 style layout */
        .music-player {
            background: #000;
            border: 1px dashed var(--hot-pink);
            padding: 10px;
            font-size: 0.85rem;
            margin-bottom: 15px;
        }

        .track {
            display: flex;
            justify-content: space-between;
            padding: 5px 0;
            border-bottom: 1px solid #222;
        }
        .track:last-child { border: none; }
        .track span.playing { color: var(--neon-pink); }

        .button-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 10px;
            text-align: center;
        }

        .y2k-btn {
            background: linear-gradient(180deg, #333 0%, #111 100%);
            border: 2px solid var(--hot-pink);
            color: #fff;
            padding: 8px;
            font-size: 0.8rem;
            text-decoration: none;
            font-weight: bold;
            text-transform: uppercase;
        }

        .y2k-btn:hover {
            background: var(--hot-pink);
            color: #000;
            box-shadow: 0 0 8px var(--neon-pink);
        }

        /* --- FOOTER --- */
        footer {
            text-align: center;
            margin-top: 40px;
            padding: 20px;
            font-size: 0.8rem;
            color: var(--silver-dark);
            border-top: 1px dashed var(--hot-pink);
        }
    </style>
</head>
<body>

    <header>
        <h1>★ SOUND_WAVEZ ★</h1>
        <p>⚡ Your Ultimate 2000s Source for Tour Blast Outs & Live Music Madness ⚡</p>
    </header>

    <div class="ticker">
        <marquee scrollamount="6">+++ HARRY STYLES ANNOUNCES JAW-DROPPING LONDON SHOWS +++ KORN WORLD TOUR TICKETS ON SALE THIS FRIDAY +++ LIVE AND LOUD +++</marquee>
    </div>

    <div class="container">
        
        <main class="main-content studded-box">
            <h2><span>[ BLOG STAGE ]</span> <span>☠</span></h2>
            
            <div class="news-post">
                <h3>HARRY STYLES: Live In London (04.07.2026)!!</h3>
                <span class="date">POSTED: June 22, 2026 // 17:05 PM</span>
                <p>
                    Oh my god, rumors confirmed! Harry is officially taking over London for a massive, spectacular show on July 4th! Word on the street is the production is completely next level—think full retro glamor, massive digital glitter cascades, and a setlist packed with absolute surprises. Fans are already mapping out feather boa color themes. Get your platform boots ready, because this is going to be jaw-dropping!
                </p>
            </div>

            <div class="news-post">
                <h3>KORN Heavy-Hitting 2026 Tour Dates Unleashed!</h3>
                <span class="date">POSTED: June 21, 2026 // 11:14 AM</span>
                <p>
                    If you want heavy, you've got it. Korn just dropped their official stadium run map! They are bringing full retro nu-metal energy back to the stage with massive support acts. Expect bagpipes, field-shaking bass riffs, and the rawest moshpits of the decade. Do not sleep on these tickets, they will evaporate instantly.
                </p>
            </div>
        </main>

        <aside class="sidebar">
            
            <div class="studded-box">
                <h3>NAVIGATION</h3>
                <div class="button-grid">
                    <a href="#" class="y2k-btn">Home</a>
                    <a href="#" class="y2k-btn">Tour Dates</a>
                    <a href="#" class="y2k-btn">Outfits</a>
                    <a href="#" class="y2k-btn">Guestbook</a>
                </div>
            </div>

            <div class="studded-box">
                <h3>HYPED TRACKS</h3>
                <div class="music-player">
                    <div class="track"><span class="playing">► Sign of the Times</span> <span>4:50</span></div>
                    <div class="track"><span>As It Was</span> <span>2:47</span></div>
                    <div class="track"><span>Freak On a Leash</span> <span>4:15</span></div>
                    <div class="track"><span>Blind</span> <span>4:19</span></div>
                </div>
                <p style="font-size: 0.75rem; text-align: center; color: var(--neon-pink);">
                    [ 💿 4 tracks loaded in layout ]
                </p>
            </div>

            <div class="studded-box" style="text-align: center;">
                <h3>SITE STATUS</h3>
                <p style="color: #00ff00; font-weight: bold; margin-bottom: 5px;">● ONLINE</p>
                <p style="font-size: 0.8rem;">Vibe check: Glitter, spikes, and high volume.</p>
            </div>

        </aside>
    </div>

    <footer>
        <p>&copy; 2026 Xx_MUSIC_UPDATES_xX. Made with pure nostalgia.</p>
        <p style="margin-top: 5px; font-size: 0.7rem; color: var(--hot-pink);">⚡ Optimized for 1024x768 resolution (Just kidding, it's responsive!) ⚡</p>
    </footer>

</body>
</html>
