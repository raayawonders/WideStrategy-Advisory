# WideStrategy-Advisory
WideStrategy Advisors LLP - Corporate website for a boutique strategic and financial advisory firm specializing in capital raising, transaction advisory, ESG consulting, wealth management, and cross-border business solutions.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="WideStrategy Advisors LLP – Boutique strategic and financial advisory firm in India. Experts in capital raising, transaction advisory, ESG consulting, and wealth management." />
  <meta name="keywords" content="strategic advisory India, financial advisory, capital raising, ESG consulting, debt fundraising, equity fundraising, transaction advisory, wealth management, family office" />
  <meta property="og:title" content="WideStrategy Advisors LLP – Where Capital Meets Strategy" />
  <meta property="og:description" content="Boutique strategic and financial advisory for growth-focused enterprises across India." />
  <title>WideStrategy Advisors LLP – Where Capital Meets Strategy</title>

  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,400;0,500;0,600;1,400&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet" />

  <style>
    /* ─── TOKENS ─────────────────────────────────────────────────── */
    :root {
      --beige:       #F5E6D3;
      --off-white:   #FAF9F6;
      --navy:        #1F3A5F;
      --dark-navy:   #14263D;
      --gold:        #D6B98C;
      --gold-light:  #E8D2B0;
      --text-body:   #3A3A3A;
      --text-muted:  #6B7280;
      --border:      rgba(31,58,95,0.10);
      --shadow-sm:   0 1px 3px rgba(20,38,61,0.06), 0 1px 2px rgba(20,38,61,0.04);
      --shadow-md:   0 4px 16px rgba(20,38,61,0.08);
      --shadow-lg:   0 12px 40px rgba(20,38,61,0.12);

      --font-display: 'Cormorant Garamond', Georgia, serif;
      --font-body:    'Inter', system-ui, sans-serif;

      --max-w: 1200px;
      --section-v: 96px;
    }

    /* ─── RESET ──────────────────────────────────────────────────── */
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
    html { scroll-behavior: smooth; font-size: 16px; }
    body {
      font-family: var(--font-body);
      color: var(--text-body);
      background: var(--off-white);
      line-height: 1.65;
      -webkit-font-smoothing: antialiased;
    }
    img { display: block; max-width: 100%; }
    a { color: inherit; text-decoration: none; }
    ul { list-style: none; }
    button { cursor: pointer; border: none; background: none; font: inherit; }

    /* ─── LAYOUT HELPERS ─────────────────────────────────────────── */
    .container { max-width: var(--max-w); margin: 0 auto; padding: 0 32px; }
    .section { padding: var(--section-v) 0; }
    .section--navy { background: var(--navy); color: var(--off-white); }
    .section--dark { background: var(--dark-navy); color: var(--off-white); }
    .section--beige { background: var(--beige); }
    .section--cream { background: #F0E6D9; }

    /* ─── TYPOGRAPHY ─────────────────────────────────────────────── */
    .eyebrow {
      font-family: var(--font-body);
      font-size: 11px;
      font-weight: 600;
      letter-spacing: 0.18em;
      text-transform: uppercase;
      color: var(--gold);
      margin-bottom: 16px;
      display: block;
    }
    .section--navy .eyebrow,
    .section--dark .eyebrow { color: var(--gold-light); }

    h1, h2, h3, h4 { font-family: var(--font-display); line-height: 1.18; font-weight: 500; }
    h1 { font-size: clamp(40px, 5.5vw, 72px); }
    h2 { font-size: clamp(32px, 3.8vw, 52px); }
    h3 { font-size: clamp(22px, 2.4vw, 30px); }
    h4 { font-size: 20px; font-weight: 500; }

    .lead {
      font-size: clamp(16px, 1.4vw, 18px);
      color: var(--text-muted);
      line-height: 1.75;
      max-width: 600px;
    }
    .section--navy .lead,
    .section--dark .lead { color: rgba(250,249,246,0.72); }

    /* ─── BUTTONS ─────────────────────────────────────────────────── */
    .btn {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 14px 28px;
      font-family: var(--font-body);
      font-size: 14px;
      font-weight: 500;
      letter-spacing: 0.04em;
      border-radius: 2px;
      transition: all 0.22s ease;
    }
    .btn-primary {
      background: var(--gold);
      color: var(--dark-navy);
    }
    .btn-primary:hover { background: #C4A478; transform: translateY(-1px); box-shadow: var(--shadow-md); }
    .btn-outline {
      border: 1.5px solid rgba(250,249,246,0.45);
      color: var(--off-white);
    }
    .btn-outline:hover { border-color: var(--gold); color: var(--gold); }
    .btn-outline-dark {
      border: 1.5px solid var(--navy);
      color: var(--navy);
    }
    .btn-outline-dark:hover { background: var(--navy); color: var(--off-white); }

    /* ─── NAVIGATION ─────────────────────────────────────────────── */
    #navbar {
      position: fixed;
      top: 0; left: 0; right: 0;
      z-index: 1000;
      padding: 0 32px;
      height: 72px;
      display: flex;
      align-items: center;
      transition: background 0.3s, box-shadow 0.3s;
    }
    #navbar.scrolled {
      background: rgba(20,38,61,0.97);
      backdrop-filter: blur(12px);
      box-shadow: 0 1px 0 rgba(214,185,140,0.15);
    }
    .nav-inner {
      max-width: var(--max-w);
      margin: 0 auto;
      width: 100%;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }
    .nav-logo {
      display: flex;
      flex-direction: row;
      align-items: center;
      gap: 14px;
    }
    .nav-logo img {
      filter: invert(1) brightness(2);
      height: 44px;
      width: auto;
      display: block;
    }
    .nav-logo-name {
      font-family: var(--font-display);
      font-size: 20px;
      font-weight: 600;
      color: var(--off-white);
      letter-spacing: 0.02em;
    }
    .nav-logo-tag {
      font-size: 9.5px;
      letter-spacing: 0.16em;
      text-transform: uppercase;
      color: var(--gold);
      font-weight: 500;
    }
    .nav-logo-text {
      display: flex;
      flex-direction: column;
      gap: 1px;
    }
    .nav-links {
      display: flex;
      align-items: center;
      gap: 36px;
    }
    .nav-links a {
      font-size: 13px;
      font-weight: 500;
      letter-spacing: 0.04em;
      color: rgba(250,249,246,0.8);
      transition: colour 0.2s;
      position: relative;
    }
    .nav-links a::after {
      content: '';
      position: absolute;
      bottom: -3px; left: 0; right: 0;
      height: 1px;
      background: var(--gold);
      transform: scaleX(0);
      transition: transform 0.2s;
    }
    .nav-links a:hover { color: var(--off-white); }
    .nav-links a:hover::after { transform: scaleX(1); }
    .nav-cta {
      padding: 10px 20px;
      background: var(--gold);
      color: var(--dark-navy) !important;
      border-radius: 2px;
      font-weight: 600 !important;
    }
    .nav-cta:hover { background: #C4A478; }
    .nav-cta::after { display: none !important; }

    .hamburger {
      display: none;
      flex-direction: column;
      gap: 5px;
      padding: 4px;
    }
    .hamburger span {
      display: block;
      width: 24px; height: 1.5px;
      background: var(--off-white);
      transition: all 0.22s;
    }

    /* ─── MOBILE MENU ────────────────────────────────────────────── */
    #mobile-menu {
      display: none;
      position: fixed;
      top: 72px; left: 0; right: 0;
      background: var(--dark-navy);
      padding: 24px 32px 32px;
      z-index: 999;
      flex-direction: column;
      gap: 20px;
      border-top: 1px solid rgba(214,185,140,0.15);
    }
    #mobile-menu.open { display: flex; }
    #mobile-menu a {
      font-size: 15px;
      font-weight: 500;
      color: rgba(250,249,246,0.85);
      padding: 8px 0;
      border-bottom: 1px solid rgba(250,249,246,0.07);
    }
    #mobile-menu a:last-child { border: none; }

    /* ─── HERO ───────────────────────────────────────────────────── */
    #hero {
      min-height: 100vh;
      background: var(--dark-navy);
      display: flex;
      align-items: center;
      position: relative;
      overflow: hidden;
      padding: 120px 32px 80px;
    }
    .hero-bg-pattern {
      position: absolute;
      inset: 0;
      opacity: 0.035;
      background-image:
        repeating-linear-gradient(
          0deg,
          transparent,
          transparent 59px,
          rgba(214,185,140,1) 59px,
          rgba(214,185,140,1) 60px
        ),
        repeating-linear-gradient(
          90deg,
          transparent,
          transparent 59px,
          rgba(214,185,140,1) 59px,
          rgba(214,185,140,1) 60px
        );
    }
    .hero-accent {
      position: absolute;
      top: -120px; right: -80px;
      width: 560px; height: 560px;
      border-radius: 50%;
      background: radial-gradient(circle, rgba(214,185,140,0.12) 0%, transparent 70%);
      pointer-events: none;
    }
    .hero-accent-2 {
      position: absolute;
      bottom: -80px; left: -60px;
      width: 400px; height: 400px;
      border-radius: 50%;
      background: radial-gradient(circle, rgba(31,58,95,0.4) 0%, transparent 70%);
      pointer-events: none;
    }
    .hero-inner {
      max-width: 780px;
      margin: 0 auto;
      width: 100%;
      position: relative;
      z-index: 1;
      display: block;
    }
    .hero-content { }
    .hero-eyebrow {
      display: inline-flex;
      align-items: center;
      gap: 10px;
      font-size: 11px;
      font-weight: 600;
      letter-spacing: 0.18em;
      text-transform: uppercase;
      color: var(--gold);
      margin-bottom: 28px;
    }
    .hero-eyebrow::before {
      content: '';
      display: block;
      width: 28px; height: 1px;
      background: var(--gold);
    }
    .hero-headline {
      color: var(--off-white);
      margin-bottom: 28px;
      font-weight: 500;
    }
    .hero-headline em { font-family: var(--font-display);
      font-style: italic;
      color: var(--gold);
    }
    .hero-sub {
      font-size: 17px;
      color: rgba(250,249,246,0.65);
      line-height: 1.72;
      margin-bottom: 48px;
      max-width: 520px;
    }
    .hero-actions { display: flex; gap: 16px; flex-wrap: wrap; }
    .hero-stat { }
    .hero-stat-value {
      font-family: var(--font-display);
      font-size: 42px;
      font-weight: 500;
      color: var(--gold);
      line-height: 1;
      margin-bottom: 8px;
    }
    .hero-stat-label {
      font-size: 12px;
      color: rgba(250,249,246,0.55);
      letter-spacing: 0.06em;
      line-height: 1.4;
    }
    .hero-stat-divider {
      grid-column: 1 / -1;
      height: 1px;
      background: rgba(214,185,140,0.12);
    }
    .hero-card-label {
      grid-column: 1 / -1;
      font-size: 10px;
      letter-spacing: 0.18em;
      text-transform: uppercase;
      color: var(--gold);
      font-weight: 600;
      padding-bottom: 16px;
      border-bottom: 1px solid rgba(214,185,140,0.12);
      margin-bottom: -8px;
    }

    /* ─── TICKER ─────────────────────────────────────────────────── */
    .ticker-bar {
      background: var(--navy);
      border-top: 1px solid rgba(214,185,140,0.12);
      border-bottom: 1px solid rgba(214,185,140,0.12);
      padding: 12px 0;
      overflow: hidden;
      white-space: nowrap;
    }
    .ticker-inner {
      display: inline-flex;
      animation: ticker 28s linear infinite;
      gap: 0;
    }
    .ticker-item {
      display: inline-flex;
      align-items: center;
      gap: 10px;
      padding: 0 40px;
      font-size: 12px;
      font-weight: 500;
      letter-spacing: 0.08em;
      color: rgba(250,249,246,0.6);
    }
    .ticker-item span { color: var(--gold); }
    @keyframes ticker {
      0% { transform: translateX(0); }
      100% { transform: translateX(-50%); }
    }

    /* ─── ABOUT PREVIEW ──────────────────────────────────────────── */
    .about-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 80px;
      align-items: center;
    }
    .about-visual {
      position: relative;
    }
    .about-img-frame {
      width: 100%;
      aspect-ratio: 4/5;
      background: linear-gradient(135deg, var(--navy) 0%, var(--dark-navy) 100%);
      border-radius: 2px;
      display: flex;
      align-items: center;
      justify-content: center;
      overflow: hidden;
      position: relative;
    }
    .about-img-inner {
      position: absolute;
      inset: 0;
      background: 
        linear-gradient(145deg, rgba(214,185,140,0.06) 0%, transparent 50%),
        repeating-linear-gradient(
          45deg,
          transparent,
          transparent 20px,
          rgba(214,185,140,0.03) 20px,
          rgba(214,185,140,0.03) 21px
        );
    }
    .about-img-text {
      font-family: var(--font-display);
      font-size: 64px;
      font-weight: 400;
      color: rgba(214,185,140,0.2);
      text-align: center;
      line-height: 1.1;
      z-index: 1;
      position: relative;
    }
    .about-badge {
      position: absolute;
      bottom: -24px; right: -24px;
      width: 140px; height: 140px;
      background: var(--gold);
      border-radius: 50%;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      color: var(--dark-navy);
      padding: 16px;
    }
    .about-badge-num {
      font-family: var(--font-display);
      font-size: 36px;
      font-weight: 600;
      line-height: 1;
    }
    .about-badge-label {
      font-size: 10px;
      font-weight: 600;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      line-height: 1.3;
      margin-top: 4px;
    }
    .about-content { }
    .about-body {
      color: var(--text-muted);
      font-size: 15.5px;
      line-height: 1.8;
      margin-bottom: 24px;
    }
    .about-pillars {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 16px;
      margin: 32px 0;
    }
    .about-pillar {
      display: flex;
      align-items: flex-start;
      gap: 12px;
      padding: 16px;
      background: var(--beige);
      border-radius: 2px;
    }
    .about-pillar-icon {
      width: 36px; height: 36px;
      flex-shrink: 0;
      background: var(--navy);
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
    }
    .about-pillar-icon svg { width: 16px; height: 16px; fill: var(--gold); }
    .about-pillar-text {
      font-size: 13px;
      font-weight: 500;
      color: var(--dark-navy);
      line-height: 1.4;
    }

    /* ─── SERVICES GRID ──────────────────────────────────────────── */
    .services-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 1px;
      background: var(--border);
      border: 1px solid var(--border);
    }
    .service-card {
      background: var(--off-white);
      padding: 36px 28px;
      transition: all 0.25s ease;
      cursor: default;
      position: relative;
      overflow: hidden;
    }
    .service-card::before {
      content: '';
      position: absolute;
      bottom: 0; left: 0;
      width: 100%; height: 2px;
      background: var(--gold);
      transform: scaleX(0);
      transform-origin: left;
      transition: transform 0.25s ease;
    }
    .service-card:hover { background: var(--navy); }
    .service-card:hover .service-num { color: rgba(214,185,140,0.25); }
    .service-card:hover .service-title { color: var(--off-white); }
    .service-card:hover .service-desc { color: rgba(250,249,246,0.6); }
    .service-card:hover::before { transform: scaleX(1); }
    .service-num {
      font-family: var(--font-display);
      font-size: 44px;
      font-weight: 400;
      color: rgba(31,58,95,0.12);
      line-height: 1;
      margin-bottom: 20px;
      transition: colour 0.25s;
    }
    .service-icon-wrap {
      width: 44px; height: 44px;
      background: var(--beige);
      border-radius: 2px;
      display: flex;
      align-items: center;
      justify-content: center;
      margin-bottom: 16px;
      transition: background 0.25s;
    }
    .service-card:hover .service-icon-wrap { background: rgba(214,185,140,0.15); }
    .service-icon-wrap svg { width: 20px; height: 20px; }
    .service-title {
      font-family: var(--font-display);
      font-size: 20px;
      font-weight: 500;
      color: var(--dark-navy);
      margin-bottom: 10px;
      transition: colour 0.25s;
      line-height: 1.25;
    }
    .service-desc {
      font-size: 13px;
      color: var(--text-muted);
      line-height: 1.65;
      transition: colour 0.25s;
    }

    /* ─── WHY CHOOSE US ──────────────────────────────────────────── */
    .why-grid {
      display: grid;
      grid-template-columns: 1fr 1.4fr;
      gap: 80px;
      align-items: center;
    }
    .why-list { display: flex; flex-direction: column; gap: 32px; }
    .why-item {
      display: flex;
      gap: 20px;
      padding-bottom: 32px;
      border-bottom: 1px solid rgba(250,249,246,0.08);
    }
    .why-item:last-child { border: none; padding-bottom: 0; }
    .why-item-num {
      font-family: var(--font-display);
      font-size: 36px;
      font-weight: 400;
      color: rgba(214,185,140,0.3);
      line-height: 1;
      flex-shrink: 0;
      width: 48px;
    }
    .why-item-content h4 {
      font-family: var(--font-display);
      font-size: 22px;
      color: var(--off-white);
      margin-bottom: 8px;
    }
    .why-item-content p {
      font-size: 14px;
      color: rgba(250,249,246,0.58);
      line-height: 1.7;
    }
    .why-visual {
      display: flex;
      flex-direction: column;
      gap: 16px;
    }
    .why-metric {
      background: rgba(31,58,95,0.5);
      border: 1px solid rgba(214,185,140,0.12);
      border-radius: 3px;
      padding: 24px 28px;
      display: flex;
      align-items: center;
      gap: 20px;
    }
    .why-metric-val {
      font-family: var(--font-display);
      font-size: 40px;
      font-weight: 500;
      color: var(--gold);
      flex-shrink: 0;
      line-height: 1;
    }
    .why-metric-info {}
    .why-metric-label {
      font-size: 14px;
      font-weight: 500;
      color: var(--off-white);
      margin-bottom: 4px;
    }
    .why-metric-sub {
      font-size: 12px;
      color: rgba(250,249,246,0.45);
    }

    /* ─── PROCESS ────────────────────────────────────────────────── */
    .process-track {
      display: grid;
      grid-template-columns: repeat(5, 1fr);
      gap: 0;
      position: relative;
    }
    .process-track::before {
      content: '';
      position: absolute;
      top: 28px;
      left: calc(10% + 28px);
      right: calc(10% + 28px);
      height: 1px;
      background: var(--gold);
      opacity: 0.3;
      z-index: 0;
    }
    .process-step {
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
      padding: 0 12px;
      position: relative;
      z-index: 1;
    }
    .process-dot {
      width: 56px; height: 56px;
      border-radius: 50%;
      background: var(--off-white);
      border: 1.5px solid var(--gold);
      display: flex;
      align-items: center;
      justify-content: center;
      margin-bottom: 20px;
      flex-shrink: 0;
    }
    .process-dot-inner {
      width: 10px; height: 10px;
      border-radius: 50%;
      background: var(--gold);
    }
    .process-step-num {
      font-size: 10px;
      font-weight: 600;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: var(--gold);
      margin-bottom: 8px;
    }
    .process-step-title {
      font-family: var(--font-display);
      font-size: 18px;
      font-weight: 500;
      color: var(--dark-navy);
      margin-bottom: 8px;
      line-height: 1.25;
    }
    .process-step-desc {
      font-size: 12.5px;
      color: var(--text-muted);
      line-height: 1.6;
    }

    /* ─── INDUSTRIES ─────────────────────────────────────────────── */
    .industries-grid {
      display: grid;
      grid-template-columns: repeat(5, 1fr);
      gap: 16px;
    }
    .industry-card {
      background: rgba(31,58,95,0.5);
      border: 1px solid rgba(214,185,140,0.1);
      border-radius: 3px;
      padding: 32px 20px;
      text-align: center;
      transition: all 0.25s ease;
    }
    .industry-card:hover {
      background: rgba(214,185,140,0.1);
      border-color: rgba(214,185,140,0.3);
      transform: translateY(-3px);
    }
    .industry-icon {
      font-size: 32px;
      margin-bottom: 16px;
      display: block;
    }
    .industry-name {
      font-family: var(--font-display);
      font-size: 17px;
      color: var(--off-white);
      margin-bottom: 8px;
    }
    .industry-desc {
      font-size: 12px;
      color: rgba(250,249,246,0.45);
      line-height: 1.5;
    }

    /* ─── INSIGHTS ───────────────────────────────────────────────── */
    .insights-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 28px;
    }
    .insight-card {
      background: var(--off-white);
      border: 1px solid var(--border);
      border-radius: 2px;
      overflow: hidden;
      transition: box-shadow 0.25s, transform 0.25s;
    }
    .insight-card:hover {
      box-shadow: var(--shadow-lg);
      transform: translateY(-3px);
    }
    .insight-thumb {
      height: 200px;
      background: linear-gradient(135deg, var(--navy) 0%, var(--dark-navy) 100%);
      display: flex;
      align-items: center;
      justify-content: center;
      position: relative;
      overflow: hidden;
    }
    .insight-thumb-text {
      font-family: var(--font-display);
      font-size: 52px;
      color: rgba(214,185,140,0.15);
      font-style: italic;
      position: absolute;
    }
    .insight-thumb-tag {
      position: absolute;
      top: 16px; left: 16px;
      background: var(--gold);
      color: var(--dark-navy);
      font-size: 10px;
      font-weight: 600;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      padding: 4px 10px;
      border-radius: 1px;
    }
    .insight-body { padding: 28px; }
    .insight-meta {
      font-size: 11px;
      color: var(--text-muted);
      letter-spacing: 0.05em;
      margin-bottom: 12px;
    }
    .insight-title {
      font-family: var(--font-display);
      font-size: 21px;
      font-weight: 500;
      color: var(--dark-navy);
      line-height: 1.3;
      margin-bottom: 12px;
    }
    .insight-excerpt {
      font-size: 13.5px;
      color: var(--text-muted);
      line-height: 1.7;
      margin-bottom: 20px;
    }
    .insight-link {
      font-size: 13px;
      font-weight: 600;
      color: var(--navy);
      letter-spacing: 0.04em;
      display: inline-flex;
      align-items: center;
      gap: 6px;
      transition: gap 0.2s;
    }
    .insight-link:hover { gap: 10px; }

    /* ─── FINAL CTA ──────────────────────────────────────────────── */
    .cta-section {
      padding: 100px 32px;
      background: var(--dark-navy);
      text-align: center;
      position: relative;
      overflow: hidden;
    }
    .cta-accent {
      position: absolute;
      top: 50%; left: 50%;
      transform: translate(-50%, -50%);
      width: 600px; height: 300px;
      border-radius: 50%;
      background: radial-gradient(ellipse, rgba(214,185,140,0.06) 0%, transparent 70%);
    }
    .cta-inner { position: relative; z-index: 1; max-width: 640px; margin: 0 auto; }
    .cta-inner h2 {
      color: var(--off-white);
      margin-bottom: 20px;
    }
    .cta-inner p {
      color: rgba(250,249,246,0.6);
      font-size: 16px;
      line-height: 1.75;
      margin-bottom: 40px;
    }
    .cta-actions { display: flex; gap: 16px; justify-content: center; flex-wrap: wrap; }

    /* ─── CONTACT ────────────────────────────────────────────────── */
    .contact-grid {
      display: grid;
      grid-template-columns: 1fr 1.4fr;
      gap: 80px;
    }
    .contact-info { }
    .contact-item {
      display: flex;
      gap: 16px;
      margin-bottom: 32px;
      align-items: flex-start;
    }
    .contact-icon {
      width: 44px; height: 44px;
      background: var(--beige);
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      flex-shrink: 0;
    }
    .contact-icon svg { width: 18px; height: 18px; stroke: var(--navy); }
    .contact-item-label {
      font-size: 11px;
      font-weight: 600;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      color: var(--gold);
      margin-bottom: 4px;
    }
    .contact-item-value {
      font-size: 15px;
      color: var(--dark-navy);
      line-height: 1.5;
    }
    .map-placeholder {
      width: 100%;
      height: 220px;
      background: linear-gradient(135deg, var(--navy) 0%, var(--dark-navy) 100%);
      border-radius: 3px;
      display: flex;
      align-items: center;
      justify-content: center;
      margin-top: 32px;
      position: relative;
      overflow: hidden;
    }
    .map-placeholder-inner {
      text-align: center;
      color: rgba(250,249,246,0.4);
      font-size: 13px;
    }

    /* Contact form */
    .contact-form { display: flex; flex-direction: column; gap: 20px; }
    .form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 16px; }
    .form-group { display: flex; flex-direction: column; gap: 7px; }
    .form-label {
      font-size: 11px;
      font-weight: 600;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: var(--navy);
    }
    .form-input, .form-select, .form-textarea {
      width: 100%;
      padding: 13px 16px;
      font-family: var(--font-body);
      font-size: 14px;
      color: var(--dark-navy);
      background: var(--off-white);
      border: 1.5px solid var(--border);
      border-radius: 2px;
      outline: none;
      transition: border-colour 0.2s;
    }
    .form-input:focus, .form-select:focus, .form-textarea:focus {
      border-color: var(--navy);
    }
    .form-textarea { resize: vertical; min-height: 120px; }
    .form-select { appearance: none; cursor: pointer; }
    .form-submit {
      background: var(--navy);
      color: var(--off-white);
      padding: 15px 32px;
      font-size: 14px;
      font-weight: 500;
      letter-spacing: 0.06em;
      border-radius: 2px;
      transition: background 0.2s;
      align-self: flex-start;
    }
    .form-submit:hover { background: var(--dark-navy); }

    /* ─── ABOUT PAGE SECTIONS ────────────────────────────────────── */
    .team-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 32px;
    }
    .team-card {
      background: var(--off-white);
      border: 1px solid var(--border);
      border-radius: 2px;
      overflow: hidden;
      transition: box-shadow 0.25s;
    }
    .team-card:hover { box-shadow: var(--shadow-lg); }
    .team-photo {
      height: 280px;
      background: linear-gradient(150deg, var(--navy) 0%, var(--dark-navy) 100%);
      display: flex;
      align-items: center;
      justify-content: center;
      position: relative;
    }
    .team-photo-initials {
      font-family: var(--font-display);
      font-size: 64px;
      color: rgba(214,185,140,0.25);
      font-style: italic;
    }
    .team-body { padding: 24px; }
    .team-name {
      font-family: var(--font-display);
      font-size: 22px;
      font-weight: 500;
      color: var(--dark-navy);
      margin-bottom: 4px;
    }
    .team-role {
      font-size: 12px;
      font-weight: 600;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--gold);
      margin-bottom: 14px;
    }
    .team-bio { font-size: 13.5px; color: var(--text-muted); line-height: 1.7; margin-bottom: 0; }

    .vm-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 40px; }
    .vm-card {
      padding: 48px 40px;
      border-radius: 2px;
      position: relative;
      overflow: hidden;
    }
    .vm-card--vision { background: var(--navy); }
    .vm-card--mission { background: var(--dark-navy); }
    .vm-card-label {
      font-size: 10px;
      font-weight: 700;
      letter-spacing: 0.2em;
      text-transform: uppercase;
      color: var(--gold);
      margin-bottom: 20px;
      display: block;
    }
    .vm-card h3 {
      color: var(--off-white);
      font-size: 26px;
      margin-bottom: 16px;
    }
    .vm-card p { color: rgba(250,249,246,0.65); font-size: 15px; line-height: 1.75; }

    /* ─── SERVICES DETAIL ────────────────────────────────────────── */
    .service-detail {
      padding: 60px 0;
      border-bottom: 1px solid var(--border);
    }
    .service-detail:last-child { border: none; }
    .service-detail-grid {
      display: grid;
      grid-template-columns: 280px 1fr;
      gap: 64px;
      align-items: start;
    }
    .service-detail-label {
      font-size: 10px;
      font-weight: 700;
      letter-spacing: 0.2em;
      text-transform: uppercase;
      color: var(--gold);
      margin-bottom: 12px;
    }
    .service-detail-title {
      font-family: var(--font-display);
      font-size: 32px;
      font-weight: 500;
      color: var(--dark-navy);
    }
    .service-detail-body {
      font-size: 15px;
      color: var(--text-muted);
      line-height: 1.8;
      margin-bottom: 24px;
    }
    .service-tags { display: flex; flex-wrap: wrap; gap: 8px; }
    .service-tag {
      padding: 6px 14px;
      background: var(--beige);
      border-radius: 20px;
      font-size: 12px;
      font-weight: 500;
      color: var(--navy);
      letter-spacing: 0.02em;
    }

    /* ─── PAGE HEADER ────────────────────────────────────────────── */
    .page-header {
      padding: 140px 32px 80px;
      background: var(--dark-navy);
      position: relative;
      overflow: hidden;
    }
    .page-header-bg {
      position: absolute;
      inset: 0;
      opacity: 0.025;
      background-image: repeating-linear-gradient(
        0deg, transparent, transparent 59px,
        rgba(214,185,140,1) 59px, rgba(214,185,140,1) 60px
      ), repeating-linear-gradient(
        90deg, transparent, transparent 59px,
        rgba(214,185,140,1) 59px, rgba(214,185,140,1) 60px
      );
    }
    .page-header-inner {
      max-width: var(--max-w);
      margin: 0 auto;
      position: relative;
      z-index: 1;
    }
    .page-header-inner h1 { color: var(--off-white); }
    .page-header-inner p {
      color: rgba(250,249,246,0.6);
      font-size: 18px;
      margin-top: 16px;
      max-width: 560px;
      line-height: 1.7;
    }

    /* ─── SECTION HEADER ─────────────────────────────────────────── */
    .section-header { margin-bottom: 56px; }
    .section-header--centre { text-align: center; }
    .section-header--centre .lead { margin: 0 auto; }

    /* ─── FOOTER ─────────────────────────────────────────────────── */
    footer {
      background: #0E1B2A;
      padding: 72px 32px 0;
    }
    .footer-inner {
      max-width: var(--max-w);
      margin: 0 auto;
    }
    .footer-top {
      display: grid;
      grid-template-columns: 2fr 1fr 1fr 1fr;
      gap: 56px;
      padding-bottom: 56px;
      border-bottom: 1px solid rgba(214,185,140,0.08);
    }
    .footer-brand-name {
      font-family: var(--font-display);
      font-size: 22px;
      font-weight: 600;
      color: var(--off-white);
      margin-bottom: 4px;
    }
    .footer-brand-tag {
      font-size: 10px;
      letter-spacing: 0.16em;
      text-transform: uppercase;
      color: var(--gold);
      margin-bottom: 20px;
    }
    .footer-desc {
      font-size: 13.5px;
      color: rgba(250,249,246,0.4);
      line-height: 1.75;
      max-width: 280px;
    }
    .footer-col-title {
      font-size: 11px;
      font-weight: 700;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      color: var(--gold);
      margin-bottom: 20px;
    }
    .footer-col ul { display: flex; flex-direction: column; gap: 12px; }
    .footer-col ul a {
      font-size: 13.5px;
      color: rgba(250,249,246,0.45);
      transition: colour 0.2s;
    }
    .footer-col ul a:hover { color: var(--off-white); }
    .footer-bottom {
      padding: 24px 0;
      display: flex;
      align-items: center;
      justify-content: space-between;
      flex-wrap: wrap;
      gap: 12px;
    }
    .footer-copy {
      font-size: 12.5px;
      color: rgba(250,249,246,0.25);
    }
    .footer-legal { display: flex; gap: 24px; }
    .footer-legal a {
      font-size: 12.5px;
      color: rgba(250,249,246,0.25);
      transition: colour 0.2s;
    }
    .footer-legal a:hover { color: rgba(250,249,246,0.6); }

    /* ─── PAGE NAVIGATION ────────────────────────────────────────── */
    .page-section {
      display: none;
    }
    .page-section.active {
      display: block;
    }

    /* ─── DIVIDER ────────────────────────────────────────────────── */
    .gold-rule {
      width: 48px; height: 2px;
      background: var(--gold);
      margin-bottom: 24px;
    }
    .section-header--centre .gold-rule { margin: 0 auto 24px; }

    /* ─── RESPONSIVE ─────────────────────────────────────────────── */
    @media (max-width: 1100px) {
      .services-grid { grid-template-columns: repeat(2, 1fr); }
      .footer-top { grid-template-columns: 1fr 1fr; gap: 40px; }
      .process-track { grid-template-columns: 1fr 1fr; gap: 32px; }
      .process-track::before { display: none; }
      .industries-grid { grid-template-columns: repeat(3, 1fr); }
    }

    @media (max-width: 768px) {
      :root { --section-v: 64px; }
      .container { padding: 0 20px; }
      #hero { padding: 100px 20px 64px; }
      .about-grid { grid-template-columns: 1fr; }
      .about-badge { display: none; }
      .about-pillars { grid-template-columns: 1fr; }
      .why-grid { grid-template-columns: 1fr; }
      .contact-grid { grid-template-columns: 1fr; }
      .form-row { grid-template-columns: 1fr; }
      .insights-grid { grid-template-columns: 1fr; }
      .team-grid { grid-template-columns: 1fr; }
      .team-founders-grid { grid-template-columns: 1fr !important; }
      .vm-grid { grid-template-columns: 1fr; }
      .footer-top { grid-template-columns: 1fr 1fr; }
      .nav-links { display: none; }
      .hamburger { display: flex; }
      .service-detail-grid { grid-template-columns: 1fr; }
      .industries-grid { grid-template-columns: 1fr 1fr; }
      .process-track { grid-template-columns: 1fr; }
      .services-grid { grid-template-columns: 1fr 1fr; }
    }

    @media (max-width: 480px) {
      .services-grid { grid-template-columns: 1fr; }
      .industries-grid { grid-template-columns: 1fr 1fr; }
      .footer-top { grid-template-columns: 1fr; }
      .footer-bottom { flex-direction: column; align-items: flex-start; }
    }

    /* ─── SCROLL ANIMATIONS ──────────────────────────────────────── */
    .fade-up {
      opacity: 0;
      transform: translateY(28px);
      transition: opacity 0.55s ease, transform 0.55s ease;
    }
    .fade-up.visible {
      opacity: 1;
      transform: translateY(0);
    }
  
    /* ─── EXPLICIT CONTRAST FIXES ───────────────────────────────── */

    /* All text inside .section--navy and .section--dark should be light */
    .section--navy h1,
    .section--navy h2,
    .section--navy h3,
    .section--navy h4,
    .section--navy p,
    .section--navy li,
    .section--navy span:not(.eyebrow):not(.service-tag) {
      color: var(--off-white);
    }
    .section--dark h1,
    .section--dark h2,
    .section--dark h3,
    .section--dark h4,
    .section--dark p,
    .section--dark li {
      color: var(--off-white);
    }

    /* Why section on navy bg */
    .why-item-content h4 { color: var(--off-white); }
    .why-item-content p  { color: rgba(250,249,246,0.72); }
    .why-metric-label    { color: var(--off-white); }
    .why-metric-sub      { color: rgba(250,249,246,0.6); }

    /* Industry cards on dark bg */
    .industry-name { color: var(--off-white); }
    .industry-desc { color: rgba(250,249,246,0.65); }

    /* VM cards (vision/mission) on dark bg */
    .vm-card h3 { color: var(--off-white); }
    .vm-card p  { color: rgba(250,249,246,0.72); }
    .vm-card-label { color: var(--gold); }

    /* Footer on very dark bg */
    .footer-brand-name { color: var(--off-white); }
    .footer-desc       { color: rgba(250,249,246,0.55); }
    .footer-copy       { color: rgba(250,249,246,0.4); }
    .footer-col ul a   { color: rgba(250,249,246,0.6); }
    .footer-col ul a:hover { color: var(--off-white); }
    .footer-legal a    { color: rgba(250,249,246,0.4); }
    .footer-legal a:hover { color: var(--off-white); }

    /* Page header (dark bg) */
    .page-header-inner h1 { color: var(--off-white); }
    .page-header-inner p  { color: rgba(250,249,246,0.72); }
    .page-header-inner .eyebrow { color: var(--gold); }

    /* Hero section (dark bg) */
    .hero-headline { color: var(--off-white); }
    .hero-sub      { color: rgba(250,249,246,0.72); }
    .hero-stat-value { color: var(--gold); }
    .hero-stat-label { color: rgba(250,249,246,0.65); }
    .hero-card-label { color: var(--gold); }

    /* Ticker bar on navy bg */
    .ticker-item { color: rgba(250,249,246,0.7); }
    .ticker-item span { color: var(--gold); }

    /* CTA section on dark bg */
    .cta-inner h2 { color: var(--off-white); }
    .cta-inner p  { color: rgba(250,249,246,0.72); }

    /* Testimonial placeholders on beige bg */
    /* already white cards so text-muted fine */

    /* Process steps on light bg */
    .process-step-title { color: var(--dark-navy); }
    .process-step-desc  { color: var(--text-muted); }
    .process-step-num   { color: var(--gold); }

    /* About section on light bg */
    .about-body  { color: var(--text-muted); }
    .about-pillar-text { color: var(--dark-navy); }

    /* Insight cards on light/beige bg */
    .insight-title   { color: var(--dark-navy); }
    .insight-excerpt { color: var(--text-muted); }
    .insight-meta    { color: var(--text-muted); }
    .insight-link    { color: var(--navy); }

    /* Service cards on light bg default */
    .service-title { color: var(--dark-navy); }
    .service-desc  { color: var(--text-muted); }
    .service-num   { color: rgba(31,58,95,0.12); }

    /* Service detail on light bg */
    .service-detail-title { color: var(--dark-navy); }
    .service-detail-body  { color: var(--text-muted); }
    .service-detail-label { color: var(--gold); }

    /* Contact items on light bg */
    .contact-item-label { color: var(--gold); }
    .contact-item-value { color: var(--dark-navy); }
    .form-label         { color: var(--navy); }

    /* Team cards on light bg */
    .team-name { color: var(--dark-navy); }
    .team-role { color: var(--gold); }
    .team-bio  { color: var(--text-muted); }

    /* Font consistency */
    h1, h2, h3, h4, .hero-headline,
    .service-title, .service-detail-title,
    .insight-title, .team-name,
    .process-step-title, .why-item-content h4,
    .industry-name, .vm-card h3,
    .about-badge-num, .hero-stat-value,
    .why-metric-val, .footer-brand-name {
      font-family: var(--font-display);
    }

    body, p, li, a, input, select, textarea, button,
    .lead, .about-body, .service-desc, .service-detail-body,
    .insight-excerpt, .insight-meta, .team-bio,
    .process-step-desc, .industry-desc, .why-item-content p,
    .contact-item-value, .footer-desc, .footer-col ul a,
    .eyebrow, .hero-sub, .form-label, .form-input,
    .btn, .service-tag {
      font-family: var(--font-body);
    }

  </style>
</head>

<body>

<!-- ══════════════════════════════════════════════
     NAVIGATION
══════════════════════════════════════════════ -->
<nav id="navbar">
  <div class="nav-inner">
    <a href="#" class="nav-logo" onclick="showPage('home')">
      <img src="data:image/png;base64,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" alt="WSA Logo" style="height:48px; width:auto; display:block;" />
      <div class="nav-logo-text">
        <span class="nav-logo-name">WideStrategy Advisors</span>
        <span class="nav-logo-tag">Where Capital Meets Strategy</span>
      </div>
    </a>
    <ul class="nav-links">
      <li><a href="#" onclick="showPage('home'); return false;">Home</a></li>
      <li><a href="#" onclick="showPage('about'); return false;">About</a></li>
      <li><a href="#" onclick="showPage('services'); return false;">Services</a></li>
      <li><a href="#" onclick="showPage('industries'); return false;">Industries</a></li>
      <li><a href="#" onclick="showPage('insights'); return false;">Insights</a></li>
      <li><a href="#" class="nav-cta" onclick="showPage('contact'); return false;">Book Consultation</a></li>
    </ul>
    <button class="hamburger" id="ham-btn" aria-label="Menu" onclick="toggleMenu()">
      <span></span><span></span><span></span>
    </button>
  </div>
</nav>

<div id="mobile-menu">
  <a href="#" onclick="showPage('home'); toggleMenu(); return false;">Home</a>
  <a href="#" onclick="showPage('about'); toggleMenu(); return false;">About Us</a>
  <a href="#" onclick="showPage('services'); toggleMenu(); return false;">Services</a>
  <a href="#" onclick="showPage('industries'); toggleMenu(); return false;">Industries</a>
  <a href="#" onclick="showPage('insights'); toggleMenu(); return false;">Insights</a>
  <a href="#" onclick="showPage('contact'); toggleMenu(); return false;">Contact</a>
</div>

<!-- ══════════════════════════════════════════════
     HOME PAGE
══════════════════════════════════════════════ -->
<div id="page-home" class="page-section active">

  <!-- HERO -->
  <section id="hero">
    <div class="hero-bg-pattern"></div>
    <div class="hero-accent"></div>
    <div class="hero-accent-2"></div>
    <div class="hero-inner">
      <div class="hero-content">
        <span class="hero-eyebrow">Strategic &amp; Content Advisory · Est. 2025, India</span>
        <h1 class="hero-headline">
          Strategic Financial &amp; Business Advisory for <em>Growth-Focused</em> Enterprises
        </h1>
        <p class="hero-sub">
          We advise mid-sized companies, family offices, and high-growth enterprises on capital raising, transaction structuring, strategic communications, ESG integration, and cross-border expansion. We deliver institutional-grade counsel with the precision and accountability of a boutique practice.
        </p>
        <div class="hero-actions">
          <a href="#" class="btn btn-primary" onclick="showPage('contact'); return false;">
            Book a Consultation
            <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M5 12h14M12 5l7 7-7 7"/></svg>
          </a>
          <a href="#" class="btn btn-outline" onclick="showPage('services'); return false;">Explore Services</a>
        </div>
      </div>
    </div>
  </section>

  <!-- TICKER -->
  <div class="ticker-bar">
    <div class="ticker-inner">
      <span class="ticker-item">Debt Fundraising <span>·</span></span>
      <span class="ticker-item">Equity Capital Raising <span>·</span></span>
      <span class="ticker-item">Transaction Advisory <span>·</span></span>
      <span class="ticker-item">ESG &amp; Sustainability Consulting <span>·</span></span>
      <span class="ticker-item">Family Office Solutions <span>·</span></span>
      <span class="ticker-item">NRI &amp; Cross-Border Advisory <span>·</span></span>
      <span class="ticker-item">Wealth Management <span>·</span></span>
      <span class="ticker-item">Strategic Business Advisory <span>·</span></span>
      <span class="ticker-item">Debt Fundraising <span>·</span></span>
      <span class="ticker-item">Equity Capital Raising <span>·</span></span>
      <span class="ticker-item">Transaction Advisory <span>·</span></span>
      <span class="ticker-item">ESG &amp; Sustainability Consulting <span>·</span></span>
      <span class="ticker-item">Family Office Solutions <span>·</span></span>
      <span class="ticker-item">NRI &amp; Cross-Border Advisory <span>·</span></span>
      <span class="ticker-item">Wealth Management <span>·</span></span>
      <span class="ticker-item">Strategic Business Advisory <span>·</span></span>
    </div>
  </div>

  <!-- ABOUT PREVIEW -->
  <section class="section">
    <div class="container">
      <div class="about-grid">
        <div class="about-visual fade-up">
          <div class="about-img-frame">
            <div class="about-img-inner"></div>
            <img src="data:image/png;base64,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" alt="WideStrategy Advisors Logo" style="width:60%; opacity:0.85; position:relative; z-index:1;" />
          </div>
          <div class="about-badge">
            <div class="about-badge-num">2025</div>
            <div class="about-badge-label">Year Founded</div>
          </div>
        </div>
        <div class="about-content fade-up">
          <span class="eyebrow">About the Firm</span>
          <div class="gold-rule"></div>
          <h2 style="color:var(--dark-navy); font-family:'Cormorant Garamond', Georgia, serif;; margin-bottom:24px;">A Trusted Partner Through Every Stage of Growth</h2>
          <p class="about-body">
            WideStrategy Advisors LLP is a Gurugram-based boutique advisory firm serving ambitious enterprises, family offices, and growth-stage businesses. We operate at the intersection of capital markets, strategic planning, corporate communications, and governance, bringing institutional rigour to every engagement.
          </p>
          <p class="about-body">
            Our founding partners bring together expertise from Nestlé, PricewaterhouseCoopers, and McKinsey &amp; Company. We combine financial advisory depth with editorial precision, enabling us to serve clients across the full spectrum of strategic, financial, and communications needs. We are advisors, not product sellers.
          </p>
          <div class="about-pillars">
            <div class="about-pillar">
              <div class="about-pillar-icon">
                <svg viewBox="0 0 24 24"><path d="M12 2L2 7l10 5 10-5-10-5zM2 17l10 5 10-5M2 12l10 5 10-5"/></svg>
              </div>
              <span class="about-pillar-text">Institutional-Grade Advisory</span>
            </div>
            <div class="about-pillar">
              <div class="about-pillar-icon">
                <svg viewBox="0 0 24 24"><path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2M9 11a4 4 0 1 0 0-8 4 4 0 0 0 0 8zM23 21v-2a4 4 0 0 0-3-3.87M16 3.13a4 4 0 0 1 0 7.75"/></svg>
              </div>
              <span class="about-pillar-text">Dedicated Relationship Team</span>
            </div>
            <div class="about-pillar">
              <div class="about-pillar-icon">
                <svg viewBox="0 0 24 24"><circle cx="12" cy="12" r="10"/><path d="M12 8v4l3 3"/></svg>
              </div>
              <span class="about-pillar-text">End-to-End Execution</span>
            </div>
            <div class="about-pillar">
              <div class="about-pillar-icon">
                <svg viewBox="0 0 24 24"><path d="M3 3h18v18H3z"/><path d="M8 12h8M12 8v8"/></svg>
              </div>
              <span class="about-pillar-text">Pan-India &amp; Cross-Border Reach</span>
            </div>
          </div>
          <a href="#" class="btn btn-outline-dark" onclick="showPage('about'); return false;">Our Story &amp; Leadership</a>
        </div>
      </div>
    </div>
  </section>

  <!-- SERVICES GRID -->
  <section class="section section--beige">
    <div class="container">
      <div class="section-header section-header--centre fade-up">
        <span class="eyebrow">Our Practice Areas</span>
        <div class="gold-rule"></div>
        <h2 style="color:var(--dark-navy); font-family:'Cormorant Garamond', Georgia, serif;;">Nine Practice Areas. One Trusted Adviser.</h2>
        <p class="lead" style="margin: 16px auto 0;">From structuring your first debt raise to advising your family office, we cover the complete spectrum of strategic and financial needs.</p>
      </div>
      <div class="services-grid" style="grid-template-columns: repeat(3, 1fr);">
        <div class="service-card fade-up">
          <div class="service-num">01</div>
          <div class="service-title">Enterprise Financing</div>
          <p class="service-desc">Capital expenditure and working capital funding, trade financing, term loans, debt refinancing, supply chain financing, and structured trade and commodity finance.</p>
        </div>
        <div class="service-card fade-up">
          <div class="service-num">02</div>
          <div class="service-title">Business Advisory</div>
          <p class="service-desc">Equity and debt structuring for startups and mature businesses, equity raising, route-to-market strategy, omni-channel advisory, mergers and acquisitions, GIFT City advisory, and ESG certification.</p>
        </div>
        <div class="service-card fade-up">
          <div class="service-num">03</div>
          <div class="service-title">Transaction Advisory</div>
          <p class="service-desc">Financial and organisational due diligence, buy-side and sell-side M&amp;A process management, transaction structuring, valuations, and deal execution support.</p>
        </div>
        <div class="service-card fade-up">
          <div class="service-num">04</div>
          <div class="service-title">Wealth Creation</div>
          <p class="service-desc">Investment advisory for individuals and family offices across insurance, listed equities, debt instruments, alternative investment funds, and overseas assets. Dedicated advisory for NRI banking and investment.</p>
        </div>
        <div class="service-card fade-up">
          <div class="service-num">05</div>
          <div class="service-title">Financial Value Engineering</div>
          <p class="service-desc">Cost optimisation, restructuring for efficiency and cost reduction, and financial process improvement for growing enterprises.</p>
        </div>
        <div class="service-card fade-up">
          <div class="service-num">06</div>
          <div class="service-title">Family Office Solutions</div>
          <p class="service-desc">Governance frameworks, succession planning, multi-asset oversight, inter-generational wealth transfer, and structured advisory for family-run enterprises.</p>
        </div>
        <div class="service-card fade-up">
          <div class="service-num">07</div>
          <div class="service-title">ESG &amp; Sustainability</div>
          <p class="service-desc">ESG framework design, BRSR compliance, sustainable investing certification, net-zero roadmaps, and responsible business advisory aligned with regulatory requirements.</p>
        </div>
        <div class="service-card fade-up">
          <div class="service-num">08</div>
          <div class="service-title">NRI &amp; Cross-Border Advisory</div>
          <p class="service-desc">Advisory on India market entry for overseas businesses, overseas expansion for Indian companies, FEMA compliance, repatriation structuring, and FDI and ODI advisory.</p>
        </div>
        <div class="service-card fade-up">
          <div class="service-num">09</div>
          <div class="service-title">Content Strategy &amp; Communications</div>
          <p class="service-desc">Integrated brand positioning, investor collateral, sales enablement, editorial governance, and communications advisory for enterprises, MSMEs, and independent practitioners.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- WHY CHOOSE US -->
  <section class="section section--navy">
    <div class="container">
      <div class="why-grid">
        <div class="fade-up">
          <span class="eyebrow">Why WideStrategy</span>
          <div class="gold-rule"></div>
          <h2 style="color:var(--off-white); font-family:'Cormorant Garamond', Georgia, serif;; margin-bottom:40px;">We Earn Trust One Mandate at a Time</h2>
          <div class="why-list">
            <div class="why-item">
              <div class="why-item-num" style="color:rgba(214,185,140,0.4);">I</div>
              <div class="why-item-content">
                <h4>Deep Domain Expertise</h4>
                <p>Decades of combined experience across investment banking, credit markets, strategic consulting, and institutional communications, drawn from Nestlé, PricewaterhouseCoopers, and McKinsey and Company.</p>
              </div>
            </div>
            <div class="why-item">
              <div class="why-item-num" style="color:rgba(214,185,140,0.4);">II</div>
              <div class="why-item-content">
                <h4>Truly Personalised Advisory</h4>
                <p>No junior analysts. You engage directly with senior partners who have accountability for outcomes, not just deliverables.</p>
              </div>
            </div>
            <div class="why-item">
              <div class="why-item-num" style="color:rgba(214,185,140,0.4);">III</div>
              <div class="why-item-content">
                <h4>Extensive Industry Network</h4>
                <p>Established relationships across lenders, private equity and venture capital funds, and regulatory bodies, as well as a global network of partner advisers, translated into meaningful introductions and access for our clients.</p>
              </div>
            </div>
            <div class="why-item">
              <div class="why-item-num" style="color:rgba(214,185,140,0.4);">IV</div>
              <div class="why-item-content">
                <h4>Independence &amp; Objectivity</h4>
                <p>We are fee-based advisors with no product bias. Our counsel is shaped entirely by what is optimal for your business, nothing else.</p>
              </div>
            </div>
          </div>
        </div>
        <div class="why-visual fade-up">
          <div class="why-metric">
            <div style="width:44px; height:44px; background:rgba(214,185,140,0.15); border-radius:50%; display:flex; align-items:center; justify-content:center; flex-shrink:0;">
              <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="var(--gold)" stroke-width="1.5"><path d="M9 12l2 2 4-4M7.835 4.697a3.42 3.42 0 001.946-.806 3.42 3.42 0 014.438 0 3.42 3.42 0 001.946.806 3.42 3.42 0 013.138 3.138 3.42 3.42 0 00.806 1.946 3.42 3.42 0 010 4.438 3.42 3.42 0 00-.806 1.946 3.42 3.42 0 01-3.138 3.138 3.42 3.42 0 00-1.946.806 3.42 3.42 0 01-4.438 0 3.42 3.42 0 00-1.946-.806 3.42 3.42 0 01-3.138-3.138 3.42 3.42 0 00-.806-1.946 3.42 3.42 0 010-4.438 3.42 3.42 0 00.806-1.946 3.42 3.42 0 013.138-3.138z"/></svg>
            </div>
            <div class="why-metric-info">
              <div class="why-metric-label">Multi-Decade Institutional Pedigree</div>
              <div class="why-metric-sub">Nestlé, PricewaterhouseCoopers, McKinsey and Company</div>
            </div>
          </div>
          <div class="why-metric">
            <div style="width:44px; height:44px; background:rgba(214,185,140,0.15); border-radius:50%; display:flex; align-items:center; justify-content:center; flex-shrink:0;">
              <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="var(--gold)" stroke-width="1.5"><path d="M17 21v-2a4 4 0 00-4-4H5a4 4 0 00-4 4v2M9 11a4 4 0 100-8 4 4 0 000 8zM23 21v-2a4 4 0 00-3-3.87M16 3.13a4 4 0 010 7.75"/></svg>
            </div>
            <div class="why-metric-info">
              <div class="why-metric-label">Direct Partner Engagement</div>
              <div class="why-metric-sub">Every client works directly with a founding partner, not a delegated analyst</div>
            </div>
          </div>
          <div class="why-metric">
            <div style="width:44px; height:44px; background:rgba(214,185,140,0.15); border-radius:50%; display:flex; align-items:center; justify-content:center; flex-shrink:0;">
              <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="var(--gold)" stroke-width="1.5"><circle cx="12" cy="12" r="10"/><path d="M2 12h20M12 2a15.3 15.3 0 010 20M12 2a15.3 15.3 0 000 20"/></svg>
            </div>
            <div class="why-metric-info">
              <div class="why-metric-label">Global Reach, Boutique Accountability</div>
              <div class="why-metric-sub">A partner network spanning India, the US, Europe, and the Gulf</div>
            </div>
          </div>
          <div class="why-metric">
            <div style="width:44px; height:44px; background:rgba(214,185,140,0.15); border-radius:50%; display:flex; align-items:center; justify-content:center; flex-shrink:0;">
              <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="var(--gold)" stroke-width="1.5"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg>
            </div>
            <div class="why-metric-info">
              <div class="why-metric-label">Fee-Based, Conflict-Free Advisory</div>
              <div class="why-metric-sub">Independent counsel with no product bias and no hidden commission</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- PROCESS -->
  <section class="section">
    <div class="container">
      <div class="section-header section-header--centre fade-up">
        <span class="eyebrow">Our Approach</span>
        <div class="gold-rule"></div>
        <h2 style="color:var(--dark-navy); font-family:'Cormorant Garamond', Georgia, serif;;">A Structured Path to Your Objectives</h2>
        <p class="lead" style="margin: 16px auto 0;">Every engagement follows a disciplined five-stage process, transparent, collaborative, and results-driven.</p>
      </div>
      <div class="process-track fade-up">
        <div class="process-step">
          <div class="process-dot"><div class="process-dot-inner"></div></div>
          <div class="process-step-num">Stage 01</div>
          <div class="process-step-title">Consultation</div>
          <p class="process-step-desc">A focused discovery session to understand your goals, constraints, and capital requirements.</p>
        </div>
        <div class="process-step">
          <div class="process-dot"><div class="process-dot-inner"></div></div>
          <div class="process-step-num">Stage 02</div>
          <div class="process-step-title">Assessment</div>
          <p class="process-step-desc">Rigorous financial and strategic analysis of your business, identifying risks, opportunities, and optimal pathways.</p>
        </div>
        <div class="process-step">
          <div class="process-dot"><div class="process-dot-inner"></div></div>
          <div class="process-step-num">Stage 03</div>
          <div class="process-step-title">Strategy</div>
          <p class="process-step-desc">A bespoke advisory plan, transaction structure, or capital blueprint aligned with your objectives and timeline.</p>
        </div>
        <div class="process-step">
          <div class="process-dot"><div class="process-dot-inner"></div></div>
          <div class="process-step-num">Stage 04</div>
          <div class="process-step-title">Execution</div>
          <p class="process-step-desc">Hands-on management of the transaction, process, or implementation, with clear milestones and accountability.</p>
        </div>
        <div class="process-step">
          <div class="process-dot"><div class="process-dot-inner"></div></div>
          <div class="process-step-num">Stage 05</div>
          <div class="process-step-title">Ongoing Support</div>
          <p class="process-step-desc">Post-close monitoring, covenant management, and continued advisory as your business evolves.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- INSIGHTS PREVIEW -->
  <section class="section section--beige">
    <div class="container">
      <div class="section-header fade-up" style="display:flex; align-items:flex-end; justify-content:space-between; flex-wrap:wrap; gap:20px;">
        <div>
          <span class="eyebrow">Thought Leadership</span>
          <div class="gold-rule"></div>
          <h2 style="color:var(--dark-navy); font-family:'Cormorant Garamond', Georgia, serif;;">Insights &amp; Perspectives</h2>
        </div>
        
      </div>
      <div class="fade-up" style="text-align:center; padding:64px 32px; background:rgba(31,58,95,0.04); border:1px solid var(--border); border-radius:2px;">
        <div style="font-family:var(--font-display); font-size:48px; color:rgba(31,58,95,0.12); margin-bottom:20px;">✦</div>
        <h3 style="color:var(--dark-navy); margin-bottom:12px; font-size:24px;">Insights Coming Soon</h3>
        <p style="color:var(--text-muted); font-size:15px; max-width:480px; margin:0 auto; line-height:1.75;">Our partners are currently working on a series of articles covering capital markets, ESG strategy, family office governance, and cross-border advisory. Check back soon.</p>
      </div>
    </div>
  </section>



  <!-- FINAL CTA -->
  <section class="cta-section">
    <div class="cta-accent"></div>
    <div class="cta-inner fade-up">
      <span class="eyebrow" style="color:var(--gold); display:block; text-align:center;">Ready to Begin?</span>
      <h2>We invite you to Build Your Next Chapter Together</h2>
      <p>Schedule a complimentary 45-minute consultation with our senior advisors. No obligations, no product pitches, just honest, expert counsel.</p>
      <div class="cta-actions">
        <a href="#" class="btn btn-primary" onclick="showPage('contact'); return false;">
          Book a Consultation
          <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M5 12h14M12 5l7 7-7 7"/></svg>
        </a>
        <a href="#" class="btn btn-outline" onclick="showPage('services'); return false;">Explore Our Services</a>
      </div>
    </div>
  </section>
</div>

<!-- ══════════════════════════════════════════════
     ABOUT PAGE
══════════════════════════════════════════════ -->
<div id="page-about" class="page-section">
  <div class="page-header">
    <div class="page-header-bg"></div>
    <div class="page-header-inner">
      <span class="eyebrow">About WideStrategy Advisors</span>
      <h1>A Boutique Firm With Institutional Depth</h1>
      <p>Founded on the belief that mid-market businesses deserve the same quality of advisory as large corporates, delivered personally, not by committee.</p>
    </div>
  </div>

  <!-- Company Overview -->
  <section class="section">
    <div class="container">
      <div class="about-grid">
        <div class="about-visual fade-up">
          <div class="about-img-frame" style="aspect-ratio:1;">
            <div class="about-img-inner"></div>
            <img src="data:image/png;base64,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" alt="WideStrategy Advisors Logo" style="width:55%; opacity:0.85; position:relative; z-index:1;" />
          </div>
        </div>
        <div class="about-content fade-up">
          <span class="eyebrow">Our Story</span>
          <div class="gold-rule"></div>
          <h2 style="color:var(--dark-navy); font-family:'Cormorant Garamond', Georgia, serif;; margin-bottom:24px; font-family:'Cormorant Garamond', Georgia, serif;">Built on Relationships. Driven by Results.</h2>
          <p class="about-body">WideStrategy Advisors LLP was established in Gurugram with a singular purpose: to provide India's ambitious mid-market enterprises access to world-class financial and strategic advisory, without the impersonality of large institutions.</p>
          <p class="about-body">Over the years, we have advised manufacturers, exporters, family businesses, and technology ventures across their most critical inflection points, capital raises, acquisitions, strategic pivots, and succession planning.</p>
          <p class="about-body">Our partners bring experience from leading investment banks, credit funds, and consulting practices. What sets us apart is not our pedigree, but our commitment: we stay engaged from strategy through execution, and we measure success by our clients' outcomes, not our fees.</p>
          <p class="about-body">We are registered as a Non-Banking Financial Company (NBFC) category-I Merchant Banker with SEBI, and operate with the highest standards of fiduciary responsibility.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Vision & Mission -->
  <section class="section section--beige">
    <div class="container">
      <div class="section-header section-header--centre fade-up">
        <span class="eyebrow">Our Purpose</span>
        <div class="gold-rule"></div>
        <h2 style="color:var(--dark-navy); font-family:'Cormorant Garamond', Georgia, serif;; font-family:'Cormorant Garamond', Georgia, serif;">Vision &amp; Mission</h2>
      </div>
      <div class="vm-grid fade-up">
        <div class="vm-card vm-card--vision">
          <span class="vm-card-label">Vision</span>
          <h3>To be the most trusted strategic partner for India's emerging champions</h3>
          <p>We envision a future where every ambitious Indian enterprise, regardless of size, has access to the calibre of advice that drives transformative, sustainable growth.</p>
        </div>
        <div class="vm-card vm-card--mission">
          <span class="vm-card-label">Mission</span>
          <h3>Deliver honest, expert-led advisory that creates measurable value</h3>
          <p>We are committed to bringing intellectual rigour, ethical practice, and genuine partnership to every engagement, ensuring our clients navigate complexity with confidence.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Leadership Team -->
  <section class="section">
    <div class="container">
      <div class="section-header section-header--centre fade-up">
        <span class="eyebrow">Leadership</span>
        <div class="gold-rule"></div>
        <h2 style="color:var(--dark-navy); font-family:'Cormorant Garamond', Georgia, serif;;">Partners &amp; Senior Advisors</h2>
        <p class="lead" style="margin: 16px auto 0;">Our founding partners bring together over six decades of combined expertise spanning corporate strategy, financial advisory, chartered accountancy, and institutional communications.</p>
      </div>
      <div style="display:grid; grid-template-columns: 1fr 1fr; gap:32px;" class="team-founders-grid">

        <!-- Kingshuk Ghosh -->
        <div class="team-card fade-up" style="display:flex; flex-direction:column;">
          <div class="team-photo" style="height:220px;">
            <span class="team-photo-initials">KG</span>
            <div style="position:absolute; bottom:0; left:0; right:0; height:3px; background:var(--gold);"></div>
          </div>
          <div class="team-body" style="flex:1; display:flex; flex-direction:column; gap:0;">
            <div class="team-name">Kingshuk Ghosh</div>
            <div class="team-role">Co-Founder &amp; Partner, Strategy &amp; Financial Advisory</div>

            <div style="display:flex; flex-wrap:wrap; gap:8px; margin:14px 0 18px;">
              <span style="padding:4px 12px; background:var(--beige); border-radius:20px; font-size:11px; font-weight:600; color:var(--navy); letter-spacing:0.04em;">Chartered Accountant</span>
              <span style="padding:4px 12px; background:var(--beige); border-radius:20px; font-size:11px; font-weight:600; color:var(--navy); letter-spacing:0.04em;">Independent Director</span>
              <span style="padding:4px 12px; background:var(--beige); border-radius:20px; font-size:11px; font-weight:600; color:var(--navy); letter-spacing:0.04em;">40+ Years Experience</span>
            </div>

            <p class="team-bio">Kingshuk Ghosh is a seasoned strategist and financial advisor whose 40-year career spans two of the world's most demanding organisations, Nestlé and PricewaterhouseCoopers. Over 32 years at Nestlé, he held senior leadership roles across strategy, finance, and capability building, developing deep expertise in operating at scale within complex, multi-market environments.</p>

            <p class="team-bio" style="margin-top:12px;">A Fellow Chartered Accountant and Independent Director, Kingshuk also serves as Partner at S.N. Guha &amp; Co., a respected Chartered Accountancy firm, bringing the dual advantage of board-level strategic counsel and rigorous financial governance to every engagement.</p>

            <p class="team-bio" style="margin-top:12px;">At WideStrategy Advisors, he leads on strategy, business advisory, and capability development, helping enterprises make better decisions, build stronger organisations, and navigate complex transitions with confidence.</p>

            <div style="margin-top:20px; padding-top:20px; border-top:1px solid var(--border);">
              <div style="font-size:11px; font-weight:600; letter-spacing:0.12em; text-transform:uppercase; color:var(--gold); margin-bottom:10px;">Affiliations</div>
              <div style="font-size:13px; color:var(--text-muted); line-height:1.8;">
                Nestlé India &amp; Group (32 years) &nbsp;·&nbsp; PricewaterhouseCoopers &nbsp;·&nbsp; S.N. Guha &amp; Co. (Partner)
              </div>
            </div>
          </div>
        </div>

        <!-- Paromita Ghosh -->
        <div class="team-card fade-up" style="display:flex; flex-direction:column;">
          <div class="team-photo" style="height:220px;">
            <span class="team-photo-initials">PG</span>
            <div style="position:absolute; bottom:0; left:0; right:0; height:3px; background:var(--gold);"></div>
          </div>
          <div class="team-body" style="flex:1; display:flex; flex-direction:column; gap:0;">
            <div class="team-name">Paromita Ghosh</div>
            <div class="team-role">Co-Founder &amp; Partner, Communications &amp; Editorial Strategy</div>

            <div style="display:flex; flex-wrap:wrap; gap:8px; margin:14px 0 18px;">
              <span style="padding:4px 12px; background:var(--beige); border-radius:20px; font-size:11px; font-weight:600; color:var(--navy); letter-spacing:0.04em;">Communications Specialist</span>
              <span style="padding:4px 12px; background:var(--beige); border-radius:20px; font-size:11px; font-weight:600; color:var(--navy); letter-spacing:0.04em;">McKinsey &amp; Co. Alumni</span>
              <span style="padding:4px 12px; background:var(--beige); border-radius:20px; font-size:11px; font-weight:600; color:var(--navy); letter-spacing:0.04em;">30 Years Experience</span>
            </div>

            <p class="team-bio">Paromita Ghosh is a communications strategist with nearly three decades of experience shaping how complex ideas are expressed, understood, and trusted. As Senior Copy Editor at McKinsey &amp; Company for 18 years, she was responsible for the accuracy, clarity, and quality of the firm's global digital publications, spanning articles, podcasts, and interactive content.</p>

            <p class="team-bio" style="margin-top:12px;">She played a defining role in McKinsey Editorial's transition from print to digital publishing, a transformation that demanded both institutional rigour and an acute sensitivity to evolving communication norms. Her work touched media organisations, industry bodies, and firms in the software and strategy consulting segments.</p>

            <p class="team-bio" style="margin-top:12px;">At WideStrategy Advisors, Paromita leads on client communications, editorial quality, and brand voice, ensuring that the firm's counsel is expressed with the same precision and credibility that it is delivered with.</p>

            <div style="margin-top:20px; padding-top:20px; border-top:1px solid var(--border);">
              <div style="font-size:11px; font-weight:600; letter-spacing:0.12em; text-transform:uppercase; color:var(--gold); margin-bottom:10px;">Specialisations</div>
              <div style="font-size:13px; color:var(--text-muted); line-height:1.8;">
                Editorial Strategy &nbsp;·&nbsp; Digital Publishing &nbsp;·&nbsp; Corporate Communications &nbsp;·&nbsp; Fact-Checking &amp; Accuracy &nbsp;·&nbsp; Freelance Advisory
              </div>
            </div>
          </div>
        </div>

      </div>

      <!-- More partners note -->
      <div class="fade-up" style="margin-top:32px; padding:28px 32px; background:var(--beige); border-radius:2px; display:flex; align-items:center; justify-content:space-between; flex-wrap:wrap; gap:16px;">
        <div>
          <div style="font-size:13px; font-weight:600; color:var(--dark-navy); margin-bottom:4px;">Growing Leadership Team</div>
          <div style="font-size:13px; color:var(--text-muted);">Additional partners and senior advisors will be joining WideStrategy Advisors, watch this space.</div>
        </div>
        <a href="#" class="btn btn-outline-dark" style="white-space:nowrap;" onclick="showPage('contact'); return false;">Get in Touch</a>
      </div>
    </div>
  </section>
</div>

<!-- ══════════════════════════════════════════════
     SERVICES PAGE
══════════════════════════════════════════════ -->
<div id="page-services" class="page-section">
  <div class="page-header">
    <div class="page-header-bg"></div>
    <div class="page-header-inner">
      <span class="eyebrow">Our Services</span>
      <h1>The Complete Advisory Spectrum</h1>
      <p>Nine integrated practice areas designed to meet every financial, strategic, and communications need of a growth-focused enterprise.</p>
    </div>
  </div>

  <section class="section">
    <div class="container">

      <div class="service-detail fade-up">
        <div class="service-detail-grid">
          <div>
            <div class="service-detail-label">Service 01</div>
            <div class="service-detail-title">Enterprise Financing</div>
          </div>
          <div>
            <p class="service-detail-body">We advise businesses at every stage on the full spectrum of debt and financing instruments. Whether the requirement is working capital, capital expenditure financing, trade credit, or a structured debt facility, we work with a broad network of PSU banks, private banks, NBFCs, and alternative credit providers to identify the most appropriate and cost-efficient solution.</p>
            <p class="service-detail-body">Our team prepares information memoranda, financial models, and lender presentations, managing the complete process from lender identification through to sanction and disbursement.</p>
            <div class="service-tags">
              <span class="service-tag">Capital Expenditure Financing</span>
              <span class="service-tag">Working Capital</span>
              <span class="service-tag">Trade Financing</span>
              <span class="service-tag">Term Loans</span>
              <span class="service-tag">Debt Refinancing</span>
              <span class="service-tag">Supply Chain Financing</span>
              <span class="service-tag">Structured Trade Finance</span>
            </div>
          </div>
        </div>
      </div>

      <div class="service-detail fade-up">
        <div class="service-detail-grid">
          <div>
            <div class="service-detail-label">Service 02</div>
            <div class="service-detail-title">Business Advisory</div>
          </div>
          <div>
            <p class="service-detail-body">We advise entrepreneurs, promoters, and management teams on equity and debt structuring, capital raising, and strategic business decisions. Our advisory spans early-stage startups through to mature enterprises, covering investor outreach, route-to-market planning, omni-channel strategy, trading terms architecture, and mergers and acquisitions.</p>
            <p class="service-detail-body">We also advise overseas businesses seeking to establish operations in India and Indian companies pursuing international expansion, including GIFT City structures and taxation advisory.</p>
            <div class="service-tags">
              <span class="service-tag">Equity Raising Advisory</span>
              <span class="service-tag">Debt Structuring</span>
              <span class="service-tag">Route-to-Market Strategy</span>
              <span class="service-tag">Omni-Channel Advisory</span>
              <span class="service-tag">Trading Terms Architecture</span>
              <span class="service-tag">Mergers &amp; Acquisitions</span>
              <span class="service-tag">GIFT City Advisory</span>
              <span class="service-tag">Taxation Advisory</span>
            </div>
          </div>
        </div>
      </div>

      <div class="service-detail fade-up">
        <div class="service-detail-grid">
          <div>
            <div class="service-detail-label">Service 03</div>
            <div class="service-detail-title">Transaction Advisory</div>
          </div>
          <div>
            <p class="service-detail-body">We provide end-to-end M&amp;A advisory for business acquisitions, strategic divestitures, joint ventures, and business restructuring, on both buy-side and sell-side mandates. Our transaction team handles valuation, due diligence, structuring, negotiation support, and regulatory coordination.</p>
            <div class="service-tags">
              <span class="service-tag">Buy-Side M&amp;A</span>
              <span class="service-tag">Sell-Side M&amp;A</span>
              <span class="service-tag">Business Valuations</span>
              <span class="service-tag">Joint Ventures</span>
              <span class="service-tag">Business Restructuring</span>
              <span class="service-tag">Promoter Buyouts</span>
            </div>
          </div>
        </div>
      </div>

      <div class="service-detail fade-up">
        <div class="service-detail-grid">
          <div>
            <div class="service-detail-label">Service 04</div>
            <div class="service-detail-title">Wealth Creation</div>
          </div>
          <div>
            <p class="service-detail-body">We provide investment advisory for high-net-worth individuals, promoters, and family offices across a broad asset class spectrum. Our counsel is independent, unbiased, and shaped entirely by the client's financial objectives, time horizon, and risk profile.</p>
            <p class="service-detail-body">We also provide dedicated advisory to NRIs on banking structures and investment options in India, navigating FEMA regulations and applicable compliance requirements.</p>
            <div class="service-tags">
              <span class="service-tag">Family Office Investment Advisory</span>
              <span class="service-tag">Listed Equities</span>
              <span class="service-tag">Debt Instruments</span>
              <span class="service-tag">Alternative Investment Funds</span>
              <span class="service-tag">Overseas Investments</span>
              <span class="service-tag">Insurance Advisory</span>
              <span class="service-tag">NRI Banking &amp; Investment</span>
            </div>
          </div>
        </div>
      </div>

      <div class="service-detail fade-up">
        <div class="service-detail-grid">
          <div>
            <div class="service-detail-label">Service 05</div>
            <div class="service-detail-title">Financial Value Engineering</div>
          </div>
          <div>
            <p class="service-detail-body">We work with management teams to identify and implement cost optimisation opportunities and structural improvements that enhance operating efficiency. Our financial value engineering practice applies analytical rigour to cost base reviews, organisational design, and process redesign, with a focus on sustainable cost reduction rather than short-term measures.</p>
            <div class="service-tags">
              <span class="service-tag">Cost Optimisation</span>
              <span class="service-tag">Efficiency Restructuring</span>
              <span class="service-tag">Cost Reduction Advisory</span>
              <span class="service-tag">Organisational Due Diligence</span>
              <span class="service-tag">Process Improvement</span>
            </div>
          </div>
        </div>
      </div>

      <div class="service-detail fade-up">
        <div class="service-detail-grid">
          <div>
            <div class="service-detail-label">Service 06</div>
            <div class="service-detail-title">Family Office Solutions</div>
          </div>
          <div>
            <p class="service-detail-body">For family-run enterprises and high-net-worth families, we provide structured advisory on governance, succession planning, and inter-generational wealth transfer. We help families establish clear governance frameworks, separate business assets from personal wealth, and plan for leadership transitions in a structured and equitable manner.</p>
            <p class="service-detail-body">Our family office practice also covers multi-asset portfolio oversight and philanthropic advisory for families seeking to formalise their charitable objectives.</p>
            <div class="service-tags">
              <span class="service-tag">Family Governance</span>
              <span class="service-tag">Succession Planning</span>
              <span class="service-tag">Family Constitution</span>
              <span class="service-tag">Multi-Asset Oversight</span>
              <span class="service-tag">Inter-Generational Wealth Transfer</span>
              <span class="service-tag">Philanthropic Advisory</span>
            </div>
          </div>
        </div>
      </div>

      <div class="service-detail fade-up">
        <div class="service-detail-grid">
          <div>
            <div class="service-detail-label">Service 07</div>
            <div class="service-detail-title">ESG &amp; Sustainability</div>
          </div>
          <div>
            <p class="service-detail-body">Sustainability is a prerequisite for accessing institutional capital, winning enterprise contracts, and meeting evolving regulatory requirements. We help businesses design credible ESG frameworks, prepare BRSR disclosures, obtain sustainable investing certification, develop net-zero roadmaps, and communicate progress to investors and stakeholders.</p>
            <div class="service-tags">
              <span class="service-tag">ESG Framework Design</span>
              <span class="service-tag">BRSR Compliance</span>
              <span class="service-tag">Sustainable Investing Certification</span>
              <span class="service-tag">Sustainability Reporting</span>
              <span class="service-tag">Net-Zero Roadmaps</span>
              <span class="service-tag">Green Finance</span>
              <span class="service-tag">Stakeholder Communication</span>
            </div>
          </div>
        </div>
      </div>

      <div class="service-detail fade-up">
        <div class="service-detail-grid">
          <div>
            <div class="service-detail-label">Service 08</div>
            <div class="service-detail-title">NRI &amp; Cross-Border Advisory</div>
          </div>
          <div>
            <p class="service-detail-body">We advise Non-Resident Indians and international businesses on India market entry, FEMA compliance, repatriation structuring, and cross-border transactions. For Indian companies expanding globally, we provide strategic and regulatory guidance on international capital raising and foreign business operations.</p>
            <div class="service-tags">
              <span class="service-tag">FEMA Compliance</span>
              <span class="service-tag">NRI Investment Structuring</span>
              <span class="service-tag">Repatriation Planning</span>
              <span class="service-tag">India Market Entry</span>
              <span class="service-tag">FDI &amp; ODI Advisory</span>
              <span class="service-tag">Export Finance</span>
              <span class="service-tag">GIFT City Advisory</span>
            </div>
          </div>
        </div>
      </div>

      <div class="service-detail fade-up">
        <div class="service-detail-grid">
          <div>
            <div class="service-detail-label">Service 09</div>
            <div class="service-detail-title">Content Strategy &amp; Communications</div>
          </div>
          <div>
            <p class="service-detail-body">WideStrategy Advisors offers a dedicated content strategy and communications practice, drawing on nearly three decades of institutional editorial experience. We serve two distinct client segments: growing enterprises and MSMEs requiring integrated brand positioning and investor collateral, and independent practitioners and solopreneurs seeking to establish a credible professional presence.</p>
            <p class="service-detail-body">For businesses, we function as an end-to-end narrative partner. Our capabilities span investor pitch decks, board presentations, website copy, sales enablement materials, thought leadership content, and multi-format digital distribution. Every asset we produce passes through a rigorous editorial governance framework, guaranteeing factual accuracy, clarity, and consistency of voice.</p>
            <p class="service-detail-body">For independent practitioners, consultants, and freelancers, we offer structured positioning advisory and practical workshops designed to help solo operators define their message, organise their digital profiles, and maintain a sustainable approach to professional visibility without disrupting their client delivery.</p>

            <div style="display:grid; grid-template-columns:1fr 1fr; gap:24px; margin:28px 0;">
              <div style="padding:24px; background:var(--beige); border-radius:2px;">
                <div style="font-size:11px; font-weight:700; letter-spacing:0.14em; text-transform:uppercase; color:var(--gold); margin-bottom:12px;">For Enterprises &amp; MSMEs</div>
                <ul style="list-style:none; padding:0; display:flex; flex-direction:column; gap:8px;">
                  <li style="font-size:13px; color:var(--text-muted); padding-left:14px; position:relative;"><span style="position:absolute;left:0;color:var(--navy);">&#8250;</span> Investor pitch decks and board presentations</li>
                  <li style="font-size:13px; color:var(--text-muted); padding-left:14px; position:relative;"><span style="position:absolute;left:0;color:var(--navy);">&#8250;</span> Website copy and structural narrative mapping</li>
                  <li style="font-size:13px; color:var(--text-muted); padding-left:14px; position:relative;"><span style="position:absolute;left:0;color:var(--navy);">&#8250;</span> Sales decks, brochures, and B2B case studies</li>
                  <li style="font-size:13px; color:var(--text-muted); padding-left:14px; position:relative;"><span style="position:absolute;left:0;color:var(--navy);">&#8250;</span> LinkedIn and digital thought leadership content</li>
                  <li style="font-size:13px; color:var(--text-muted); padding-left:14px; position:relative;"><span style="position:absolute;left:0;color:var(--navy);">&#8250;</span> Executive newsletters and whitepapers</li>
                  <li style="font-size:13px; color:var(--text-muted); padding-left:14px; position:relative;"><span style="position:absolute;left:0;color:var(--navy);">&#8250;</span> Data visualisation and infographics</li>
                </ul>
              </div>
              <div style="padding:24px; background:var(--beige); border-radius:2px;">
                <div style="font-size:11px; font-weight:700; letter-spacing:0.14em; text-transform:uppercase; color:var(--gold); margin-bottom:12px;">For Independent Practitioners</div>
                <ul style="list-style:none; padding:0; display:flex; flex-direction:column; gap:8px;">
                  <li style="font-size:13px; color:var(--text-muted); padding-left:14px; position:relative;"><span style="position:absolute;left:0;color:var(--navy);">&#8250;</span> Positioning and profile foundations advisory</li>
                  <li style="font-size:13px; color:var(--text-muted); padding-left:14px; position:relative;"><span style="position:absolute;left:0;color:var(--navy);">&#8250;</span> Brand strategy workshops (group and 1:1 formats)</li>
                  <li style="font-size:13px; color:var(--text-muted); padding-left:14px; position:relative;"><span style="position:absolute;left:0;color:var(--navy);">&#8250;</span> Digital profile audit and optimisation</li>
                  <li style="font-size:13px; color:var(--text-muted); padding-left:14px; position:relative;"><span style="position:absolute;left:0;color:var(--navy);">&#8250;</span> Sustainable communications planning</li>
                  <li style="font-size:13px; color:var(--text-muted); padding-left:14px; position:relative;"><span style="position:absolute;left:0;color:var(--navy);">&#8250;</span> Message mapping and reputation alignment</li>
                  <li style="font-size:13px; color:var(--text-muted); padding-left:14px; position:relative;"><span style="position:absolute;left:0;color:var(--navy);">&#8250;</span> Strategic advisory sprints (focused 1:1 sessions)</li>
                </ul>
              </div>
            </div>

            <div style="padding:20px 24px; background:var(--navy); border-radius:2px; margin-bottom:24px;">
              <div style="font-size:11px; font-weight:700; letter-spacing:0.14em; text-transform:uppercase; color:var(--gold); margin-bottom:8px;">Editorial Governance</div>
              <p style="font-size:13.5px; color:rgba(250,249,246,0.82); line-height:1.7; margin:0; font-family:'Inter', sans-serif;">Every document, script, or content asset we produce passes through a multi-layer human editing and fact-checking process. This reflects our founding commitment to accuracy and protects the reputation of every client we serve.</p>
            </div>

            <div class="service-tags">
              <span class="service-tag">Integrated Retainer</span>
              <span class="service-tag">Production Sprints</span>
              <span class="service-tag">Investor Collateral</span>
              <span class="service-tag">Brand Positioning</span>
              <span class="service-tag">Editorial Governance</span>
              <span class="service-tag">Thought Leadership</span>
              <span class="service-tag">Solopreneur Advisory</span>
              <span class="service-tag">Brand Strategy Workshops</span>
            </div>
          </div>
        </div>
      </div>

    </div>
  </section>

  <section class="cta-section">
    <div class="cta-accent"></div>
    <div class="cta-inner fade-up">
      <span class="eyebrow" style="color:var(--gold); display:block; text-align:center;">Get Started</span>
      <h2>Not Sure Which Service Fits?</h2>
      <p>Our partners will assess your needs and recommend the right advisory approach, in a no-obligation consultation.</p>
      <div class="cta-actions">
        <a href="#" class="btn btn-primary" onclick="showPage('contact'); return false;">Book a Consultation</a>
      </div>
    </div>
  </section>
</div>

<!-- ══════════════════════════════════════════════
     INDUSTRIES PAGE
══════════════════════════════════════════════ -->
<div id="page-industries" class="page-section">
  <div class="page-header">
    <div class="page-header-bg"></div>
    <div class="page-header-inner">
      <span class="eyebrow">Industries We Serve</span>
      <h1>Sector Intelligence, Not Generic Advice</h1>
      <p>Our advisory is sharpened by deep sector familiarity, we understand the unique capital dynamics, regulatory landscape, and growth drivers of each industry we serve.</p>
    </div>
  </div>

  <section class="section section--dark">
    <div class="container">
      <div class="industries-grid fade-up">
        <div class="industry-card">
          <span class="industry-icon">🏭</span>
          <div class="industry-name">Manufacturing</div>
          <p class="industry-desc">Capex financing, working capital structuring, and growth advisory for Indian manufacturers.</p>
        </div>
        <div class="industry-card">
          <span class="industry-icon">📦</span>
          <div class="industry-name">Exporters</div>
          <p class="industry-desc">Export credit, FEMA advisory, cross-border transaction structuring, and forex risk management.</p>
        </div>
        <div class="industry-card">
          <span class="industry-icon">💻</span>
          <div class="industry-name">Technology &amp; Startups</div>
          <p class="industry-desc">Seed to pre-IPO fundraising, ESOP design, cap table advisory, and investor relations.</p>
        </div>
        <div class="industry-card">
          <span class="industry-icon">🛍️</span>
          <div class="industry-name">Consumer &amp; Retail</div>
          <p class="industry-desc">Brand acquisition advisory, retail expansion finance, and D2C growth capital.</p>
        </div>
        <div class="industry-card">
          <span class="industry-icon">🏛️</span>
          <div class="industry-name">Family-Owned Businesses</div>
          <p class="industry-desc">Governance structures, succession planning, professionalisation, and family wealth management.</p>
        </div>
      </div>
    </div>
  </section>

  <section class="section">
    <div class="container">
      <div class="section-header section-header--centre fade-up">
        <span class="eyebrow">Our Track Record</span>
        <div class="gold-rule"></div>
        <h2 style="color:var(--dark-navy); font-family:'Cormorant Garamond', Georgia, serif;;">Experience Across India's Growth Economy</h2>
        <p class="lead" style="margin: 16px auto 0;">We have executed mandates across sectors spanning ₹20 crore to ₹500 crore in transaction size, bringing the same quality of attention to each.</p>
      </div>
      <div style="display:grid; grid-template-columns: repeat(3, 1fr); gap:24px;" class="fade-up">
        <div style="padding:36px; background:var(--beige); border-radius:2px; text-align:center;">
          <div style="font-family:var(--font-display); font-size:48px; color:var(--navy); line-height:1; margin-bottom:12px;">₹20Cr–<br/>₹500Cr</div>
          <div style="font-size:13px; color:var(--text-muted); letter-spacing:0.04em;">Typical Transaction Range</div>
        </div>
        <div style="padding:36px; background:var(--beige); border-radius:2px; text-align:center;">
          <div style="font-family:var(--font-display); font-size:48px; color:var(--navy); line-height:1; margin-bottom:12px;">15+<br/>States</div>
          <div style="font-size:13px; color:var(--text-muted); letter-spacing:0.04em;">Geographic Footprint Across India</div>
        </div>
        <div style="padding:36px; background:var(--beige); border-radius:2px; text-align:center;">
          <div style="font-family:var(--font-display); font-size:48px; color:var(--navy); line-height:1; margin-bottom:12px;">12+<br/>Sectors</div>
          <div style="font-size:13px; color:var(--text-muted); letter-spacing:0.04em;">Industries Served Since Inception</div>
        </div>
      </div>
    </div>
  </section>
</div>

<!-- ══════════════════════════════════════════════
     INSIGHTS PAGE
══════════════════════════════════════════════ -->
<div id="page-insights" class="page-section">
  <div class="page-header">
    <div class="page-header-bg"></div>
    <div class="page-header-inner">
      <span class="eyebrow">Insights &amp; Perspectives</span>
      <h1>Thought Leadership From the Field</h1>
      <p>Practical views on capital markets, strategy, regulation, and business, written by advisors who are active in these conversations every day.</p>
    </div>
  </div>

  <section class="section">
    <div class="container">
      <div class="fade-up" style="text-align:center; padding:96px 32px;">
        <div style="font-family:var(--font-display); font-size:64px; color:rgba(31,58,95,0.08); margin-bottom:24px; line-height:1;">WSA</div>
        <h3 style="color:var(--dark-navy); margin-bottom:16px;">Articles Coming Soon</h3>
        <p style="color:var(--text-muted); font-size:16px; max-width:560px; margin:0 auto 40px; line-height:1.8;">Our partners are preparing a series of thought leadership pieces on capital markets, ESG strategy, transaction advisory, family office governance, and cross-border finance. These will be published here as they are ready.</p>
        <a href="#" class="btn btn-outline-dark" onclick="showPage('contact'); return false;">Speak with Our Partners</a>
      </div>
    </div>
  </section>
</div>

<!-- ══════════════════════════════════════════════
     CONTACT PAGE
══════════════════════════════════════════════ -->
<div id="page-contact" class="page-section">
  <div class="page-header">
    <div class="page-header-bg"></div>
    <div class="page-header-inner">
      <span class="eyebrow">Get in Touch</span>
      <h1>Begin With a Conversation</h1>
      <p>Schedule a complimentary 45-minute consultation with our senior advisors. Confidential, obligation-free, and focused entirely on your needs.</p>
    </div>
  </div>

  <section class="section">
    <div class="container">
      <div class="contact-grid">
        <div class="fade-up">
          <span class="eyebrow">Contact Information</span>
          <div class="gold-rule"></div>
          <h3 style="color:var(--dark-navy); margin-bottom:32px;">Our Office</h3>

          <div class="contact-item">
            <div class="contact-icon">
              <svg viewBox="0 0 24 24" fill="none" stroke-width="1.5"><path d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z" stroke-linecap="round" stroke-linejoin="round"/><path d="M15 11a3 3 0 11-6 0 3 3 0 016 0z" stroke-linecap="round" stroke-linejoin="round"/></svg>
            </div>
            <div>
              <div class="contact-item-label">Office Address</div>
              <div class="contact-item-value">#505, 5th Floor, Urban Square Tower D<br/>Golf Course Extension Road, Sector 62<br/>Gurugram – 122101, Haryana, India</div>
            </div>
          </div>

          <div class="contact-item">
            <div class="contact-icon">
              <svg viewBox="0 0 24 24" fill="none" stroke-width="1.5"><path d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" stroke-linecap="round" stroke-linejoin="round"/></svg>
            </div>
            <div>
              <div class="contact-item-label">Email</div>
              <div class="contact-item-value">kingshukghosh@widestrategyadvisors.com<br/>paromitaghosh@widestrategyadvisors.com</div>
            </div>
          </div>

          <div class="contact-item">
            <div class="contact-icon">
              <svg viewBox="0 0 24 24" fill="none" stroke-width="1.5"><path d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" stroke-linecap="round" stroke-linejoin="round"/></svg>
            </div>
            <div>
              <div class="contact-item-label">General Enquiries</div>
              <div class="contact-item-value">info@widestrategyadvisors.com</div>
            </div>
          </div>

          <div class="contact-item">
            <div class="contact-icon">
              <svg viewBox="0 0 24 24" fill="none" stroke-width="1.5"><circle cx="12" cy="12" r="10" stroke-linecap="round" stroke-linejoin="round"/><path d="M12 8v4l3 3" stroke-linecap="round" stroke-linejoin="round"/></svg>
            </div>
            <div>
              <div class="contact-item-label">Office Hours</div>
              <div class="contact-item-value">Monday – Friday: 9:00 AM – 7:00 PM IST<br/>Saturday: 10:00 AM – 2:00 PM (by appointment)</div>
            </div>
          </div>

          <div class="map-placeholder">
            <div class="map-placeholder-inner">
              <svg width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="rgba(250,249,246,0.3)" stroke-width="1" style="margin:0 auto 10px;display:block;"><path d="M17.657 16.657L13.414 20.9a2 2 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"/><path d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"/></svg>
              Urban Square Tower D, Sector 62, Gurugram
            </div>
          </div>
        </div>

        <div class="fade-up">
          <span class="eyebrow">Send an Enquiry</span>
          <div class="gold-rule"></div>
          <h3 style="color:var(--dark-navy); margin-bottom:32px;">Book a Consultation</h3>
          <form class="contact-form" onsubmit="handleFormSubmit(event)">
            <div class="form-row">
              <div class="form-group">
                <label class="form-label">First Name</label>
                <input type="text" class="form-input" placeholder="Rajiv" required />
              </div>
              <div class="form-group">
                <label class="form-label">Last Name</label>
                <input type="text" class="form-input" placeholder="Kapoor" required />
              </div>
            </div>
            <div class="form-row">
              <div class="form-group">
                <label class="form-label">Email Address</label>
                <input type="email" class="form-input" placeholder="rajiv@company.com" required />
              </div>
              <div class="form-group">
                <label class="form-label">Mobile Number</label>
                <input type="tel" class="form-input" placeholder="+91 98XXX XXXXX" />
              </div>
            </div>
            <div class="form-group">
              <label class="form-label">Company Name</label>
              <input type="text" class="form-input" placeholder="Your Company Pvt. Ltd." />
            </div>
            <div class="form-row">
              <div class="form-group">
                <label class="form-label">Annual Turnover</label>
                <select class="form-select form-input">
                  <option value="">Select Range</option>
                  <option>Below ₹25 Crore</option>
                  <option>₹25 – ₹100 Crore</option>
                  <option>₹100 – ₹500 Crore</option>
                  <option>Above ₹500 Crore</option>
                  <option>Startup (Pre-Revenue)</option>
                </select>
              </div>
              <div class="form-group">
                <label class="form-label">Service of Interest</label>
                <select class="form-select form-input">
                  <option value="">Select Service</option>
                  <option>Debt &amp; Structured Finance</option>
                  <option>Equity Fund Raising</option>
                  <option>Transaction Advisory (M&amp;A)</option>
                  <option>ESG &amp; Strategic Advisory</option>
                  <option>Wealth Management</option>
                  <option>Family Office Solutions</option>
                  <option>NRI &amp; Cross-Border Advisory</option>
                  <option>Not Sure – Explore Options</option>
                </select>
              </div>
            </div>
            <div class="form-group">
              <label class="form-label">Brief Description of Your Requirement</label>
              <textarea class="form-textarea" placeholder="Please describe your situation and what you are looking to achieve. All enquiries are treated with strict confidentiality."></textarea>
            </div>
            <button type="submit" class="form-submit">Submit Enquiry →</button>
          </form>
          <p style="font-size:12px; color:var(--text-muted); margin-top:16px;">All information shared is treated with absolute confidentiality. We will respond within one business day.</p>
        </div>
      </div>
    </div>
  </section>
</div>

<!-- ══════════════════════════════════════════════
     FOOTER
══════════════════════════════════════════════ -->
<footer>
  <div class="footer-inner">
    <div class="footer-top">
      <div>
        <div class="footer-brand-name">WideStrategy Advisors LLP</div>
        <div class="footer-brand-tag">Where Capital Meets Strategy</div>
        <p class="footer-desc">A boutique strategic and financial advisory firm headquartered in Gurugram, India, serving ambitious enterprises across the capital spectrum.</p>
      </div>
      <div class="footer-col">
        <div class="footer-col-title">Services</div>
        <ul>
          <li><a href="#" onclick="showPage('services'); return false;">Debt &amp; Structured Finance</a></li>
          <li><a href="#" onclick="showPage('services'); return false;">Equity &amp; Fund Raising</a></li>
          <li><a href="#" onclick="showPage('services'); return false;">Transaction Advisory</a></li>
          <li><a href="#" onclick="showPage('services'); return false;">ESG Advisory</a></li>
          <li><a href="#" onclick="showPage('services'); return false;">Wealth Management</a></li>
          <li><a href="#" onclick="showPage('services'); return false;">Family Office</a></li>
        </ul>
      </div>
      <div class="footer-col">
        <div class="footer-col-title">Company</div>
        <ul>
          <li><a href="#" onclick="showPage('about'); return false;">About Us</a></li>
          <li><a href="#" onclick="showPage('about'); return false;">Leadership Team</a></li>
          <li><a href="#" onclick="showPage('industries'); return false;">Industries</a></li>
          <li><a href="#" onclick="showPage('insights'); return false;">Insights</a></li>
          <li><a href="#" onclick="showPage('contact'); return false;">Contact</a></li>
        </ul>
      </div>
      <div class="footer-col">
        <div class="footer-col-title">Contact</div>
        <ul>
          <li><a href="mailto:kingshukghosh@widestrategyadvisors.com">kingshukghosh@widestrategyadvisors.com</a></li>
          <li><a href="mailto:info@widestrategyadvisors.com">info@widestrategyadvisors.com</a></li>
          <li><a href="#">Gurugram, Haryana – 122101</a></li>
          <li><a href="#" onclick="showPage('contact'); return false;">Book a Consultation</a></li>
        </ul>
      </div>
    </div>
    <div class="footer-bottom">
      <span class="footer-copy">© 2025 WideStrategy Advisors LLP. All rights reserved. SEBI Reg. No. INM000XXXXXX.</span>
      <div class="footer-legal">
        <a href="#">Privacy Policy</a>
        <a href="#">Disclaimer</a>
        <a href="#">SEBI Disclosure</a>
      </div>
    </div>
  </div>
</footer>

<!-- ══════════════════════════════════════════════
     TOAST
══════════════════════════════════════════════ -->
<div id="toast" style="
  position:fixed; bottom:32px; right:32px; z-index:9999;
  background:var(--navy); color:var(--off-white);
  padding:16px 24px; border-radius:3px;
  border-left:3px solid var(--gold);
  font-size:14px; box-shadow:var(--shadow-lg);
  transform:translateY(80px); opacity:0;
  transition:all 0.35s ease;
  max-width:320px; line-height:1.5;
">✓ &nbsp;Thank you. We will be in touch within one business day.</div>

<script>
  // ── PAGE ROUTING ────────────────────────────────────────────────
  function showPage(id) {
    document.querySelectorAll('.page-section').forEach(el => el.classList.remove('active'));
    document.getElementById('page-' + id).classList.add('active');
    window.scrollTo({ top: 0, behavior: 'smooth' });
    observeFadeUps();
  }

  // ── NAVBAR SCROLL ───────────────────────────────────────────────
  window.addEventListener('scroll', () => {
    document.getElementById('navbar').classList.toggle('scrolled', window.scrollY > 40);
  });
  document.getElementById('navbar').classList.add('scrolled');

  // ── MOBILE MENU ─────────────────────────────────────────────────
  function toggleMenu() {
    document.getElementById('mobile-menu').classList.toggle('open');
  }

  // ── FADE-UP ANIMATIONS ──────────────────────────────────────────
  function observeFadeUps() {
    const io = new IntersectionObserver((entries) => {
      entries.forEach((e, i) => {
        if (e.isIntersecting) {
          setTimeout(() => e.target.classList.add('visible'), i * 80);
          io.unobserve(e.target);
        }
      });
    }, { threshold: 0.08 });
    document.querySelectorAll('.page-section.active .fade-up:not(.visible)').forEach(el => io.observe(el));
  }
  observeFadeUps();

  // ── FORM SUBMIT ─────────────────────────────────────────────────
  function handleFormSubmit(e) {
    e.preventDefault();
    const toast = document.getElementById('toast');
    toast.style.transform = 'translateY(0)';
    toast.style.opacity = '1';
    setTimeout(() => {
      toast.style.transform = 'translateY(80px)';
      toast.style.opacity = '0';
    }, 4500);
    e.target.reset();
  }
</script>
</body>
</html>
