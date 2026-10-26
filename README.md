<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HALAL STOCK MARKET - Telegram Channel</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        :root {
            --bg-top: #0a111e;
            --bg-bottom: #040810;
            --card-bg: rgba(16, 26, 44, 0.7);
            --primary-cyan: #229ED9;
            --btn-gradient: linear-gradient(135deg, #0088cc 0%, #229ED9 100%);
            --accent-gold: #f5c518;
            --gold-gradient: linear-gradient(135deg, #ffe066 0%, #f5c518 100%);
            --text-main: #ffffff;
            --text-muted: #8e9bb0;
            --border-color: rgba(255, 255, 255, 0.08);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Plus Jakarta Sans', -apple-system, BlinkMacSystemFont, sans-serif;
            -webkit-tap-highlight-color: transparent;
        }

        body {
            background: linear-gradient(180deg, var(--bg-top) 0%, var(--bg-bottom) 100%);
            color: var(--text-main);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: flex-start;
            padding: 20px 15px 40px 15px;
            overflow-x: hidden;
        }

        .container {
            width: 100%;
            max-width: 440px;
            margin: 0 auto;
            display: flex;
            flex-direction: column;
            align-items: center;
            position: relative;
        }

        /* Top Header Badge */
        .top-badge {
            background: rgba(255, 255, 255, 0.04);
            border: 1px solid rgba(245, 197, 24, 0.25);
            padding: 6px 14px;
            border-radius: 20px;
            font-size: 0.72rem;
            font-weight: 700;
            letter-spacing: 1px;
            color: var(--accent-gold);
            display: flex;
            align-items: center;
            gap: 8px;
            margin-bottom: 25px;
            backdrop-filter: blur(10px);
            text-transform: uppercase;
        }

        .top-badge .dot {
            width: 7px;
            height: 7px;
            background-color: var(--accent-gold);
            border-radius: 50%;
            box-shadow: 0 0 8px var(--accent-gold);
            animation: pulse 1.8s infinite;
        }

        @keyframes pulse {
            0% { opacity: 0.4; transform: scale(0.9); }
            50% { opacity: 1; transform: scale(1.15); }
            100% { opacity: 0.4; transform: scale(0.9); }
        }

        /* Profile Image Section */
        .profile-wrapper {
            position: relative;
            margin-bottom: 18px;
        }

        .profile-img-container {
            width: 125px;
            height: 125px;
            border-radius: 50%;
            padding: 4px;
            background: linear-gradient(135deg, #f5c518 0%, #4facfe 100%);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.5), 0 0 15px rgba(34, 158, 217, 0.3);
            position: relative;
        }

        .profile-img {
            width: 100%;
            height: 100%;
            border-radius: 50%;
            object-fit: cover;
            border: 3px solid #0a111e;
            background-color: #101a2c;
        }

        .verified-badge {
            position: absolute;
            bottom: -4px;
            left: 50%;
            transform: translateX(-50%);
            background: var(--gold-gradient);
            color: #000;
            font-size: 0.7rem;
            font-weight: 800;
            padding: 3px 10px;
            border-radius: 12px;
            display: flex;
            align-items: center;
            gap: 4px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.4);
            white-space: nowrap;
        }

        /* Subtitle */
        .sub-tag {
            color: var(--accent-gold);
            font-size: 0.78rem;
            font-weight: 700;
            letter-spacing: 1.5px;
            text-transform: uppercase;
            margin-top: 10px;
            margin-bottom: 6px;
            text-align: center;
        }

        /* Title */
        .main-title {
            font-family: 'Playfair Display', serif;
            font-size: 1.95rem;
            font-weight: 700;
            text-align: center;
            color: #ffffff;
            margin-bottom: 8px;
            line-height: 1.2;
        }

        .main-title span {
            background: var(--gold-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            display: block;
        }

        /* Description */
        .description {
            color: var(--text-muted);
            font-size: 0.88rem;
            text-align: center;
            line-height: 1.45;
            margin-bottom: 24px;
            padding: 0 10px;
        }

        /* Primary CTA Button */
        .btn-telegram {
            width: 100%;
            background: var(--btn-gradient);
            color: #ffffff;
            text-decoration: none;
            padding: 16px 20px;
            border-radius: 14px;
            font-size: 1.05rem;
            font-weight: 700;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 12px;
            box-shadow: 0 8px 25px rgba(34, 158, 217, 0.4);
            transition: all 0.25s ease;
            position: relative;
            overflow: hidden;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        .btn-telegram:active {
            transform: scale(0.98);
        }

        .btn-telegram i {
            font-size: 1.3rem;
        }

        /* Helper Note */
        .cta-note {
            font-size: 0.75rem;
            color: var(--text-muted);
            margin-top: 10px;
            margin-bottom: 22px;
            text-align: center;
        }

        /* Member Counter Pill */
        .members-pill {
            background: rgba(255, 255, 255, 0.03);
            border: 1px solid var(--border-color);
            padding: 8px 16px;
            border-radius: 30px;
            display: flex;
            align-items: center;
            gap: 10px;
            margin-bottom: 25px;
        }

        .avatar-group {
            display: flex;
        }

        .avatar-group span {
            width: 20px;
            height: 20px;
            border-radius: 50%;
            background-color: var(--primary-cyan);
            border: 2px solid #0a111e;
            margin-left: -6px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 0.5rem;
            color: #fff;
            font-weight: 700;
        }

        .avatar-group span:first-child { margin-left: 0; background-color: #f5c518; color: #000; }
        .avatar-group span:nth-child(2) { background-color: #25d366; }
        .avatar-group span:nth-child(3) { background-color: #e1306c; }

        .members-text {
            font-size: 0.78rem;
            color: #d1d5db;
        }

        .members-text strong {
            color: #fff;
        }

        /* Feature Badges Grid */
        .features-grid {
            width: 100%;
            display: flex;
            gap: 10px;
            margin-bottom: 15px;
        }

        .feature-card {
            flex: 1;
            background: var(--card-bg);
            border: 1px solid var(--border-color);
            padding: 12px 10px;
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
            font-size: 0.78rem;
            font-weight: 600;
            color: #e2e8f0;
            backdrop-filter: blur(8px);
        }

        .feature-card i {
            color: var(--accent-gold);
            font-size: 0.9rem;
        }

        /* Bottom Tagline */
        .bottom-tag {
            background: rgba(255, 255, 255, 0.03);
            border: 1px solid var(--border-color);
            padding: 8px 18px;
            border-radius: 20px;
            font-size: 0.75rem;
            color: var(--text-muted);
            display: flex;
            align-items: center;
            gap: 6px;
            margin-top: 5px;
        }

        /* Disclaimer */
        .disclaimer {
            font-size: 0.65rem;
            color: #5d6b82;
            text-align: center;
            margin-top: 25px;
            line-height: 1.4;
        }
    </style>
</head>
<body>

    <div class="container">
        <!-- SEBI / Research Header -->
        <div class="top-badge">
            <span class="dot"></span>
            SEBI REGISTERED RESEARCH ANALYST
        </div>

        <!-- Profile Picture & Verified Tag -->
        <div class="profile-wrapper">
            <div class="profile-img-container">
                <img src="https://i.ibb.co/WNS5t62h/IMG-20261025-125833-583.jpg" alt="Halal Stock Market" class="profile-img">
            </div>
            <div class="verified-badge">
                <i class="fa-solid fa-check"></i> SEBI REG.
            </div>
        </div>

        <!-- Tagline -->
        <div class="sub-tag">Research & Market Education</div>

        <!-- Channel Title -->
        <h1 class="main-title">
            Learn with
            <span>HALAL STOCK MARKET</span>
        </h1>

        <!-- Short Description -->
        <p class="description">
            Daily Market Research • Halal Equity Research • Educational Insights
        </p>

        <!-- Main Join Button -->
        <a href="https://t.me/+gM70YcQjR7xkODI1" class="btn-telegram" target="_blank">
            <i class="fa-paper-plane"></i>
            Join Research Community — Free
        </a>

        <div class="cta-note">Access research updates and educational content.</div>

        <!-- Social Proof / Members Count -->
        <div class="members-pill">
            <div class="avatar-group">
                <span><i class="fa-solid fa-user"></i></span>
                <span><i class="fa-solid fa-user"></i></span>
                <span><i class="fa-solid fa-user"></i></span>
                <span>+</span>
            </div>
            <div class="members-text">Join our growing <strong>research community</strong></div>
        </div>

        <!-- Feature Badges -->
        <div class="features-grid">
            <div class="feature-card">
                <i class="fa-solid fa-building-columns"></i>
                SEBI Registered
            </div>
            <div class="feature-card">
                <i class="fa-solid fa-chart-line"></i>
                Market Research
            </div>
        </div>

        <!-- Location/Tagline -->
        <div class="bottom-tag">
            🇮🇳 Made for Indian Markets
        </div>

        <!-- Regulatory Disclaimer -->
        <p class="disclaimer">
            Disclaimer: Investments in securities market are subject to market risks. Read all related documents carefully before investing. Registration granted by SEBI is no guarantee of performance.
        </p>
    </div>

</body>
</html>
