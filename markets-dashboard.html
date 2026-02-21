<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MarketPulse — Dashboard Financiero</title>
<link href="https://fonts.googleapis.com/css2?family=Space+Mono:ital,wght@0,400;0,700;1,400&family=Bebas+Neue&family=DM+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">
<style>
  :root {
    --bg: #050810;
    --bg2: #0a0e1a;
    --bg3: #0f1525;
    --border: rgba(255,255,255,0.07);
    --accent: #00ff88;
    --accent2: #0088ff;
    --accent3: #ff4466;
    --accent4: #ffaa00;
    --text: #e8edf5;
    --text2: #7a8499;
    --text3: #4a5166;
    --green: #00e676;
    --red: #ff3d57;
    --gold: #ffd700;
    --card: rgba(255,255,255,0.03);
    --card-hover: rgba(255,255,255,0.06);
    --glow: 0 0 30px rgba(0,255,136,0.15);
    --glow2: 0 0 30px rgba(0,136,255,0.15);
  }

  * { margin: 0; padding: 0; box-sizing: border-box; }

  body {
    font-family: 'DM Sans', sans-serif;
    background: var(--bg);
    color: var(--text);
    min-height: 100vh;
    overflow-x: hidden;
  }

  /* Animated background */
  body::before {
    content: '';
    position: fixed;
    top: 0; left: 0; right: 0; bottom: 0;
    background: 
      radial-gradient(ellipse 80% 50% at 20% 10%, rgba(0,255,136,0.04) 0%, transparent 60%),
      radial-gradient(ellipse 60% 40% at 80% 80%, rgba(0,136,255,0.05) 0%, transparent 60%),
      radial-gradient(ellipse 40% 30% at 60% 20%, rgba(255,68,102,0.03) 0%, transparent 50%);
    pointer-events: none;
    z-index: 0;
  }

  /* Grid scanlines */
  body::after {
    content: '';
    position: fixed;
    top: 0; left: 0; right: 0; bottom: 0;
    background-image: linear-gradient(rgba(255,255,255,0.01) 1px, transparent 1px);
    background-size: 100% 40px;
    pointer-events: none;
    z-index: 0;
  }

  /* HEADER */
  header {
    position: sticky;
    top: 0;
    z-index: 100;
    background: rgba(5,8,16,0.95);
    backdrop-filter: blur(20px);
    border-bottom: 1px solid var(--border);
    padding: 0 24px;
    height: 60px;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .logo {
    font-family: 'Bebas Neue', cursive;
    font-size: 28px;
    letter-spacing: 3px;
    background: linear-gradient(135deg, var(--accent), var(--accent2));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }

  .logo span {
    color: var(--text2);
    font-size: 11px;
    letter-spacing: 2px;
    font-family: 'Space Mono', monospace;
    display: block;
    -webkit-text-fill-color: var(--text2);
    line-height: 1;
  }

  .header-right {
    display: flex;
    align-items: center;
    gap: 16px;
  }

  .live-badge {
    display: flex;
    align-items: center;
    gap: 6px;
    background: rgba(0,230,118,0.1);
    border: 1px solid rgba(0,230,118,0.3);
    border-radius: 20px;
    padding: 4px 12px;
    font-size: 11px;
    font-family: 'Space Mono', monospace;
    color: var(--green);
    letter-spacing: 1px;
  }

  .live-dot {
    width: 6px; height: 6px;
    border-radius: 50%;
    background: var(--green);
    animation: pulse 1.5s ease-in-out infinite;
  }

  @keyframes pulse {
    0%, 100% { opacity: 1; transform: scale(1); }
    50% { opacity: 0.5; transform: scale(0.8); }
  }

  #clock {
    font-family: 'Space Mono', monospace;
    font-size: 12px;
    color: var(--text2);
    letter-spacing: 1px;
  }

  /* TICKER */
  .ticker-wrap {
    background: var(--bg2);
    border-bottom: 1px solid var(--border);
    overflow: hidden;
    height: 36px;
    display: flex;
    align-items: center;
    position: relative;
    z-index: 1;
  }

  .ticker-label {
    background: var(--accent);
    color: #000;
    font-family: 'Space Mono', monospace;
    font-size: 10px;
    font-weight: 700;
    letter-spacing: 2px;
    padding: 0 14px;
    height: 100%;
    display: flex;
    align-items: center;
    flex-shrink: 0;
    z-index: 2;
  }

  .ticker-track {
    display: flex;
    animation: scroll 40s linear infinite;
    white-space: nowrap;
  }

  @keyframes scroll {
    0% { transform: translateX(0); }
    100% { transform: translateX(-50%); }
  }

  .ticker-item {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    padding: 0 24px;
    font-family: 'Space Mono', monospace;
    font-size: 11px;
    border-right: 1px solid var(--border);
  }

  .ticker-item .sym { color: var(--text2); }
  .ticker-item .price { color: var(--text); }
  .ticker-item .chg.up { color: var(--green); }
  .ticker-item .chg.down { color: var(--red); }

  /* NAV */
  nav {
    position: relative;
    z-index: 1;
    background: var(--bg2);
    border-bottom: 1px solid var(--border);
    padding: 0 24px;
    display: flex;
    gap: 4px;
    overflow-x: auto;
    scrollbar-width: none;
  }

  nav::-webkit-scrollbar { display: none; }

  .nav-btn {
    background: none;
    border: none;
    color: var(--text2);
    font-family: 'DM Sans', sans-serif;
    font-size: 13px;
    font-weight: 500;
    padding: 14px 18px;
    cursor: pointer;
    white-space: nowrap;
    border-bottom: 2px solid transparent;
    transition: all 0.2s;
    letter-spacing: 0.5px;
  }

  .nav-btn:hover { color: var(--text); }
  .nav-btn.active { color: var(--accent); border-bottom-color: var(--accent); }

  /* MAIN */
  main {
    position: relative;
    z-index: 1;
    padding: 24px;
    max-width: 1600px;
    margin: 0 auto;
  }

  /* SECTION */
  .section { display: none; }
  .section.active { display: block; }

  /* GRID LAYOUTS */
  .grid-4 {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 16px;
    margin-bottom: 24px;
  }

  .grid-3 {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 16px;
    margin-bottom: 24px;
  }

  .grid-2 {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 16px;
    margin-bottom: 24px;
  }

  .grid-2-1 {
    display: grid;
    grid-template-columns: 2fr 1fr;
    gap: 16px;
    margin-bottom: 24px;
  }

  /* CARDS */
  .card {
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 20px;
    transition: all 0.3s;
    position: relative;
    overflow: hidden;
  }

  .card::before {
    content: '';
    position: absolute;
    top: 0; left: 0; right: 0;
    height: 1px;
    background: linear-gradient(90deg, transparent, rgba(255,255,255,0.1), transparent);
  }

  .card:hover {
    background: var(--card-hover);
    border-color: rgba(255,255,255,0.12);
    transform: translateY(-2px);
  }

  .card-label {
    font-size: 11px;
    letter-spacing: 2px;
    color: var(--text3);
    font-family: 'Space Mono', monospace;
    text-transform: uppercase;
    margin-bottom: 10px;
  }

  .card-value {
    font-family: 'Bebas Neue', cursive;
    font-size: 36px;
    letter-spacing: 1px;
    line-height: 1;
    margin-bottom: 6px;
  }

  .card-sub {
    font-size: 12px;
    color: var(--text2);
  }

  .badge {
    display: inline-flex;
    align-items: center;
    gap: 4px;
    padding: 3px 10px;
    border-radius: 20px;
    font-size: 12px;
    font-family: 'Space Mono', monospace;
    font-weight: 700;
  }

  .badge.up { background: rgba(0,230,118,0.12); color: var(--green); border: 1px solid rgba(0,230,118,0.2); }
  .badge.down { background: rgba(255,61,87,0.12); color: var(--red); border: 1px solid rgba(255,61,87,0.2); }
  .badge.neutral { background: rgba(255,170,0,0.12); color: var(--accent4); border: 1px solid rgba(255,170,0,0.2); }

  /* SECTION HEADER */
  .section-header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 20px;
  }

  .section-title {
    font-family: 'Bebas Neue', cursive;
    font-size: 24px;
    letter-spacing: 2px;
    color: var(--text);
  }

  .section-title span {
    color: var(--accent);
  }

  /* TABLE */
  .data-table {
    width: 100%;
    border-collapse: collapse;
    font-size: 13px;
  }

  .data-table th {
    text-align: left;
    padding: 10px 14px;
    font-family: 'Space Mono', monospace;
    font-size: 10px;
    letter-spacing: 1.5px;
    color: var(--text3);
    border-bottom: 1px solid var(--border);
    text-transform: uppercase;
  }

  .data-table td {
    padding: 12px 14px;
    border-bottom: 1px solid rgba(255,255,255,0.03);
    vertical-align: middle;
  }

  .data-table tr:hover td {
    background: rgba(255,255,255,0.02);
  }

  .asset-name {
    display: flex;
    align-items: center;
    gap: 10px;
  }

  .asset-icon {
    width: 32px;
    height: 32px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 14px;
    flex-shrink: 0;
  }

  .asset-sym {
    font-weight: 600;
    font-size: 14px;
    color: var(--text);
  }

  .asset-full {
    font-size: 11px;
    color: var(--text2);
  }

  .up { color: var(--green); }
  .down { color: var(--red); }
  .neutral { color: var(--accent4); }

  /* MINI CHART */
  .mini-chart {
    display: flex;
    align-items: flex-end;
    gap: 2px;
    height: 32px;
    width: 80px;
  }

  .mini-bar {
    flex: 1;
    border-radius: 2px 2px 0 0;
    transition: height 0.3s;
  }

  /* PROGRESS BAR */
  .progress-wrap {
    background: rgba(255,255,255,0.06);
    border-radius: 4px;
    height: 6px;
    overflow: hidden;
    margin-top: 8px;
  }

  .progress-fill {
    height: 100%;
    border-radius: 4px;
    transition: width 1s ease;
  }

  /* GAUGE */
  .gauge-wrap {
    text-align: center;
    padding: 20px;
  }

  .gauge-svg { width: 180px; height: 100px; }

  .gauge-value {
    font-family: 'Bebas Neue', cursive;
    font-size: 48px;
    letter-spacing: 2px;
  }

  .gauge-label {
    font-size: 13px;
    color: var(--text2);
    margin-top: 4px;
  }

  /* NEWS */
  .news-item {
    padding: 16px 0;
    border-bottom: 1px solid var(--border);
    cursor: pointer;
    transition: all 0.2s;
  }

  .news-item:last-child { border-bottom: none; }
  .news-item:hover { padding-left: 8px; }

  .news-meta {
    display: flex;
    align-items: center;
    gap: 10px;
    margin-bottom: 6px;
  }

  .news-source {
    font-family: 'Space Mono', monospace;
    font-size: 10px;
    letter-spacing: 1px;
    color: var(--accent);
    text-transform: uppercase;
  }

  .news-time {
    font-size: 11px;
    color: var(--text3);
  }

  .news-title {
    font-size: 14px;
    font-weight: 500;
    color: var(--text);
    line-height: 1.4;
    margin-bottom: 4px;
  }

  .news-tags {
    display: flex;
    gap: 6px;
    flex-wrap: wrap;
  }

  .news-tag {
    background: rgba(255,255,255,0.05);
    border: 1px solid var(--border);
    border-radius: 4px;
    padding: 2px 8px;
    font-size: 10px;
    color: var(--text2);
  }

  /* ANALYSIS CARD */
  .analysis-card {
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 24px;
    margin-bottom: 16px;
  }

  .signal-row {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 10px 0;
    border-bottom: 1px solid rgba(255,255,255,0.04);
  }

  .signal-row:last-child { border-bottom: none; }

  .signal-name {
    font-size: 13px;
    color: var(--text2);
  }

  .signal-val {
    font-family: 'Space Mono', monospace;
    font-size: 12px;
    font-weight: 700;
  }

  /* ALERT */
  .alert {
    display: flex;
    align-items: center;
    gap: 12px;
    background: rgba(255,170,0,0.08);
    border: 1px solid rgba(255,170,0,0.2);
    border-radius: 8px;
    padding: 12px 16px;
    margin-bottom: 12px;
    font-size: 13px;
    color: var(--text);
  }

  .alert-icon { font-size: 18px; }
  .alert-time { font-size: 11px; color: var(--text2); margin-left: auto; }

  /* ASSET HEADER in detail */
  .asset-header {
    display: flex;
    align-items: flex-start;
    gap: 20px;
    margin-bottom: 24px;
    flex-wrap: wrap;
  }

  .asset-big-icon {
    width: 60px; height: 60px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 28px;
    border: 2px solid var(--border);
  }

  .asset-big-price {
    font-family: 'Bebas Neue', cursive;
    font-size: 52px;
    letter-spacing: 2px;
    line-height: 1;
  }

  /* CHART placeholder */
  .chart-container {
    width: 100%;
    height: 280px;
    background: var(--bg3);
    border: 1px solid var(--border);
    border-radius: 12px;
    overflow: hidden;
    position: relative;
  }

  .chart-container canvas {
    width: 100% !important;
    height: 100% !important;
  }

  /* FEAR GREED */
  .fg-meter {
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  /* REFRESH BTN */
  .refresh-btn {
    background: rgba(0,255,136,0.1);
    border: 1px solid rgba(0,255,136,0.3);
    color: var(--accent);
    border-radius: 8px;
    padding: 8px 16px;
    font-family: 'Space Mono', monospace;
    font-size: 11px;
    cursor: pointer;
    letter-spacing: 1px;
    transition: all 0.2s;
    display: flex;
    align-items: center;
    gap: 6px;
  }

  .refresh-btn:hover {
    background: rgba(0,255,136,0.2);
    transform: scale(1.02);
  }

  .spin { animation: spin 1s linear infinite; }
  @keyframes spin { to { transform: rotate(360deg); } }

  /* RESUMEN AI */
  .ai-summary {
    background: linear-gradient(135deg, rgba(0,136,255,0.05), rgba(0,255,136,0.05));
    border: 1px solid rgba(0,255,136,0.15);
    border-radius: 12px;
    padding: 24px;
    margin-bottom: 24px;
    position: relative;
    overflow: hidden;
  }

  .ai-summary::before {
    content: 'AI';
    position: absolute;
    top: -10px; right: -10px;
    font-family: 'Bebas Neue', cursive;
    font-size: 80px;
    color: rgba(0,255,136,0.04);
    letter-spacing: 5px;
  }

  .ai-summary-title {
    font-family: 'Bebas Neue', cursive;
    font-size: 20px;
    letter-spacing: 2px;
    color: var(--accent);
    margin-bottom: 12px;
    display: flex;
    align-items: center;
    gap: 8px;
  }

  .ai-summary-text {
    font-size: 14px;
    line-height: 1.7;
    color: var(--text2);
  }

  .ai-summary-text strong { color: var(--text); }

  /* RESPONSIVE */
  @media (max-width: 1024px) {
    .grid-4 { grid-template-columns: repeat(2, 1fr); }
    .grid-3 { grid-template-columns: repeat(2, 1fr); }
    .grid-2-1 { grid-template-columns: 1fr; }
  }

  @media (max-width: 640px) {
    main { padding: 16px; }
    header { padding: 0 16px; }
    nav { padding: 0 12px; }
    .grid-4, .grid-3, .grid-2 { grid-template-columns: 1fr; }
    .card-value { font-size: 28px; }
    .asset-big-price { font-size: 36px; }
    .logo { font-size: 22px; }
    #clock { display: none; }
  }

  /* LOADING */
  .loading {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 200px;
    flex-direction: column;
    gap: 16px;
  }

  .loading-ring {
    width: 40px; height: 40px;
    border: 3px solid var(--border);
    border-top-color: var(--accent);
    border-radius: 50%;
    animation: spin 0.8s linear infinite;
  }

  .loading-text {
    font-family: 'Space Mono', monospace;
    font-size: 11px;
    color: var(--text3);
    letter-spacing: 2px;
  }

  /* SPARKLINE */
  .sparkline { width: 90px; height: 36px; }

  /* TAG */
  .tag {
    display: inline-block;
    padding: 2px 10px;
    border-radius: 4px;
    font-size: 11px;
    font-family: 'Space Mono', monospace;
    letter-spacing: 0.5px;
    background: rgba(255,255,255,0.05);
    border: 1px solid var(--border);
    color: var(--text2);
  }

  /* FULL WIDTH */
  .full { grid-column: 1/-1; }

  /* SCROLL BAR */
  ::-webkit-scrollbar { width: 6px; height: 6px; }
  ::-webkit-scrollbar-track { background: var(--bg2); }
  ::-webkit-scrollbar-thumb { background: var(--border); border-radius: 3px; }
  ::-webkit-scrollbar-thumb:hover { background: rgba(255,255,255,0.2); }

  /* ANIMATED NUMBER */
  .animated-num { transition: all 0.5s; }

  /* DOMINANCE BAR */
  .dom-bar { height: 8px; border-radius: 4px; background: rgba(255,255,255,0.08); overflow: hidden; }
  .dom-fill { height: 100%; border-radius: 4px; }

  /* SEPARATOR */
  .sep {
    height: 1px;
    background: var(--border);
    margin: 24px 0;
  }

</style>
</head>
<body>

<!-- HEADER -->
<header>
  <div>
    <div class="logo">MarketPulse</div>
    <span style="font-family:'Space Mono',monospace;font-size:10px;color:var(--text3);letter-spacing:2px;">FINANCIAL INTELLIGENCE</span>
  </div>
  <div class="header-right">
    <div class="live-badge"><div class="live-dot"></div>EN VIVO</div>
    <div id="clock"></div>
  </div>
</header>

<!-- TICKER -->
<div class="ticker-wrap">
  <div class="ticker-label">LIVE</div>
  <div style="overflow:hidden;flex:1">
    <div class="ticker-track" id="ticker"></div>
  </div>
</div>

<!-- NAV -->
<nav>
  <button class="nav-btn active" onclick="showSection('overview')">📊 Resumen</button>
  <button class="nav-btn" onclick="showSection('crypto')">₿ Crypto</button>
  <button class="nav-btn" onclick="showSection('indices')">📈 Índices</button>
  <button class="nav-btn" onclick="showSection('forex')">💱 Forex</button>
  <button class="nav-btn" onclick="showSection('commodities')">🥇 Commodities</button>
  <button class="nav-btn" onclick="showSection('analysis')">🔬 Análisis</button>
  <button class="nav-btn" onclick="showSection('news')">📰 Noticias</button>
</nav>

<!-- MAIN -->
<main>

  <!-- ===== OVERVIEW ===== -->
  <div id="overview" class="section active">
    
    <div class="ai-summary">
      <div class="ai-summary-title">🤖 RESUMEN DE MERCADOS — <span id="today-date"></span></div>
      <div class="ai-summary-text" id="ai-text">
        <strong>Sesión destacada:</strong> Los mercados globales operan con tono mixto. 
        <strong>S&P 500</strong> cotiza al alza impulsado por datos de empleo sólidos. 
        <strong>Bitcoin</strong> consolida sobre $67K con volumen moderado. 
        El <strong>oro</strong> mantiene zona de máximos históricos cerca de $5.100/oz ante tensiones geopolíticas. 
        La <strong>Fed</strong> sin señales de recorte inminente. El <strong>DXY</strong> cede terreno tras fallo arancelario. 
        Sentimiento general: <strong style="color:var(--accent4)">NEUTRAL — cautela con sesgo alcista.</strong>
      </div>
    </div>

    <!-- KPI Cards -->
    <div class="grid-4" id="kpi-cards"></div>

    <!-- Charts Row -->
    <div class="grid-2">
      <div class="card">
        <div class="section-header" style="margin-bottom:12px">
          <div class="card-label">MERCADOS GLOBALES — 7D</div>
          <span id="last-update" style="font-size:11px;color:var(--text3);font-family:'Space Mono',monospace"></span>
        </div>
        <div class="chart-container" style="height:220px">
          <canvas id="overviewChart"></canvas>
        </div>
      </div>
      <div class="card">
        <div class="card-label" style="margin-bottom:16px">FEAR & GREED — CRYPTO</div>
        <div class="gauge-wrap">
          <canvas id="fgGauge" width="220" height="130"></canvas>
          <div class="gauge-value" id="fg-value" style="color:var(--accent4)">52</div>
          <div class="gauge-label" id="fg-label">NEUTRAL</div>
          <div style="margin-top:16px;font-size:12px;color:var(--text3)">
            Ayer: <span style="color:var(--text2)">49</span> &nbsp; Semana pasada: <span style="color:var(--text2)">61</span>
          </div>
        </div>
      </div>
    </div>

    <!-- Top Movers -->
    <div class="section-header">
      <div class="section-title">TOP <span>MOVERS</span> HOY</div>
      <button class="refresh-btn" onclick="refreshData()"><span id="refresh-icon">↻</span> ACTUALIZAR</button>
    </div>
    <div class="card" style="margin-bottom:24px">
      <table class="data-table" id="movers-table"></table>
    </div>

    <!-- Alerts -->
    <div class="section-header">
      <div class="section-title">⚡ <span>ALERTAS</span> ACTIVAS</div>
    </div>
    <div id="alerts-container"></div>

  </div>

  <!-- ===== CRYPTO ===== -->
  <div id="crypto" class="section">
    <div class="section-header">
      <div class="section-title">₿ MERCADO <span>CRYPTO</span></div>
      <button class="refresh-btn" onclick="refreshData()">↻ ACTUALIZAR</button>
    </div>

    <div class="grid-4" id="crypto-kpi"></div>

    <div class="card" style="margin-bottom:24px">
      <div class="card-label" style="margin-bottom:16px">DOMINANCIA DE MERCADO</div>
      <div style="display:flex;gap:20px;flex-wrap:wrap" id="dominance-bars"></div>
    </div>

    <div class="card" style="margin-bottom:24px">
      <div class="card-label" style="margin-bottom:16px">BITCOIN — GRÁFICO 7D</div>
      <div class="chart-container" style="height:240px">
        <canvas id="btcChart"></canvas>
      </div>
    </div>

    <div class="section-header">
      <div class="section-title">TODAS LAS <span>MONEDAS</span></div>
    </div>
    <div class="card">
      <table class="data-table" id="crypto-table"></table>
    </div>
  </div>

  <!-- ===== ÍNDICES ===== -->
  <div id="indices" class="section">
    <div class="section-header">
      <div class="section-title">📈 ÍNDICES <span>GLOBALES</span></div>
      <button class="refresh-btn" onclick="refreshData()">↻ ACTUALIZAR</button>
    </div>
    <div class="grid-4" id="indices-kpi"></div>
    <div class="card" style="margin-bottom:24px">
      <div class="card-label" style="margin-bottom:16px">COMPARATIVA ÍNDICES — 30D</div>
      <div class="chart-container" style="height:280px">
        <canvas id="indicesChart"></canvas>
      </div>
    </div>
    <div class="card">
      <table class="data-table" id="indices-table"></table>
    </div>
  </div>

  <!-- ===== FOREX ===== -->
  <div id="forex" class="section">
    <div class="section-header">
      <div class="section-title">💱 MERCADO <span>FOREX</span></div>
      <button class="refresh-btn" onclick="refreshData()">↻ ACTUALIZAR</button>
    </div>
    <div class="grid-4" id="forex-kpi"></div>
    <div class="card" style="margin-bottom:24px">
      <div class="card-label" style="margin-bottom:16px">DXY — ÍNDICE DÓLAR</div>
      <div class="chart-container" style="height:240px">
        <canvas id="forexChart"></canvas>
      </div>
    </div>
    <div class="card">
      <table class="data-table" id="forex-table"></table>
    </div>
  </div>

  <!-- ===== COMMODITIES ===== -->
  <div id="commodities" class="section">
    <div class="section-header">
      <div class="section-title">🥇 <span>COMMODITIES</span></div>
      <button class="refresh-btn" onclick="refreshData()">↻ ACTUALIZAR</button>
    </div>
    <div class="grid-4" id="comm-kpi"></div>
    <div class="card" style="margin-bottom:24px">
      <div class="card-label" style="margin-bottom:16px">ORO vs PETRÓLEO — 30D</div>
      <div class="chart-container" style="height:240px">
        <canvas id="commChart"></canvas>
      </div>
    </div>
    <div class="card">
      <table class="data-table" id="comm-table"></table>
    </div>
  </div>

  <!-- ===== ANALYSIS ===== -->
  <div id="analysis" class="section">
    <div class="section-header">
      <div class="section-title">🔬 ANÁLISIS <span>TÉCNICO</span></div>
    </div>

    <div class="grid-2">
      <!-- BTC Analysis -->
      <div class="analysis-card">
        <div style="display:flex;align-items:center;gap:12px;margin-bottom:20px">
          <div class="asset-icon" style="background:rgba(247,147,26,0.15);border:1px solid rgba(247,147,26,0.3)">₿</div>
          <div>
            <div style="font-weight:600;font-size:16px">Bitcoin / USD</div>
            <div style="font-size:12px;color:var(--text2)">BTC — Análisis 4H + 1D</div>
          </div>
          <div class="badge up" style="margin-left:auto">COMPRA</div>
        </div>
        <div id="btc-signals"></div>
        <div class="sep"></div>
        <div style="font-size:13px;color:var(--text2);line-height:1.7">
          <strong style="color:var(--text)">Conclusión:</strong> BTC consolida sobre soporte $64K. RSI neutro. 
          Resistencia crítica en $68K — ruptura confirmaría impulso hacia $72K. 
          Soporte clave: <strong style="color:var(--green)">$64.200</strong>. 
          Stop loss sugerido: <strong style="color:var(--red)">$61.800</strong>.
        </div>
      </div>

      <!-- S&P Analysis -->
      <div class="analysis-card">
        <div style="display:flex;align-items:center;gap:12px;margin-bottom:20px">
          <div class="asset-icon" style="background:rgba(0,136,255,0.15);border:1px solid rgba(0,136,255,0.3)">📈</div>
          <div>
            <div style="font-weight:600;font-size:16px">S&P 500</div>
            <div style="font-size:12px;color:var(--text2)">SPX — Análisis Diario</div>
          </div>
          <div class="badge neutral" style="margin-left:auto">NEUTRAL</div>
        </div>
        <div id="spx-signals"></div>
        <div class="sep"></div>
        <div style="font-size:13px;color:var(--text2);line-height:1.7">
          <strong style="color:var(--text)">Conclusión:</strong> SPX en zona de resistencia histórica 6.900. 
          Momento comprador se desacelera. RSI sobrecomprado en 1D. 
          Soporte: <strong style="color:var(--green)">6.720</strong>. 
          Escenario bajista si rompe: <strong style="color:var(--red)">6.500</strong>.
        </div>
      </div>
    </div>

    <!-- ORO Analysis -->
    <div class="analysis-card">
      <div style="display:flex;align-items:center;gap:12px;margin-bottom:20px">
        <div class="asset-icon" style="background:rgba(255,215,0,0.15);border:1px solid rgba(255,215,0,0.3)">🥇</div>
        <div>
          <div style="font-weight:600;font-size:16px">Oro / USD</div>
          <div style="font-size:12px;color:var(--text2)">XAU/USD — Tendencia Principal</div>
        </div>
        <div class="badge up" style="margin-left:auto">FUERTE COMPRA</div>
      </div>
      <div class="grid-3" id="gold-signals" style="margin-bottom:16px"></div>
      <div style="font-size:13px;color:var(--text2);line-height:1.7">
        <strong style="color:var(--text)">Conclusión:</strong> El oro se encuentra en una tendencia alcista estructural. 
        Supera máximos históricos consecutivos. Refugio seguro ante incertidumbre geopolítica, 
        compras de bancos centrales y expectativas de recorte Fed. 
        Target: <strong style="color:var(--green)">$5.300</strong>. Soporte: <strong style="color:var(--green)">$5.000</strong>.
      </div>
    </div>

    <!-- Macro Calendar -->
    <div class="section-header">
      <div class="section-title">📅 CALENDARIO <span>MACRO</span></div>
    </div>
    <div class="card" id="macro-calendar"></div>

  </div>

  <!-- ===== NEWS ===== -->
  <div id="news" class="section">
    <div class="section-header">
      <div class="section-title">📰 <span>NOTICIAS</span> RELEVANTES</div>
      <button class="refresh-btn" onclick="refreshData()">↻ ACTUALIZAR</button>
    </div>
    <div class="grid-2-1">
      <div class="card" id="news-main"></div>
      <div>
        <div class="card" id="news-sidebar"></div>
      </div>
    </div>
  </div>

</main>

<script>
// ============================================================
// DATA
// ============================================================
const MARKET_DATA = {
  crypto: [
    { sym: 'BTC', name: 'Bitcoin', icon: '₿', color: '#F7931A', price: 67655, change: 2.07, vol: '48.2B', cap: '1.35T', high: 68900, low: 64100 },
    { sym: 'ETH', name: 'Ethereum', icon: 'Ξ', color: '#627EEA', price: 2412, change: 1.45, vol: '18.7B', cap: '290B', high: 2500, low: 2280 },
    { sym: 'BNB', name: 'BNB', icon: '◆', color: '#F3BA2F', price: 624, change: -0.82, vol: '2.1B', cap: '93B', high: 640, low: 610 },
    { sym: 'SOL', name: 'Solana', icon: '◎', color: '#9945FF', price: 198, change: 3.21, vol: '5.8B', cap: '94B', high: 205, low: 188 },
    { sym: 'XRP', name: 'XRP', icon: '✕', color: '#00B4D8', price: 2.84, change: -1.12, vol: '6.4B', cap: '163B', high: 2.95, low: 2.74 },
    { sym: 'ADA', name: 'Cardano', icon: '₳', color: '#0033AD', price: 0.82, change: 0.94, vol: '0.8B', cap: '29B', high: 0.85, low: 0.79 },
    { sym: 'AVAX', name: 'Avalanche', icon: '▲', color: '#E84142', price: 34.5, change: 4.21, vol: '1.2B', cap: '14B', high: 36, low: 32 },
    { sym: 'DOGE', name: 'Dogecoin', icon: 'Ð', color: '#CBA135', price: 0.218, change: -2.34, vol: '2.9B', cap: '32B', high: 0.23, low: 0.21 },
  ],
  indices: [
    { sym: 'SPX', name: 'S&P 500', icon: '🇺🇸', price: 6881, change: 0.56, vol: 'Alto', country: 'EE.UU.' },
    { sym: 'NDX', name: 'Nasdaq 100', icon: '🇺🇸', price: 22753, change: 0.78, vol: 'Alto', country: 'EE.UU.' },
    { sym: 'DJI', name: 'Dow Jones', icon: '🇺🇸', price: 49662, change: 0.26, vol: 'Medio', country: 'EE.UU.' },
    { sym: 'DAX', name: 'DAX 40', icon: '🇩🇪', price: 22841, change: 1.12, vol: 'Alto', country: 'Alemania' },
    { sym: 'FTSE', name: 'FTSE 100', icon: '🇬🇧', price: 8742, change: 0.34, vol: 'Medio', country: 'Reino Unido' },
    { sym: 'N225', name: 'Nikkei 225', icon: '🇯🇵', price: 38640, change: -0.45, vol: 'Medio', country: 'Japón' },
    { sym: 'HSI', name: 'Hang Seng', icon: '🇭🇰', price: 23180, change: -1.23, vol: 'Medio', country: 'Hong Kong' },
    { sym: 'IBEX', name: 'IBEX 35', icon: '🇪🇸', price: 13240, change: 0.67, vol: 'Bajo', country: 'España' },
  ],
  forex: [
    { sym: 'EUR/USD', name: 'Euro / Dólar', icon: '€', price: 1.0842, change: 0.21, color: '#0088FF' },
    { sym: 'GBP/USD', name: 'Libra / Dólar', icon: '£', price: 1.2614, change: 0.14, color: '#FF4466' },
    { sym: 'USD/JPY', name: 'Dólar / Yen', icon: '¥', price: 149.82, change: -0.32, color: '#FFAA00' },
    { sym: 'USD/MXN', name: 'Dólar / Peso MX', icon: '$', price: 17.11, change: -0.80, color: '#00E676' },
    { sym: 'USD/CHF', name: 'Dólar / Franco', icon: '₣', price: 0.8923, change: -0.18, color: '#FF4466' },
    { sym: 'AUD/USD', name: 'Dólar AU / USD', icon: '$', price: 0.6324, change: 0.42, color: '#0088FF' },
    { sym: 'DXY', name: 'Índice Dólar', icon: '$', price: 103.42, change: -0.35, color: '#FFAA00' },
    { sym: 'USD/BRL', name: 'Dólar / Real BR', icon: 'R$', price: 5.82, change: -0.24, color: '#00E676' },
  ],
  commodities: [
    { sym: 'XAU', name: 'Oro', icon: '🥇', price: 5112, change: 0.82, unit: '$/oz', color: '#FFD700' },
    { sym: 'XAG', name: 'Plata', icon: '🥈', price: 32.4, change: 1.14, unit: '$/oz', color: '#C0C0C0' },
    { sym: 'WTI', name: 'Petróleo WTI', icon: '🛢️', price: 78.4, change: -0.64, unit: '$/bbl', color: '#FF6600' },
    { sym: 'BRENT', name: 'Brent', icon: '⛽', price: 82.1, change: -0.52, unit: '$/bbl', color: '#FF8844' },
    { sym: 'NG', name: 'Gas Natural', icon: '🔥', price: 3.84, change: 2.12, unit: '$/MMBtu', color: '#FF4488' },
    { sym: 'COPPER', name: 'Cobre', icon: '🔶', price: 4.58, change: 0.44, unit: '$/lb', color: '#CD7F32' },
    { sym: 'WHEAT', name: 'Trigo', icon: '🌾', price: 540, change: -1.2, unit: '¢/bu', color: '#DAA520' },
    { sym: 'CORN', name: 'Maíz', icon: '🌽', price: 480, change: -0.8, unit: '¢/bu', color: '#FFCC00' },
  ]
};

const NEWS_DATA = [
  { source: 'Reuters', time: 'Hace 12 min', title: 'Corte Suprema de EE.UU. anula aranceles globales de Trump en histórico fallo 6-3', tags: ['Macro', 'EE.UU.', 'Aranceles'], hot: true },
  { source: 'Bloomberg', time: 'Hace 28 min', title: 'Bitcoin supera resistencia de $67K con volumen creciente; traders apuntan a $70K', tags: ['BTC', 'Crypto'], hot: true },
  { source: 'FT', time: 'Hace 45 min', title: 'Oro alcanza nuevo máximo histórico por encima de $5.100/oz ante tensiones Irán-Israel', tags: ['Oro', 'Geopolítica'] },
  { source: 'WSJ', time: 'Hace 1h', title: 'Fed mantendría tasas sin cambios hasta junio; datos de empleo superan expectativas', tags: ['Fed', 'Tasas', 'Macro'] },
  { source: 'CNBC', time: 'Hace 1.5h', title: 'Ethereum registra entrada de $480M en ETFs spot; BlackRock lidera flujos institucionales', tags: ['ETH', 'ETF'] },
  { source: 'CoinDesk', time: 'Hace 2h', title: 'Solana supera los $200 impulsada por crecimiento de DeFi y nuevas integraciones DePIN', tags: ['SOL', 'DeFi'] },
  { source: 'MarketWatch', time: 'Hace 3h', title: 'Nasdaq 100 anota nuevo máximo anual; sector tech lidera con ganancias >2%', tags: ['Nasdaq', 'Tech'] },
  { source: 'CryptoSlate', time: 'Hace 4h', title: 'XRP bajo presión: SEC apela fallo; precio cede 1.1% en la sesión', tags: ['XRP', 'Regulación'] },
];

const MACRO_EVENTS = [
  { date: 'HOY', time: '15:30', event: 'IPC EE.UU. (MoM)', prev: '0.2%', est: '0.3%', impact: 'high' },
  { date: 'HOY', time: '17:00', event: 'Ventas minoristas EE.UU.', prev: '-0.4%', est: '0.1%', impact: 'medium' },
  { date: 'LUN', time: '10:00', event: 'PMI Manufacturero Eurozona', prev: '46.6', est: '47.1', impact: 'medium' },
  { date: 'LUN', time: '15:30', event: 'Solicitudes desempleo EE.UU.', prev: '219K', est: '215K', impact: 'medium' },
  { date: 'MIÉ', time: '15:30', event: 'PIB EE.UU. Q4 (Rev.)', prev: '2.3%', est: '3.1%', impact: 'high' },
  { date: 'JUE', time: '20:00', event: 'Actas FOMC', prev: '—', est: '—', impact: 'high' },
];

// ============================================================
// CLOCK
// ============================================================
function updateClock() {
  const now = new Date();
  document.getElementById('clock').textContent = now.toLocaleTimeString('es-MX', { hour: '2-digit', minute: '2-digit', second: '2-digit' });
  document.getElementById('last-update').textContent = 'Act: ' + now.toLocaleTimeString('es-MX', { hour: '2-digit', minute: '2-digit' });
}
setInterval(updateClock, 1000);
updateClock();

document.getElementById('today-date').textContent = new Date().toLocaleDateString('es-MX', { weekday: 'long', year: 'numeric', month: 'long', day: 'numeric' }).toUpperCase();

// ============================================================
// TICKER
// ============================================================
function buildTicker() {
  const items = [
    ...MARKET_DATA.crypto.slice(0,4).map(a => ({ sym: a.sym, price: fmtPrice(a.price, a.sym), chg: a.change })),
    ...MARKET_DATA.indices.slice(0,4).map(a => ({ sym: a.sym, price: a.price.toLocaleString(), chg: a.change })),
    ...MARKET_DATA.forex.slice(0,4).map(a => ({ sym: a.sym, price: a.price.toString(), chg: a.change })),
    ...MARKET_DATA.commodities.slice(0,4).map(a => ({ sym: a.sym, price: '$'+a.price, chg: a.change })),
  ];
  const html = items.map(i => `
    <div class="ticker-item">
      <span class="sym">${i.sym}</span>
      <span class="price">${i.price}</span>
      <span class="chg ${i.chg >= 0 ? 'up':'down'}">${i.chg >= 0 ? '+' : ''}${i.chg}%</span>
    </div>
  `).join('');
  document.getElementById('ticker').innerHTML = html + html; // duplicate for infinite scroll
}
buildTicker();

// ============================================================
// NAVIGATION
// ============================================================
function showSection(id) {
  document.querySelectorAll('.section').forEach(s => s.classList.remove('active'));
  document.querySelectorAll('.nav-btn').forEach(b => b.classList.remove('active'));
  document.getElementById(id).classList.add('active');
  event.target.classList.add('active');
  // Render charts when section becomes visible
  setTimeout(() => renderCharts(id), 50);
}

// ============================================================
// HELPERS
// ============================================================
function fmtPrice(price, sym) {
  if (price > 1000) return '$' + price.toLocaleString();
  if (price < 1) return '$' + price.toFixed(4);
  return '$' + price.toFixed(2);
}

function chgBadge(chg) {
  const cls = chg >= 0 ? 'up' : 'down';
  const arrow = chg >= 0 ? '▲' : '▼';
  return `<span class="badge ${cls}">${arrow} ${Math.abs(chg).toFixed(2)}%</span>`;
}

function miniSpark(vals, color) {
  const max = Math.max(...vals), min = Math.min(...vals);
  return `<svg class="sparkline" viewBox="0 0 90 36" preserveAspectRatio="none">
    <polyline fill="none" stroke="${color}" stroke-width="2"
      points="${vals.map((v,i) => `${i*(90/(vals.length-1))},${36-((v-min)/(max-min||1))*32}`).join(' ')}"/>
  </svg>`;
}

function randomSpark(base, n=8) {
  return Array.from({length:n}, (_,i) => base + (Math.random()-0.5)*base*0.04);
}

// ============================================================
// OVERVIEW KPI
// ============================================================
function renderOverviewKPI() {
  const cards = [
    { label: 'BITCOIN', value: '$67,655', sub: 'BTC/USD', badge: '+2.07%', dir: 'up', color: '#F7931A' },
    { label: 'S&P 500', value: '6,881', sub: 'SPX — EE.UU.', badge: '+0.56%', dir: 'up', color: '#0088FF' },
    { label: 'ORO', value: '$5,112', sub: 'XAU/USD / oz', badge: '+0.82%', dir: 'up', color: '#FFD700' },
    { label: 'PETRÓLEO WTI', value: '$78.4', sub: 'WTI / barril', badge: '-0.64%', dir: 'down', color: '#FF6600' },
  ];
  document.getElementById('kpi-cards').innerHTML = cards.map(c => `
    <div class="card">
      <div class="card-label">${c.label}</div>
      <div class="card-value" style="color:${c.color}">${c.value}</div>
      <div style="display:flex;align-items:center;justify-content:space-between;margin-top:8px">
        <span class="card-sub">${c.sub}</span>
        ${chgBadge(parseFloat(c.badge))}
      </div>
    </div>
  `).join('');
}

// ============================================================
// MOVERS TABLE
// ============================================================
function renderMovers() {
  const all = [
    ...MARKET_DATA.crypto.map(a => ({...a, cat:'Crypto'})),
    ...MARKET_DATA.indices.map(a => ({...a, cat:'Índice'})),
    ...MARKET_DATA.commodities.map(a => ({...a, cat:'Commodity'})),
  ].sort((a,b) => Math.abs(b.change) - Math.abs(a.change)).slice(0,8);

  document.getElementById('movers-table').innerHTML = `
    <thead><tr>
      <th>Activo</th><th>Precio</th><th>Cambio</th><th>Categoría</th><th>Tendencia</th>
    </tr></thead>
    <tbody>${all.map(a => `
      <tr>
        <td><div class="asset-name">
          <div class="asset-icon" style="background:rgba(${hexToRgb(a.color||'#888')},0.15);border:1px solid rgba(${hexToRgb(a.color||'#888')},0.3)">${a.icon}</div>
          <div><div class="asset-sym">${a.sym}</div><div class="asset-full">${a.name}</div></div>
        </div></td>
        <td style="font-family:'Space Mono',monospace;font-weight:700">${fmtPrice(a.price, a.sym)}</td>
        <td>${chgBadge(a.change)}</td>
        <td><span class="tag">${a.cat}</span></td>
        <td>${miniSpark(randomSpark(a.price), a.change >= 0 ? '#00e676':'#ff3d57')}</td>
      </tr>
    `).join('')}</tbody>
  `;
}

// ============================================================
// ALERTS
// ============================================================
function renderAlerts() {
  const alerts = [
    { icon: '🚨', text: '<strong>Bitcoin</strong> se acerca a resistencia clave de <strong>$68.000</strong> — Volumen aumentando', time: '14:32' },
    { icon: '⚡', text: '<strong>IPC EE.UU.</strong> a las 15:30 — Evento de alta volatilidad esperado', time: '14:15' },
    { icon: '🔥', text: '<strong>Oro</strong> supera máximo histórico — Nuevo ATH confirmado', time: '13:58' },
    { icon: '📊', text: '<strong>Fallo SCOTUS</strong> sobre aranceles impacta positivamente en mercados emergentes', time: '12:41' },
  ];
  document.getElementById('alerts-container').innerHTML = alerts.map(a => `
    <div class="alert">
      <span class="alert-icon">${a.icon}</span>
      <span style="font-size:13px">${a.text}</span>
      <span class="alert-time">${a.time}</span>
    </div>
  `).join('');
}

// ============================================================
// CRYPTO SECTION
// ============================================================
function renderCrypto() {
  const kpi = MARKET_DATA.crypto.slice(0,4);
  document.getElementById('crypto-kpi').innerHTML = kpi.map(c => `
    <div class="card">
      <div class="card-label">${c.sym}</div>
      <div class="card-value" style="color:${c.color}">${fmtPrice(c.price, c.sym)}</div>
      <div style="display:flex;align-items:center;justify-content:space-between;margin-top:8px">
        <span class="card-sub">Cap: ${c.cap}</span>
        ${chgBadge(c.change)}
      </div>
      <div class="progress-wrap"><div class="progress-fill" style="width:${40+c.change*5}%;background:${c.color}"></div></div>
    </div>
  `).join('');

  // Dominance
  const dom = [
    { sym:'BTC', pct:58.2, color:'#F7931A'},
    { sym:'ETH', pct:10.2, color:'#627EEA'},
    { sym:'BNB', pct:3.8, color:'#F3BA2F'},
    { sym:'SOL', pct:4.1, color:'#9945FF'},
    { sym:'Otros', pct:23.7, color:'#4a5166'},
  ];
  document.getElementById('dominance-bars').innerHTML = dom.map(d => `
    <div style="flex:1;min-width:100px">
      <div style="display:flex;justify-content:space-between;margin-bottom:6px">
        <span style="font-size:12px;color:var(--text2)">${d.sym}</span>
        <span style="font-family:'Space Mono',monospace;font-size:12px;font-weight:700;color:${d.color}">${d.pct}%</span>
      </div>
      <div class="dom-bar"><div class="dom-fill" style="width:${d.pct}%;background:${d.color}"></div></div>
    </div>
  `).join('');

  // Table
  document.getElementById('crypto-table').innerHTML = `
    <thead><tr><th>Moneda</th><th>Precio</th><th>24H</th><th>Máx 24H</th><th>Mín 24H</th><th>Vol 24H</th><th>Cap. Mercado</th></tr></thead>
    <tbody>${MARKET_DATA.crypto.map(c => `
      <tr>
        <td><div class="asset-name">
          <div class="asset-icon" style="background:rgba(${hexToRgb(c.color)},0.15);border:1px solid rgba(${hexToRgb(c.color)},0.3);font-weight:700;color:${c.color}">${c.icon}</div>
          <div><div class="asset-sym">${c.sym}</div><div class="asset-full">${c.name}</div></div>
        </div></td>
        <td style="font-family:'Space Mono',monospace;font-weight:700;font-size:14px">${fmtPrice(c.price,c.sym)}</td>
        <td>${chgBadge(c.change)}</td>
        <td style="color:var(--green);font-family:'Space Mono',monospace;font-size:12px">${fmtPrice(c.high,c.sym)}</td>
        <td style="color:var(--red);font-family:'Space Mono',monospace;font-size:12px">${fmtPrice(c.low,c.sym)}</td>
        <td style="color:var(--text2);font-size:13px">$${c.vol}</td>
        <td style="color:var(--text2);font-size:13px">$${c.cap}</td>
      </tr>
    `).join('')}</tbody>
  `;
}

// ============================================================
// INDICES SECTION
// ============================================================
function renderIndices() {
  document.getElementById('indices-kpi').innerHTML = MARKET_DATA.indices.slice(0,4).map(a => `
    <div class="card">
      <div class="card-label">${a.sym}</div>
      <div class="card-value" style="color:${a.change >= 0 ? 'var(--green)':'var(--red)'}">${a.price.toLocaleString()}</div>
      <div style="display:flex;align-items:center;justify-content:space-between;margin-top:8px">
        <span class="card-sub">${a.icon} ${a.country}</span>
        ${chgBadge(a.change)}
      </div>
    </div>
  `).join('');

  document.getElementById('indices-table').innerHTML = `
    <thead><tr><th>Índice</th><th>Precio</th><th>Cambio</th><th>País</th><th>Volumen</th></tr></thead>
    <tbody>${MARKET_DATA.indices.map(a => `
      <tr>
        <td><div class="asset-name">
          <div class="asset-icon" style="font-size:18px;background:rgba(255,255,255,0.03)">${a.icon}</div>
          <div><div class="asset-sym">${a.sym}</div><div class="asset-full">${a.name}</div></div>
        </div></td>
        <td style="font-family:'Space Mono',monospace;font-weight:700">${a.price.toLocaleString()}</td>
        <td>${chgBadge(a.change)}</td>
        <td style="color:var(--text2);font-size:13px">${a.country}</td>
        <td><span class="tag">${a.vol}</span></td>
      </tr>
    `).join('')}</tbody>
  `;
}

// ============================================================
// FOREX
// ============================================================
function renderForex() {
  document.getElementById('forex-kpi').innerHTML = MARKET_DATA.forex.slice(0,4).map(a => `
    <div class="card">
      <div class="card-label">${a.sym}</div>
      <div class="card-value" style="color:${a.color}">${a.price}</div>
      <div style="display:flex;align-items:center;justify-content:space-between;margin-top:8px">
        <span class="card-sub">${a.name}</span>
        ${chgBadge(a.change)}
      </div>
    </div>
  `).join('');

  document.getElementById('forex-table').innerHTML = `
    <thead><tr><th>Par</th><th>Precio</th><th>Cambio</th><th>Tendencia</th></tr></thead>
    <tbody>${MARKET_DATA.forex.map(a => `
      <tr>
        <td><div class="asset-name">
          <div class="asset-icon" style="background:rgba(${hexToRgb(a.color)},0.15);border:1px solid rgba(${hexToRgb(a.color)},0.3);color:${a.color};font-weight:700;font-size:12px">${a.icon}</div>
          <div><div class="asset-sym">${a.sym}</div><div class="asset-full">${a.name}</div></div>
        </div></td>
        <td style="font-family:'Space Mono',monospace;font-weight:700">${a.price}</td>
        <td>${chgBadge(a.change)}</td>
        <td>${miniSpark(randomSpark(a.price), a.change >= 0 ? '#00e676':'#ff3d57')}</td>
      </tr>
    `).join('')}</tbody>
  `;
}

// ============================================================
// COMMODITIES
// ============================================================
function renderCommodities() {
  document.getElementById('comm-kpi').innerHTML = MARKET_DATA.commodities.slice(0,4).map(a => `
    <div class="card">
      <div class="card-label">${a.sym}</div>
      <div class="card-value" style="color:${a.color}">${a.price} <span style="font-size:16px;font-family:'DM Sans'">${a.unit}</span></div>
      <div style="display:flex;align-items:center;justify-content:space-between;margin-top:8px">
        <span class="card-sub">${a.name}</span>
        ${chgBadge(a.change)}
      </div>
    </div>
  `).join('');

  document.getElementById('comm-table').innerHTML = `
    <thead><tr><th>Commodity</th><th>Precio</th><th>Unidad</th><th>Cambio</th><th>Tendencia</th></tr></thead>
    <tbody>${MARKET_DATA.commodities.map(a => `
      <tr>
        <td><div class="asset-name">
          <span style="font-size:22px">${a.icon}</span>
          <div><div class="asset-sym">${a.sym}</div><div class="asset-full">${a.name}</div></div>
        </div></td>
        <td style="font-family:'Space Mono',monospace;font-weight:700;color:${a.color}">${a.price}</td>
        <td style="font-size:12px;color:var(--text3)">${a.unit}</td>
        <td>${chgBadge(a.change)}</td>
        <td>${miniSpark(randomSpark(a.price), a.change >= 0 ? '#00e676':'#ff3d57')}</td>
      </tr>
    `).join('')}</tbody>
  `;
}

// ============================================================
// ANALYSIS
// ============================================================
function renderAnalysis() {
  const btcSig = [
    { name: 'RSI (14)', val: '56.4', cls: 'neutral', txt: 'NEUTRAL' },
    { name: 'MACD', val: '+124', cls: 'up', txt: 'COMPRA' },
    { name: 'Media 50D', val: '$64.800', cls: 'up', txt: 'SOBRE' },
    { name: 'Media 200D', val: '$58.200', cls: 'up', txt: 'SOBRE' },
    { name: 'Bollinger', val: 'Medio', cls: 'neutral', txt: 'NEUTRAL' },
    { name: 'Volumen', val: 'Normal', cls: 'neutral', txt: 'NORMAL' },
    { name: 'Stoch RSI', val: '62', cls: 'up', txt: 'COMPRA' },
    { name: 'ADX', val: '28', cls: 'up', txt: 'TENDENCIA' },
  ];
  document.getElementById('btc-signals').innerHTML = btcSig.map(s => `
    <div class="signal-row">
      <span class="signal-name">${s.name}</span>
      <div style="display:flex;gap:10px;align-items:center">
        <span style="font-family:'Space Mono',monospace;font-size:12px;color:var(--text2)">${s.val}</span>
        <span class="badge ${s.cls}" style="font-size:10px">${s.txt}</span>
      </div>
    </div>
  `).join('');

  const spxSig = [
    { name: 'RSI (14)', val: '68.2', cls: 'down', txt: 'SOBRECOMP.' },
    { name: 'MACD', val: '+18', cls: 'neutral', txt: 'DEBIL' },
    { name: 'Media 50D', val: '6.720', cls: 'up', txt: 'SOBRE' },
    { name: 'Media 200D', val: '6.100', cls: 'up', txt: 'SOBRE' },
    { name: 'VIX', val: '19.62', cls: 'up', txt: 'BAJO' },
    { name: 'P/E S&P', val: '24.8x', cls: 'down', txt: 'CARO' },
    { name: 'Momentum', val: 'Débil', cls: 'neutral', txt: 'NEUTRAL' },
    { name: 'Soporte', val: '6.720', cls: 'up', txt: 'ACTIVO' },
  ];
  document.getElementById('spx-signals').innerHTML = spxSig.map(s => `
    <div class="signal-row">
      <span class="signal-name">${s.name}</span>
      <div style="display:flex;gap:10px;align-items:center">
        <span style="font-family:'Space Mono',monospace;font-size:12px;color:var(--text2)">${s.val}</span>
        <span class="badge ${s.cls}" style="font-size:10px">${s.txt}</span>
      </div>
    </div>
  `).join('');

  const goldCards = [
    { label: 'TENDENCIA', val: 'ALCISTA FUERTE', cls: 'up' },
    { label: 'SOPORTE', val: '$5.000/oz', cls: 'up' },
    { label: 'TARGET', val: '$5.300/oz', cls: 'up' },
    { label: 'RSI (14)', val: '71 — SOBRECOMP.', cls: 'down' },
    { label: 'MEDIA 50D', val: '$4.820/oz', cls: 'up' },
    { label: 'SEÑAL', val: 'COMPRA ESCALONADA', cls: 'up' },
  ];
  document.getElementById('gold-signals').innerHTML = goldCards.map(g => `
    <div style="text-align:center">
      <div style="font-size:10px;letter-spacing:1.5px;color:var(--text3);font-family:'Space Mono',monospace;margin-bottom:6px">${g.label}</div>
      <span class="badge ${g.cls}" style="font-size:11px">${g.val}</span>
    </div>
  `).join('');

  // Macro Calendar
  document.getElementById('macro-calendar').innerHTML = `
    <table class="data-table">
      <thead><tr><th>Fecha</th><th>Hora</th><th>Evento</th><th>Anterior</th><th>Estimado</th><th>Impacto</th></tr></thead>
      <tbody>${MACRO_EVENTS.map(e => `
        <tr>
          <td style="font-family:'Space Mono',monospace;font-size:12px;font-weight:700;color:var(--accent4)">${e.date}</td>
          <td style="font-family:'Space Mono',monospace;font-size:12px">${e.time}</td>
          <td style="font-weight:500">${e.event}</td>
          <td style="font-family:'Space Mono',monospace;font-size:12px;color:var(--text2)">${e.prev}</td>
          <td style="font-family:'Space Mono',monospace;font-size:12px;color:var(--accent)">${e.est}</td>
          <td><span class="badge ${e.impact === 'high' ? 'down':'neutral'}" style="font-size:10px">${e.impact === 'high' ? '🔴 ALTO':'🟡 MEDIO'}</span></td>
        </tr>
      `).join('')}</tbody>
    </table>
  `;
}

// ============================================================
// NEWS
// ============================================================
function renderNews() {
  document.getElementById('news-main').innerHTML = `
    <div class="card-label" style="margin-bottom:16px">ÚLTIMAS NOTICIAS</div>
    ${NEWS_DATA.map(n => `
      <div class="news-item">
        <div class="news-meta">
          <span class="news-source">${n.source}</span>
          ${n.hot ? '<span class="badge down" style="font-size:9px;padding:2px 6px">🔥 TRENDING</span>':''}
          <span class="news-time">${n.time}</span>
        </div>
        <div class="news-title">${n.title}</div>
        <div class="news-tags">${n.tags.map(t => `<span class="news-tag">${t}</span>`).join('')}</div>
      </div>
    `).join('')}
  `;

  const sidebar = [
    { label: 'SENTIMIENTO GLOBAL', val: 'NEUTRAL 52/100', cls: 'neutral' },
    { label: 'DOMINANCIA BTC', val: '58.2%', cls: 'up' },
    { label: 'OPEN INTEREST BTC', val: '$28.4B ↑', cls: 'up' },
    { label: 'FINANCIACIÓN PERPS', val: '+0.018% (LONGS)', cls: 'up' },
    { label: 'FLUJO STABLECOINS', val: '+$1.2B (ENTRADA)', cls: 'up' },
    { label: 'ETF BTC FLUJO HOY', val: '+$420M', cls: 'up' },
  ];

  document.getElementById('news-sidebar').innerHTML = `
    <div class="card-label" style="margin-bottom:16px">MÉTRICAS ON-CHAIN</div>
    ${sidebar.map(s => `
      <div class="signal-row">
        <span class="signal-name" style="font-size:12px">${s.label}</span>
        <span class="badge ${s.cls}" style="font-size:11px">${s.val}</span>
      </div>
    `).join('')}
  `;
}

// ============================================================
// CHARTS (Canvas)
// ============================================================
let charts = {};

function generateLineData(base, n=20, vol=0.02) {
  let v = base;
  return Array.from({length:n}, () => { v *= 1 + (Math.random()-0.48)*vol; return +v.toFixed(2); });
}

const LABELS_7D = ['Lun','Mar','Mié','Jue','Vie','Sáb','Dom'];
const LABELS_30D = Array.from({length:30}, (_,i) => i+1);

function drawLineChart(canvasId, datasets, labels) {
  const canvas = document.getElementById(canvasId);
  if (!canvas) return;
  if (charts[canvasId]) { charts[canvasId].destroy(); }

  const ctx = canvas.getContext('2d');
  // Simple manual chart
  const W = canvas.offsetWidth || 600;
  const H = canvas.offsetHeight || 240;
  canvas.width = W;
  canvas.height = H;

  const PAD = { t:20, r:20, b:30, l:50 };
  const cW = W - PAD.l - PAD.r;
  const cH = H - PAD.t - PAD.b;

  ctx.clearRect(0,0,W,H);

  // Background
  ctx.fillStyle = '#0f1525';
  ctx.fillRect(0,0,W,H);

  // Grid
  ctx.strokeStyle = 'rgba(255,255,255,0.04)';
  ctx.lineWidth = 1;
  for(let i=0;i<=4;i++) {
    const y = PAD.t + (cH/4)*i;
    ctx.beginPath(); ctx.moveTo(PAD.l, y); ctx.lineTo(PAD.l+cW, y); ctx.stroke();
  }

  datasets.forEach(ds => {
    const vals = ds.data;
    const allVals = datasets.flatMap(d => d.data);
    const min = Math.min(...allVals), max = Math.max(...allVals);
    const range = max - min || 1;

    const pts = vals.map((v,i) => ({
      x: PAD.l + (i/(vals.length-1))*cW,
      y: PAD.t + cH - ((v-min)/range)*cH
    }));

    // Area fill
    const grad = ctx.createLinearGradient(0, PAD.t, 0, PAD.t+cH);
    grad.addColorStop(0, ds.color+'33');
    grad.addColorStop(1, ds.color+'00');

    ctx.beginPath();
    ctx.moveTo(pts[0].x, PAD.t+cH);
    pts.forEach(p => ctx.lineTo(p.x, p.y));
    ctx.lineTo(pts[pts.length-1].x, PAD.t+cH);
    ctx.closePath();
    ctx.fillStyle = grad;
    ctx.fill();

    // Line
    ctx.beginPath();
    ctx.strokeStyle = ds.color;
    ctx.lineWidth = 2;
    pts.forEach((p,i) => i===0 ? ctx.moveTo(p.x, p.y) : ctx.lineTo(p.x, p.y));
    ctx.stroke();

    // Dots
    ctx.fillStyle = ds.color;
    pts.forEach((p,i) => {
      if(i===0||i===pts.length-1||i%Math.ceil(pts.length/5)===0) {
        ctx.beginPath(); ctx.arc(p.x, p.y, 3, 0, Math.PI*2); ctx.fill();
      }
    });
  });

  // Labels
  if(labels) {
    ctx.fillStyle = 'rgba(122,132,153,0.8)';
    ctx.font = '10px Space Mono';
    ctx.textAlign = 'center';
    const step = Math.ceil(labels.length / 6);
    labels.forEach((l,i) => {
      if(i % step === 0 || i === labels.length-1) {
        const x = PAD.l + (i/(labels.length-1))*cW;
        ctx.fillText(l, x, H-8);
      }
    });
  }

  charts[canvasId] = {destroy: () => {}};
}

function drawGauge(canvasId, value) {
  const canvas = document.getElementById(canvasId);
  if(!canvas) return;
  const ctx = canvas.getContext('2d');
  const W=220, H=130;
  canvas.width=W; canvas.height=H;
  ctx.clearRect(0,0,W,H);

  const cx=110, cy=110, r=80;
  const startA = Math.PI, endA = 2*Math.PI;

  // Background arc
  ctx.beginPath();
  ctx.arc(cx, cy, r, startA, endA);
  ctx.strokeStyle = 'rgba(255,255,255,0.07)';
  ctx.lineWidth = 16;
  ctx.stroke();

  // Color gradient arc
  const pct = value / 100;
  const color = value < 25 ? '#ff3d57' : value < 45 ? '#ff8844' : value < 55 ? '#ffaa00' : value < 75 ? '#88dd00' : '#00e676';
  ctx.beginPath();
  ctx.arc(cx, cy, r, startA, startA + pct*Math.PI);
  ctx.strokeStyle = color;
  ctx.lineWidth = 16;
  ctx.lineCap = 'round';
  ctx.stroke();

  // Needle
  const angle = Math.PI + pct*Math.PI;
  ctx.beginPath();
  ctx.moveTo(cx, cy);
  ctx.lineTo(cx + Math.cos(angle)*65, cy + Math.sin(angle)*65);
  ctx.strokeStyle = color;
  ctx.lineWidth = 2;
  ctx.stroke();

  ctx.beginPath();
  ctx.arc(cx, cy, 5, 0, Math.PI*2);
  ctx.fillStyle = color;
  ctx.fill();

  document.getElementById('fg-value').style.color = color;
}

function renderCharts(section) {
  if(section === 'overview' || section === undefined) {
    drawLineChart('overviewChart', [
      { data: generateLineData(6700, 20, 0.008), color: '#F7931A' },
      { data: generateLineData(6800, 20, 0.005), color: '#0088FF' },
    ], LABELS_7D);
    drawGauge('fgGauge', 52);
  }
  if(section === 'crypto') {
    drawLineChart('btcChart', [
      { data: generateLineData(64000, 14, 0.012), color: '#F7931A' },
    ], LABELS_7D);
  }
  if(section === 'indices') {
    drawLineChart('indicesChart', [
      { data: generateLineData(6800, 30, 0.006), color: '#0088FF' },
      { data: generateLineData(22600, 30, 0.007), color: '#00E676' },
      { data: generateLineData(49500, 30, 0.004), color: '#FFAA00' },
    ], LABELS_30D);
  }
  if(section === 'forex') {
    drawLineChart('forexChart', [
      { data: generateLineData(103.5, 30, 0.003), color: '#FFAA00' },
    ], LABELS_30D);
  }
  if(section === 'commodities') {
    drawLineChart('commChart', [
      { data: generateLineData(5000, 30, 0.008), color: '#FFD700' },
      { data: generateLineData(78, 30, 0.012), color: '#FF6600' },
    ], LABELS_30D);
  }
}

// ============================================================
// REFRESH
// ============================================================
function refreshData() {
  const icon = document.getElementById('refresh-icon');
  if(icon) { icon.classList.add('spin'); }
  setTimeout(() => {
    if(icon) icon.classList.remove('spin');
    // Simulate price update
    MARKET_DATA.crypto.forEach(c => {
      c.price *= (1 + (Math.random()-0.499)*0.003);
      c.change += (Math.random()-0.5)*0.1;
      c.price = +c.price.toFixed(c.price > 100 ? 2 : 4);
    });
    initAll();
    buildTicker();
  }, 800);
}

// ============================================================
// UTILS
// ============================================================
function hexToRgb(hex) {
  if(!hex || hex[0]!=='#') return '128,128,128';
  const r = parseInt(hex.slice(1,3),16);
  const g = parseInt(hex.slice(3,5),16);
  const b = parseInt(hex.slice(5,7),16);
  return `${r},${g},${b}`;
}

// ============================================================
// INIT
// ============================================================
function initAll() {
  renderOverviewKPI();
  renderMovers();
  renderAlerts();
  renderCrypto();
  renderIndices();
  renderForex();
  renderCommodities();
  renderAnalysis();
  renderNews();
  renderCharts();
}

window.addEventListener('load', () => {
  initAll();
  // Auto-refresh every 30s
  setInterval(() => {
    MARKET_DATA.crypto.forEach(c => {
      c.price *= (1 + (Math.random()-0.499)*0.001);
      c.change += (Math.random()-0.5)*0.05;
    });
    buildTicker();
    renderOverviewKPI();
    renderMovers();
  }, 30000);
});

// Resize charts
window.addEventListener('resize', () => {
  const active = document.querySelector('.section.active');
  if(active) renderCharts(active.id);
});
</script>
</body>
</html>
