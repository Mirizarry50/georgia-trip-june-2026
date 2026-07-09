<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>June 2026 Georgia Trip — Money Summary</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,400;9..144,500;9..144,600;9..144,700&family=Public+Sans:wght@400;500;600;700&family=IBM+Plex+Mono:wght@400;500;600&display=swap" rel="stylesheet">
<style>
  :root{
    --bg: #F6F1E5;
    --bg-deep: #EFE7D4;
    --card: #FFFDF8;
    --ink: #1B3634;
    --ink-soft: #4A6360;
    --teal: #15514E;
    --teal-dark: #0C3735;
    --teal-tint: #E4EEEC;
    --tan: #D9A85F;
    --tan-tint: #F5E6C8;
    --orange: #BD5B2A;
    --orange-tint: #F6E1D3;
    --green: #2E7A62;
    --green-tint: #DCEEE6;
    --line: #DFD2B4;
    --shadow: 0 10px 30px -12px rgba(20,55,52,0.25);
    --radius: 14px;
  }

  *{ box-sizing: border-box; }
  html{ scroll-behavior: smooth; }
  body{
    margin:0;
    background: var(--bg);
    color: var(--ink);
    font-family: "Public Sans", system-ui, sans-serif;
    line-height: 1.5;
  }

  h1,h2,h3, .display{
    font-family: "Fraunces", Georgia, serif;
    font-weight: 600;
    color: var(--teal-dark);
    letter-spacing: -0.01em;
  }

  .num, .money, table td.num, .status-pill, .badge{
    font-family: "IBM Plex Mono", "Courier New", monospace;
    font-feature-settings: "tnum";
  }

  a{ color: var(--teal); }

  button{ font-family: inherit; cursor: pointer; }
  button:focus-visible, a:focus-visible, input:focus-visible, [tabindex]:focus-visible{
    outline: 3px solid var(--orange);
    outline-offset: 2px;
  }

  .wrap{ max-width: 1080px; margin: 0 auto; padding: 0 20px 80px; }

  /* ---------- HERO ---------- */
  .hero{
    position: relative;
    background: linear-gradient(180deg, var(--teal-dark) 0%, var(--teal) 100%);
    color: #F3ECDA;
    overflow: hidden;
    padding: 56px 20px 84px;
  }
  .hero-inner{ max-width: 1080px; margin: 0 auto; position: relative; z-index: 2; }
  .hero .eyebrow{
    display:inline-flex; align-items:center; gap:8px;
    font-family:"IBM Plex Mono", monospace; font-size: 12px; letter-spacing: .12em; text-transform: uppercase;
    color: var(--tan-tint); background: rgba(217,168,95,0.15); border:1px solid rgba(217,168,95,0.4);
    padding: 5px 12px; border-radius: 999px; margin-bottom: 18px;
  }
  .hero h1{ color:#FBF6EA; font-size: clamp(28px, 4.4vw, 44px); margin: 0 0 10px; max-width: 720px; }
  .hero p.subtitle{ font-size: clamp(15px, 2vw, 18px); color: #CFE3DE; margin: 0 0 22px; max-width: 620px; }
  .status-banner{
    display:flex; gap: 12px; align-items:flex-start;
    background: rgba(246,241,229,0.08);
    border: 1px solid rgba(246,241,229,0.22);
    border-radius: var(--radius);
    padding: 14px 16px; max-width: 640px; font-size: 14.5px; color: #E7EFE9;
  }
  .status-banner svg{ flex-shrink:0; margin-top: 2px; }

  .wave-bg{ position:absolute; inset:0; opacity: 0.5; z-index:1; }

  /* ---------- SUMMARY CARDS ---------- */
  .summary-grid{
    display:grid; grid-template-columns: repeat(4, 1fr); gap:16px;
    margin-top: -52px; position: relative; z-index: 3;
  }
  .sum-card{
    background: var(--card); border-radius: var(--radius); box-shadow: var(--shadow);
    padding: 18px 18px 16px; border: 1px solid var(--line);
    display:flex; flex-direction:column; gap: 6px;
  }
  .sum-card .label{ font-size: 12.5px; text-transform: uppercase; letter-spacing:.06em; color: var(--ink-soft); font-weight:600; }
  .sum-card .amount{ font-size: 26px; font-weight: 600; color: var(--teal-dark); }
  .sum-card .dir{
    align-self:flex-start; font-size: 11.5px; padding: 3px 9px; border-radius: 999px; font-weight:600;
    display:inline-flex; align-items:center; gap:5px;
  }
  .dir.to-organizer{ background: var(--orange-tint); color: var(--orange); }
  .dir.from-organizer{ background: var(--green-tint); color: var(--green); }
  .dir.neutral{ background: var(--tan-tint); color: #8A6420; }

  section{ margin-top: 52px; }
  .section-head{ display:flex; align-items:baseline; justify-content:space-between; gap:16px; flex-wrap:wrap; margin-bottom: 6px; }
  .section-head h2{ font-size: 24px; margin: 0; }
  .section-note{ color: var(--ink-soft); font-size: 14px; margin: 4px 0 20px; max-width: 680px; }

  /* ---------- CONTROLS ---------- */
  .controls{
    display:flex; gap:12px; flex-wrap:wrap; align-items:center;
    background: var(--card); border: 1px solid var(--line); border-radius: var(--radius);
    padding: 14px 16px; margin-top: 30px; box-shadow: var(--shadow);
  }
  .search-box{ position:relative; flex: 1 1 220px; min-width: 200px; }
  .search-box input{
    width:100%; padding: 10px 12px 10px 34px; border-radius: 10px; border: 1px solid var(--line);
    background: var(--bg); font-size: 14.5px; color: var(--ink);
  }
  .search-box svg{ position:absolute; left:10px; top:50%; transform:translateY(-50%); opacity:.6; }
  .filter-btns{ display:flex; gap:8px; flex-wrap:wrap; }
  .filter-btn{
    border: 1px solid var(--line); background: var(--bg); color: var(--ink-soft);
    padding: 8px 14px; border-radius: 999px; font-size: 13.5px; font-weight:600; transition: all .15s ease;
  }
  .filter-btn:hover{ border-color: var(--teal); color: var(--teal-dark); }
  .filter-btn.active{ background: var(--teal); color: #fff; border-color: var(--teal); }
  .print-btn{
    border: 1px solid var(--teal); background: var(--teal); color:#fff; padding: 9px 16px;
    border-radius: 10px; font-weight:600; font-size: 13.5px; display:inline-flex; gap:7px; align-items:center;
  }
  .print-btn:hover{ background: var(--teal-dark); }

  /* ---------- COUPLE CARDS ---------- */
  .couple-grid{ display:grid; grid-template-columns: repeat(3, 1fr); gap: 14px; }
  .couple-card{
    background: var(--card); border:1px solid var(--line); border-radius: var(--radius);
    padding: 16px; box-shadow: var(--shadow); display:flex; flex-direction:column; gap:10px;
  }
  .couple-card .row-top{ display:flex; justify-content:space-between; align-items:flex-start; gap: 10px; }
  .couple-card .name{ font-family:"Fraunces", serif; font-size: 17px; font-weight: 600; color: var(--teal-dark); }
  .couple-card .due{ font-size: 20px; font-weight:600; color: var(--orange); }
  .toggle-row{ display:flex; align-items:center; justify-content:space-between; gap: 10px; }
  .status-toggle{
    border: 1px solid var(--line); background: var(--bg); border-radius: 999px; padding: 6px 12px;
    font-size: 12.5px; font-weight:600; display:inline-flex; align-items:center; gap:6px;
  }
  .status-toggle[data-status="paid"]{ background: var(--green-tint); color: var(--green); border-color: var(--green); }
  .status-toggle[data-status="unpaid"]{ background: var(--orange-tint); color: var(--orange); border-color: var(--orange); }
  .note-input{
    border: none; border-top: 1px dashed var(--line); background: transparent; padding-top: 8px;
    font-size: 12.5px; color: var(--ink-soft); width: 100%;
  }
  .note-input::placeholder{ color: #A7998A; }

  .footer-total{
    margin-top: 18px; display:flex; justify-content:space-between; align-items:baseline;
    background: var(--teal-tint); border-radius: var(--radius); padding: 14px 18px; flex-wrap:wrap; gap: 8px;
  }
  .footer-total .total-amt{ font-size: 22px; font-weight:700; color: var(--teal-dark); }
  .rounding-note{ font-size: 12.5px; color: var(--ink-soft); margin-top: 8px; }

  /* ---------- TABLES ---------- */
  .table-scroll{ overflow-x:auto; border-radius: var(--radius); box-shadow: var(--shadow); border: 1px solid var(--line); }
  table{ width:100%; border-collapse: collapse; background: var(--card); min-width: 560px; }
  thead th{
    text-align:left; font-size: 12.5px; text-transform:uppercase; letter-spacing:.05em;
    color: #fff; background: var(--teal); padding: 12px 14px; font-weight:600; white-space:nowrap;
  }
  thead th.num, tbody td.num{ text-align:right; }
  tbody td{ padding: 11px 14px; border-bottom: 1px solid var(--line); font-size: 14.5px; }
  tbody tr:last-child td{ border-bottom:none; }
  tbody tr.total-row td{ font-weight:700; background: var(--tan-tint); }
  tbody tr:hover td{ background: var(--bg-deep); }
  tbody tr.total-row:hover td{ background: var(--tan-tint); }
  .status-pill{
    font-size: 11.5px; font-weight:700; padding: 4px 10px; border-radius: 999px; border: none;
    display:inline-flex; align-items:center; gap:5px;
  }
  .status-pill[data-status="paid"]{ background: var(--green-tint); color: var(--green); }
  .status-pill[data-status="unpaid"]{ background: var(--orange-tint); color: var(--orange); }

  /* ---------- SETTLEMENT CARDS ---------- */
  .settle-grid{ display:grid; grid-template-columns: repeat(3, 1fr); gap: 18px; }
  .ticket{
    background: var(--card); border-radius: var(--radius); box-shadow: var(--shadow);
    border: 1px solid var(--line); overflow:hidden; position:relative;
  }
  .ticket-head{
    padding: 14px 16px 12px; display:flex; justify-content:space-between; align-items:center;
    border-bottom: 1px dashed var(--line); background: var(--bg-deep);
  }
  .ticket-head .p-name{ font-family:"Fraunces", serif; font-weight:600; font-size: 17px; color: var(--teal-dark); }
  .perf{
    height: 14px; background: var(--bg-deep);
    background-image: radial-gradient(circle, var(--bg) 4px, transparent 4.5px);
    background-size: 16px 16px; background-position: -4px center;
    border-bottom: 1px dashed var(--line);
  }
  .ticket-body{ padding: 14px 16px 16px; display:flex; flex-direction:column; gap: 10px; }
  .flow-line{ display:flex; align-items:center; justify-content:space-between; gap: 10px; padding: 9px 10px; border-radius: 10px; }
  .flow-line.out{ background: var(--orange-tint); }
  .flow-line.in{ background: var(--green-tint); }
  .flow-line .label{ display:flex; align-items:center; gap:8px; font-size: 13.5px; font-weight:600; }
  .flow-line.out .label{ color: var(--orange); }
  .flow-line.in .label{ color: var(--green); }
  .flow-line .amt{ font-size: 15.5px; font-weight:700; }
  .net-line{
    display:flex; justify-content:space-between; align-items:center; font-size: 12px; color: var(--ink-soft);
    border-top: 1px dashed var(--line); padding-top: 8px; margin-top: 2px;
  }
  .net-line .ref-tag{ font-size: 10.5px; text-transform:uppercase; letter-spacing:.05em; background: var(--tan-tint); color:#8A6420; padding: 2px 7px; border-radius:999px; margin-left:6px; }
  .ticket-actions{ display:flex; gap: 8px; padding: 0 16px 16px; }
  .ghost-btn{
    flex:1; border:1px solid var(--line); background: var(--bg); color: var(--teal-dark);
    padding: 8px 10px; border-radius: 9px; font-size: 12.5px; font-weight:600; display:flex; align-items:center; justify-content:center; gap:6px;
  }
  .ghost-btn:hover{ border-color: var(--teal); }
  .ghost-btn.copied{ background: var(--green); color:#fff; border-color: var(--green); }

  .empty-state{
    text-align:center; padding: 40px 20px; color: var(--ink-soft); background: var(--card);
    border: 1px dashed var(--line); border-radius: var(--radius); font-size: 14.5px;
  }

  footer.page-footer{
    margin-top: 60px; padding-top: 24px; border-top: 1px solid var(--line);
    color: var(--ink-soft); font-size: 13px; display:flex; justify-content:space-between; gap: 12px; flex-wrap:wrap;
  }

  [data-label]{}

  @media (max-width: 900px){
    .summary-grid{ grid-template-columns: repeat(2, 1fr); }
    .couple-grid{ grid-template-columns: repeat(2, 1fr); }
    .settle-grid{ grid-template-columns: repeat(2, 1fr); }
  }
  @media (max-width: 640px){
    .summary-grid{ grid-template-columns: 1fr 1fr; margin-top:-40px; }
    .couple-grid, .settle-grid{ grid-template-columns: 1fr; }
    .hero{ padding: 44px 16px 76px; }
    /* Stack tables on mobile */
    .table-scroll table, .table-scroll thead, .table-scroll tbody, .table-scroll th, .table-scroll td, .table-scroll tr{ display:block; }
    .table-scroll thead{ position:absolute; top:-9999px; left:-9999px; }
    .table-scroll tr{ border-bottom: 1px solid var(--line); padding: 10px 12px; }
    .table-scroll tr.total-row{ background: var(--tan-tint); }
    .table-scroll td{ border-bottom:none; padding: 4px 4px; display:flex; justify-content:space-between; }
    .table-scroll td.num{ text-align:right; }
    .table-scroll td[data-label]::before{
      content: attr(data-label); font-weight:600; color: var(--ink-soft); font-family:"Public Sans", sans-serif; font-size:12px; text-transform:uppercase; letter-spacing:.04em;
    }
    .table-scroll{ min-width: 0; }
    table{ min-width: 0; }
  }

  /* ---------- PRINT ---------- */
  @media print{
    .no-print{ display:none !important; }
    body{ background:#fff; color:#000; }
    .hero{ background:#fff !important; color:#000; padding: 10px 0 20px; }
    .hero h1, .hero p.subtitle{ color:#000; }
    .status-banner{ background:#fff; border-color:#999; color:#000; }
    .wave-bg{ display:none; }
    .summary-grid{ margin-top: 10px; }
    .sum-card, .couple-card, .ticket, table{ box-shadow:none !important; break-inside: avoid; }
    section{ margin-top: 24px; }
    .settle-grid{ grid-template-columns: repeat(2,1fr); }
  }
</style>
</head>
<body>

<header class="hero">
  <svg class="wave-bg" viewBox="0 0 1080 300" preserveAspectRatio="none" aria-hidden="true">
    <path d="M0,180 C120,140 240,220 360,190 C480,160 600,230 720,200 C840,170 960,220 1080,190 L1080,300 L0,300 Z" fill="#0C3735" opacity="0.55"/>
    <path d="M0,220 C130,200 260,250 390,225 C520,200 650,255 780,230 C900,208 990,240 1080,222 L1080,300 L0,300 Z" fill="#0A2F2D" opacity="0.65"/>
  </svg>
  <div class="hero-inner">
    <span class="eyebrow">Lake Ledger · Settled Through the Organizer</span>
    <h1>June 2026 Georgia Trip — Money Summary</h1>
    <p class="subtitle">Shared Expenses and Horse Game Settlement</p>
    <div class="status-banner">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true"><path d="M12 2L2 7l10 5 10-5-10-5z" stroke="#F5E6C8" stroke-width="1.6" stroke-linejoin="round"/><path d="M2 12l10 5 10-5M2 17l10 5 10-5" stroke="#F5E6C8" stroke-width="1.6" stroke-linejoin="round"/></svg>
      <span>Every dollar routes through Michael. Couples pay their share to Michael; horse buy‑ins go to Michael; horse payouts come from Michael. Nothing is netted — buy‑ins and payouts are always tracked as separate transactions.</span>
    </div>
  </div>
</header>

<div class="wrap">

  <div class="summary-grid" id="summaryGrid"></div>

  <!-- CONTROLS -->
  <div class="controls no-print">
    <div class="search-box">
      <svg width="16" height="16" viewBox="0 0 24 24" fill="none" aria-hidden="true"><circle cx="11" cy="11" r="7" stroke="#4A6360" stroke-width="1.8"/><path d="M20 20l-3.5-3.5" stroke="#4A6360" stroke-width="1.8" stroke-linecap="round"/></svg>
      <label for="searchInput" class="sr-only" style="position:absolute;left:-9999px;">Search by name</label>
      <input id="searchInput" type="text" placeholder="Search a name…" autocomplete="off">
    </div>
    <div class="filter-btns" role="group" aria-label="Filter by settlement status">
      <button class="filter-btn active" data-filter="all">All</button>
      <button class="filter-btn" data-filter="toOrganizer">Needs to Pay Organizer</button>
      <button class="filter-btn" data-filter="fromOrganizer">Organizer Needs to Pay</button>
      <button class="filter-btn" data-filter="completed">Completed</button>
    </div>
    <button class="print-btn" id="printBtn">
      <svg width="15" height="15" viewBox="0 0 24 24" fill="none"><path d="M6 9V3h12v6M6 18H4a1 1 0 01-1-1v-6a1 1 0 011-1h16a1 1 0 011 1v6a1 1 0 01-1 1h-2M6 14h12v7H6v-7z" stroke="#fff" stroke-width="1.6" stroke-linejoin="round"/></svg>
      Print Summary
    </button>
  </div>

  <!-- COUPLE REIMBURSEMENT -->
  <section id="coupleSection">
    <div class="section-head">
      <h2>Couple Reimbursement</h2>
    </div>
    <p class="section-note">Six couples split the actual shared costs. Each couple owes a fixed <strong>$368.00</strong> — this is the collectible amount and is never recalculated to $367.375.</p>
    <div class="couple-grid" id="coupleGrid"></div>
    <div class="footer-total">
      <div>
        <div style="font-size:12.5px; text-transform:uppercase; letter-spacing:.05em; color:var(--ink-soft); font-weight:600;">Total Collected from Couples</div>
        <div class="rounding-note">Actual shared costs were $2,204.25. Six fixed shares of $368.00 total $2,208.00 — a $3.75 rounding difference above actual cost, kept by design for clean, round collections.</div>
      </div>
      <div class="total-amt num" id="coupleFooterTotal">$2,208.00</div>
    </div>
  </section>

  <!-- HORSE BUY-INS -->
  <section id="buyinSection">
    <div class="section-head"><h2>Horse Buy‑Ins — Players Pay Organizer</h2></div>
    <p class="section-note">The full combined buy‑in each player sends Michael. This is a payment obligation only — it is <strong>not</strong> reduced by what that player later wins.</p>
    <div class="table-scroll">
      <table id="buyinTable">
        <thead><tr><th>Player</th><th class="num">Day 1</th><th class="num">Day 2</th><th class="num">Pay Organizer</th><th>Status</th></tr></thead>
        <tbody></tbody>
      </table>
    </div>
  </section>

  <!-- HORSE PAYOUTS -->
  <section id="payoutSection">
    <div class="section-head"><h2>Horse Payouts — Organizer Pays Players</h2></div>
    <p class="section-note">The full gross payout Michael sends each player, based on horses won. This uses the payout figures, not the spreadsheet's net winnings.</p>
    <div class="table-scroll">
      <table id="payoutTable">
        <thead><tr><th>Player</th><th class="num">Day 1</th><th class="num">Day 2</th><th class="num">Organizer Pays</th><th>Status</th></tr></thead>
        <tbody></tbody>
      </table>
    </div>
  </section>

  <!-- INDIVIDUAL SETTLEMENT -->
  <section id="settleSection">
    <div class="section-head"><h2>Individual Settlement Cards</h2></div>
    <p class="section-note">Both directions of money for each player, shown separately and never combined into one net payment. The net line below is informational only.</p>
    <div class="settle-grid" id="settleGrid"></div>
    <div class="empty-state" id="settleEmpty" hidden>No players match your search or filter.</div>
  </section>

  <footer class="page-footer">
    <span>Georgia Trip · June 2026 · Organizer: Michael</span>
    <span>Source: Georgia Money.xlsx — actual shared costs $2,204.25</span>
  </footer>
</div>

<script>
(function(){
  "use strict";

  /* ---------------- DATA (amounts stored as integer cents) ---------------- */
  const sharedExpenses = [
    { category: "Boat Gas", cents: 4065 },
    { category: "Boat Rental", cents: 57860 },
    { category: "Groceries", cents: 48500 },
    { category: "Cleaning", cents: 50000 },
    { category: "Steaks and Burgers", cents: 60000 }
  ];
  const ACTUAL_SHARED_COST_CENTS = sharedExpenses.reduce((s,e)=>s+e.cents,0); // 220425

  // Editable: couple names — spreadsheet doesn't identify pairings
  const couples = [
    { id: "couple1", name: "Michael & Alyson", dueCents: 36800, note: "" },
    { id: "couple2", name: "Cole & Whit", dueCents: 36800, note: "" },
    { id: "couple3", name: "Terence & Shannon", dueCents: 36800, note: "" },
    { id: "couple4", name: "Cren & Maggie", dueCents: 36800, note: "" },
    { id: "couple5", name: "Tanner & Ille", dueCents: 36800, note: "" },
    { id: "couple6", name: "Justin & Haley", dueCents: 36800, note: "" }
  ];
  const COUPLE_COLLECTED_CENTS = couples.reduce((s,c)=>s+c.dueCents,0); // 220800
  const ROUNDING_DIFF_CENTS = COUPLE_COLLECTED_CENTS - ACTUAL_SHARED_COST_CENTS; // 375

  const horseBuyIns = [
    { id:"whit", name:"Whit", day1:1600, day2:1600, totalCents:3200 },
    { id:"cole", name:"Cole", day1:1750, day2:1650, totalCents:3400 },
    { id:"michael", name:"Michael", day1:1250, day2:1250, totalCents:2500 },
    { id:"terence", name:"Terence", day1:1500, day2:1700, totalCents:3200 },
    { id:"tanner", name:"Tanner", day1:1100, day2:900, totalCents:2000 },
    { id:"ille", name:"Ille", day1:1250, day2:0, totalCents:1250 },
    { id:"haley", name:"Haley", day1:2000, day2:1750, totalCents:3750 },
    { id:"justin", name:"Justin", day1:1700, day2:1700, totalCents:3400 },
    { id:"maggie", name:"Maggie", day1:1250, day2:950, totalCents:2200 },
    { id:"cren", name:"Cren", day1:2100, day2:1450, totalCents:3550 },
    { id:"alyson", name:"Alyson", day1:0, day2:1200, totalCents:1200 },
    { id:"shannon", name:"Shannon", day1:0, day2:1900, totalCents:1900 }
  ];
  const BUYIN_CONTROL_TOTAL_CENTS = 31550;

  const horsePayouts = [
    { id:"whit", name:"Whit", day1:900, day2:2310, totalCents:3210 },
    { id:"cole", name:"Cole", day1:2150, day2:2470, totalCents:4620 },
    { id:"michael", name:"Michael", day1:1110, day2:940, totalCents:2050 },
    { id:"terence", name:"Terence", day1:1300, day2:1000, totalCents:2300 },
    { id:"tanner", name:"Tanner", day1:1250, day2:600, totalCents:1850 },
    { id:"ille", name:"Ille", day1:830, day2:0, totalCents:830 },
    { id:"haley", name:"Haley", day1:3330, day2:2650, totalCents:5980 },
    { id:"justin", name:"Justin", day1:1700, day2:0, totalCents:1700 },
    { id:"maggie", name:"Maggie", day1:1310, day2:990, totalCents:2300 },
    { id:"cren", name:"Cren", day1:1620, day2:1580, totalCents:3200 },
    { id:"alyson", name:"Alyson", day1:0, day2:1740, totalCents:1740 },
    { id:"shannon", name:"Shannon", day1:0, day2:1770, totalCents:1770 }
  ];
  const PAYOUT_CONTROL_TOTAL_CENTS = 31550;

  /* ---------------- Validation against control totals ---------------- */
  (function validate(){
    const buyinSum = horseBuyIns.reduce((s,p)=>s+p.totalCents,0);
    const payoutSum = horsePayouts.reduce((s,p)=>s+p.totalCents,0);
    if (buyinSum !== BUYIN_CONTROL_TOTAL_CENTS) console.warn("Buy-in total mismatch:", buyinSum);
    if (payoutSum !== PAYOUT_CONTROL_TOTAL_CENTS) console.warn("Payout total mismatch:", payoutSum);
  })();

  /* ---------------- Formatting helpers ---------------- */
  const currencyFmt = new Intl.NumberFormat("en-US", { style: "currency", currency: "USD" });
  function fmt(cents){ return currencyFmt.format(cents / 100); }

  /* ---------------- Persisted status (localStorage) ---------------- */
  const STORAGE_KEY = "gaTrip2026_paymentStatus";
  let statusMap = {};
  try{ statusMap = JSON.parse(localStorage.getItem(STORAGE_KEY)) || {}; } catch(e){ statusMap = {}; }

  function getStatus(key){ return statusMap[key] === "paid" ? "paid" : "unpaid"; }
  function setStatus(key, val){
    statusMap[key] = val;
    try{ localStorage.setItem(STORAGE_KEY, JSON.stringify(statusMap)); } catch(e){ /* storage unavailable */ }
  }
  function toggleStatus(key){
    setStatus(key, getStatus(key) === "paid" ? "unpaid" : "paid");
  }

  /* ---------------- Render: Summary Cards ---------------- */
  function renderSummary(){
    const el = document.getElementById("summaryGrid");
    el.innerHTML = `
      <div class="sum-card">
        <span class="label">Shared Trip Costs</span>
        <span class="amount num">${fmt(ACTUAL_SHARED_COST_CENTS)}</span>
        <span class="dir neutral">Actual spend</span>
      </div>
      <div class="sum-card">
        <span class="label">Cost per Couple</span>
        <span class="amount num">${fmt(36800)}</span>
        <span class="dir to-organizer">Pay Organizer</span>
      </div>
      <div class="sum-card">
        <span class="label">Horse Buy‑Ins Due</span>
        <span class="amount num">${fmt(BUYIN_CONTROL_TOTAL_CENTS)}</span>
        <span class="dir to-organizer">Pay Organizer</span>
      </div>
      <div class="sum-card">
        <span class="label">Horse Payouts Due</span>
        <span class="amount num">${fmt(PAYOUT_CONTROL_TOTAL_CENTS)}</span>
        <span class="dir from-organizer">Organizer Pays</span>
      </div>`;
  }

  /* ---------------- Render: Couple cards ---------------- */
  function matchesSearch(name, query){
    return !query || name.toLowerCase().includes(query.toLowerCase());
  }

  function coupleBucket(status){
    return status === "paid" ? "completed" : "toOrganizer";
  }

  function renderCouples(query, filter){
    const grid = document.getElementById("coupleGrid");
    grid.innerHTML = "";
    let visibleCount = 0;
    couples.forEach(c=>{
      const status = getStatus(c.id);
      const bucket = coupleBucket(status);
      const visible = matchesSearch(c.name, query) && (filter === "all" || filter === bucket);
      if (!visible) return;
      visibleCount++;
      const card = document.createElement("div");
      card.className = "couple-card";
      card.innerHTML = `
        <div class="row-top">
          <span class="name">${c.name}</span>
          <span class="due num">${fmt(c.dueCents)}</span>
        </div>
        <div class="toggle-row">
          <span style="font-size:12.5px;color:var(--ink-soft);">Due to organizer</span>
          <button class="status-toggle" data-status="${status}" data-id="${c.id}" data-kind="couple"
            aria-pressed="${status === 'paid'}">
            ${status === "paid" ? "✓ Paid" : "Unpaid"}
          </button>
        </div>
        <input class="note-input" type="text" placeholder="Payment method / note (optional)"
          data-note-id="${c.id}" value="${c.note ? c.note.replace(/"/g,'&quot;') : ''}">
      `;
      grid.appendChild(card);
    });
    document.getElementById("coupleSection").style.display = visibleCount === 0 && (query || filter !== "all") ? "none" : "";
  }

  /* ---------------- Render: Buy-in / Payout tables ---------------- */
  function renderTable(tbodyEl, data, kind, directionBucket, query, filter){
    tbodyEl.innerHTML = "";
    let anyVisible = false;
    data.forEach(p=>{
      const statusKey = kind + "_" + p.id;
      const status = getStatus(statusKey);
      const bucket = status === "paid" ? "completed" : directionBucket;
      const visible = matchesSearch(p.name, query) && (filter === "all" || filter === bucket);
      if (!visible) return;
      anyVisible = true;
      const tr = document.createElement("tr");
      tr.innerHTML = `
        <td data-label="Player">${p.name}</td>
        <td class="num" data-label="Day 1">${fmt(p.day1)}</td>
        <td class="num" data-label="Day 2">${fmt(p.day2)}</td>
        <td class="num" data-label="${kind === 'buyin' ? 'Pay Organizer' : 'Organizer Pays'}"><strong>${fmt(p.totalCents)}</strong></td>
        <td data-label="Status">
          <button class="status-pill" data-status="${status}" data-id="${p.id}" data-kind="${kind}" aria-pressed="${status === 'paid'}">
            ${status === "paid" ? "✓ Paid" : "Unpaid"}
          </button>
        </td>`;
      tbodyEl.appendChild(tr);
    });
    // Total row (always shown when not actively filtered to empty and not searching)
    if (!query){
      const totalCents = data.reduce((s,p)=>s+p.totalCents,0);
      const day1Total = data.reduce((s,p)=>s+p.day1,0);
      const day2Total = data.reduce((s,p)=>s+p.day2,0);
      const tr = document.createElement("tr");
      tr.className = "total-row";
      tr.innerHTML = `
        <td data-label="Player">TOTAL</td>
        <td class="num" data-label="Day 1">${fmt(day1Total)}</td>
        <td class="num" data-label="Day 2">${fmt(day2Total)}</td>
        <td class="num" data-label="${kind === 'buyin' ? 'Pay Organizer' : 'Organizer Pays'}">${fmt(totalCents)}</td>
        <td data-label="Status">—</td>`;
      tbodyEl.appendChild(tr);
    }
    return anyVisible;
  }

  /* ---------------- Render: Settlement cards ---------------- */
  function playerSettleBucket(id){
    const buyinPaid = getStatus("buyin_" + id) === "paid";
    const payoutPaid = getStatus("payout_" + id) === "paid";
    if (buyinPaid && payoutPaid) return "completed";
    // If buy-in still owed, player needs to pay organizer; if payout still owed, organizer needs to pay
    if (!buyinPaid) return "toOrganizer";
    return "fromOrganizer";
  }

  function renderSettlement(query, filter){
    const grid = document.getElementById("settleGrid");
    grid.innerHTML = "";
    let visibleCount = 0;
    horseBuyIns.forEach(buyin=>{
      const payout = horsePayouts.find(p=>p.id === buyin.id);
      const bucket = playerSettleBucket(buyin.id);
      const visible = matchesSearch(buyin.name, query) && (filter === "all" || filter === bucket);
      if (!visible) return;
      visibleCount++;
      const netCents = payout.totalCents - buyin.totalCents;
      const netLabel = netCents >= 0 ? `+${fmt(netCents)}` : `-${fmt(Math.abs(netCents))}`;
      const buyinStatus = getStatus("buyin_" + buyin.id);
      const payoutStatus = getStatus("payout_" + buyin.id);

      const card = document.createElement("div");
      card.className = "ticket";
      card.innerHTML = `
        <div class="ticket-head">
          <span class="p-name">${buyin.name}</span>
          <span class="badge" style="font-size:11px;color:var(--ink-soft);">Georgia · June '26</span>
        </div>
        <div class="perf" aria-hidden="true"></div>
        <div class="ticket-body">
          <div class="flow-line out">
            <span class="label">
              <svg width="14" height="14" viewBox="0 0 24 24" fill="none"><path d="M5 12h14M13 6l6 6-6 6" stroke="#BD5B2A" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>
              You send Michael
            </span>
            <span class="amt num">${fmt(buyin.totalCents)}</span>
          </div>
          <div class="flow-line in">
            <span class="label">
              <svg width="14" height="14" viewBox="0 0 24 24" fill="none"><path d="M19 12H5m6 6l-6-6 6-6" stroke="#2E7A62" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>
              Michael sends you
            </span>
            <span class="amt num">${fmt(payout.totalCents)}</span>
          </div>
          <div class="net-line">
            <span>Net game result<span class="ref-tag">For reference only</span></span>
            <span class="num">${netLabel}</span>
          </div>
        </div>
        <div class="ticket-actions no-print">
          <button class="ghost-btn" data-id="${buyin.id}" data-kind="buyin" data-toggle-status="${buyinStatus}">
            ${buyinStatus === "paid" ? "✓ Buy‑in paid" : "Mark buy‑in paid"}
          </button>
          <button class="ghost-btn" data-id="${buyin.id}" data-kind="payout" data-toggle-status="${payoutStatus}">
            ${payoutStatus === "paid" ? "✓ Payout received" : "Mark payout paid"}
          </button>
        </div>
        <div class="ticket-actions no-print" style="padding-top:0;">
          <button class="ghost-btn copy-btn" data-id="${buyin.id}">
            <svg width="13" height="13" viewBox="0 0 24 24" fill="none"><rect x="9" y="9" width="11" height="11" rx="1.5" stroke="currentColor" stroke-width="1.6"/><path d="M5 15V5a1 1 0 011-1h10" stroke="currentColor" stroke-width="1.6"/></svg>
            Copy Payment Summary
          </button>
        </div>
      `;
      grid.appendChild(card);
    });
    document.getElementById("settleEmpty").hidden = visibleCount !== 0;
  }

  /* ---------------- Copy summary text ---------------- */
  function copySummary(playerId){
    const buyin = horseBuyIns.find(p=>p.id === playerId);
    const payout = horsePayouts.find(p=>p.id === playerId);
    const netCents = payout.totalCents - buyin.totalCents;
    const netLabel = netCents >= 0 ? `+${fmt(netCents)}` : `-${fmt(Math.abs(netCents))}`;
    const text =
`June 2026 Georgia Trip — Settlement for ${buyin.name}
You send Michael: ${fmt(buyin.totalCents)} (horse buy-ins)
Michael sends you: ${fmt(payout.totalCents)} (horse payouts)
Net game result (for reference only, not a payment amount): ${netLabel}`;
    if (navigator.clipboard && navigator.clipboard.writeText){
      navigator.clipboard.writeText(text).catch(()=>fallbackCopy(text));
    } else {
      fallbackCopy(text);
    }
  }
  function fallbackCopy(text){
    const ta = document.createElement("textarea");
    ta.value = text; ta.style.position = "fixed"; ta.style.left = "-9999px";
    document.body.appendChild(ta); ta.select();
    try{ document.execCommand("copy"); } catch(e){}
    document.body.removeChild(ta);
  }

  /* ---------------- Master render ---------------- */
  let currentFilter = "all";
  let currentQuery = "";

  function renderAll(){
    renderSummary();
    renderCouples(currentQuery, currentFilter);

    const buyinTbody = document.querySelector("#buyinTable tbody");
    const buyinVisible = renderTable(buyinTbody, horseBuyIns, "buyin", "toOrganizer", currentQuery, currentFilter);
    document.getElementById("buyinSection").style.display = (!buyinVisible && (currentQuery || currentFilter !== "all")) ? "none" : "";

    const payoutTbody = document.querySelector("#payoutTable tbody");
    const payoutVisible = renderTable(payoutTbody, horsePayouts, "payout", "fromOrganizer", currentQuery, currentFilter);
    document.getElementById("payoutSection").style.display = (!payoutVisible && (currentQuery || currentFilter !== "all")) ? "none" : "";

    renderSettlement(currentQuery, currentFilter);

    document.getElementById("coupleFooterTotal").textContent = fmt(COUPLE_COLLECTED_CENTS);
  }

  /* ---------------- Event delegation ---------------- */
  document.addEventListener("click", function(e){
    const toggle = e.target.closest("[data-kind][data-id]");
    if (toggle && (toggle.classList.contains("status-toggle") || toggle.classList.contains("status-pill") || toggle.classList.contains("ghost-btn")) && !toggle.classList.contains("copy-btn")){
      const kind = toggle.dataset.kind;
      const id = toggle.dataset.id;
      const key = kind === "couple" ? id : (kind + "_" + id);
      toggleStatus(key);
      renderAll();
      return;
    }
    const copyBtn = e.target.closest(".copy-btn");
    if (copyBtn){
      copySummary(copyBtn.dataset.id);
      copyBtn.classList.add("copied");
      copyBtn.innerHTML = "✓ Copied to clipboard";
      setTimeout(()=>{ renderAll(); }, 1400);
    }
  });

  document.addEventListener("input", function(e){
    if (e.target.id === "searchInput"){
      currentQuery = e.target.value.trim();
      renderAll();
    }
    if (e.target.dataset && e.target.dataset.noteId){
      const c = couples.find(c=>c.id === e.target.dataset.noteId);
      if (c) c.note = e.target.value;
    }
  });

  document.querySelectorAll(".filter-btn").forEach(btn=>{
    btn.addEventListener("click", function(){
      document.querySelectorAll(".filter-btn").forEach(b=>b.classList.remove("active"));
      btn.classList.add("active");
      currentFilter = btn.dataset.filter;
      renderAll();
    });
  });

  document.getElementById("printBtn").addEventListener("click", function(){ window.print(); });

  renderAll();
})();
</script>
</body>
</html>
