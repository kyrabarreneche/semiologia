[Uploading Apendicite_Aguda_KyraBarreneche.html…]()
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Apendicite Aguda — Kyra Barreneche</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;600;700;900&family=IBM+Plex+Sans:wght@300;400;500;600&family=IBM+Plex+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
  :root {
    --bg: #1a0d10;
    --surface: #271118;
    --surface2: #33151d;
    --surface3: #3d1a22;
    --rose-deep: #c2566e;
    --rose-mid: #e07b95;
    --rose-light: #f0a8b8;
    --rose-pale: #fce8ed;
    --rose-blush: #fdf3f5;
    --rose-mist: #fff7f9;
    --gold: #e8c9a0;
    --text-primary: #fdf0f2;
    --text-secondary: #d4a0ac;
    --text-muted: #a07080;
    --border: rgba(224, 123, 149, 0.18);
    --border-strong: rgba(224, 123, 149, 0.35);
    --shadow: 0 4px 24px rgba(0,0,0,0.5);
    --radius: 12px;
    --radius-sm: 8px;
  }

  * { margin: 0; padding: 0; box-sizing: border-box; }

  html { scroll-behavior: smooth; }

  body {
    background: var(--bg);
    color: var(--text-primary);
    font-family: 'IBM Plex Sans', sans-serif;
    line-height: 1.7;
    font-size: 15px;
  }

  /* PROGRESS BAR */
  #progress-bar {
    position: fixed;
    top: 0; left: 0;
    height: 3px;
    background: linear-gradient(90deg, var(--rose-deep), var(--rose-light));
    z-index: 9999;
    transition: width 0.1s linear;
    width: 0%;
  }

  /* NAVBAR */
  nav {
    position: fixed;
    top: 0; left: 0; right: 0;
    background: rgba(26, 13, 16, 0.95);
    backdrop-filter: blur(12px);
    border-bottom: 1px solid var(--border);
    z-index: 1000;
    padding: 0 2rem;
    height: 56px;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .nav-brand {
    font-family: 'Playfair Display', serif;
    font-size: 1rem;
    color: var(--rose-light);
    font-weight: 700;
    letter-spacing: 0.02em;
  }

  .nav-links {
    display: flex;
    gap: 0.1rem;
    list-style: none;
    flex-wrap: wrap;
  }

  .nav-links a {
    color: var(--text-secondary);
    text-decoration: none;
    font-size: 0.72rem;
    font-weight: 500;
    letter-spacing: 0.04em;
    text-transform: uppercase;
    padding: 0.3rem 0.6rem;
    border-radius: var(--radius-sm);
    transition: all 0.2s;
  }

  .nav-links a:hover {
    color: var(--rose-light);
    background: rgba(224, 123, 149, 0.12);
  }

  /* HERO */
  .hero {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 6rem 2rem 4rem;
    background: radial-gradient(ellipse at 50% 30%, rgba(194, 86, 110, 0.12) 0%, transparent 70%);
    position: relative;
    overflow: hidden;
  }

  .hero::before {
    content: '';
    position: absolute;
    top: 10%; left: 50%;
    transform: translateX(-50%);
    width: 600px; height: 600px;
    background: radial-gradient(circle, rgba(224, 123, 149, 0.06) 0%, transparent 70%);
    pointer-events: none;
  }

  .hero-eyebrow {
    font-family: 'IBM Plex Mono', monospace;
    font-size: 0.7rem;
    letter-spacing: 0.2em;
    text-transform: uppercase;
    color: var(--rose-mid);
    margin-bottom: 1.2rem;
    opacity: 0.9;
  }

  .hero-title {
    font-family: 'Playfair Display', serif;
    font-size: clamp(2.4rem, 6vw, 4.2rem);
    font-weight: 900;
    line-height: 1.1;
    color: var(--text-primary);
    margin-bottom: 0.6rem;
    letter-spacing: -0.01em;
  }

  .hero-title span {
    color: var(--rose-mid);
    font-style: italic;
  }

  .hero-subtitle {
    font-size: 0.95rem;
    color: var(--text-secondary);
    margin-bottom: 2.4rem;
    max-width: 520px;
    line-height: 1.6;
  }

  .author-badge {
    display: inline-flex;
    align-items: center;
    gap: 0.7rem;
    background: var(--surface2);
    border: 1px solid var(--border-strong);
    border-radius: 100px;
    padding: 0.5rem 1.2rem;
    margin-bottom: 2rem;
  }

  .author-dot {
    width: 8px; height: 8px;
    border-radius: 50%;
    background: var(--rose-mid);
    animation: pulse 2s infinite;
  }

  @keyframes pulse {
    0%, 100% { opacity: 1; transform: scale(1); }
    50% { opacity: 0.6; transform: scale(0.8); }
  }

  .author-name {
    font-family: 'IBM Plex Mono', monospace;
    font-size: 0.78rem;
    color: var(--rose-light);
    font-weight: 500;
    letter-spacing: 0.08em;
  }

  .hero-meta {
    font-family: 'IBM Plex Mono', monospace;
    font-size: 0.7rem;
    color: var(--text-muted);
    letter-spacing: 0.06em;
  }

  .scroll-cue {
    position: absolute;
    bottom: 2.5rem;
    left: 50%;
    transform: translateX(-50%);
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 0.4rem;
    color: var(--text-muted);
    font-size: 0.65rem;
    letter-spacing: 0.15em;
    text-transform: uppercase;
    animation: float 3s ease-in-out infinite;
  }

  @keyframes float {
    0%, 100% { transform: translateX(-50%) translateY(0); }
    50% { transform: translateX(-50%) translateY(-6px); }
  }

  .scroll-line {
    width: 1px;
    height: 40px;
    background: linear-gradient(to bottom, var(--rose-mid), transparent);
  }

  /* MAIN LAYOUT */
  main {
    max-width: 900px;
    margin: 0 auto;
    padding: 4rem 2rem 6rem;
  }

  /* SECTION */
  section {
    margin-bottom: 4rem;
    scroll-margin-top: 80px;
  }

  .section-header {
    display: flex;
    align-items: center;
    gap: 1rem;
    margin-bottom: 2rem;
    padding-bottom: 1rem;
    border-bottom: 1px solid var(--border);
  }

  .section-num {
    font-family: 'IBM Plex Mono', monospace;
    font-size: 0.65rem;
    color: var(--rose-mid);
    letter-spacing: 0.15em;
    background: rgba(224, 123, 149, 0.1);
    padding: 0.3rem 0.7rem;
    border-radius: 100px;
    border: 1px solid var(--border);
    white-space: nowrap;
  }

  .section-title {
    font-family: 'Playfair Display', serif;
    font-size: 1.7rem;
    font-weight: 700;
    color: var(--text-primary);
    line-height: 1.2;
  }

  .section-title em {
    color: var(--rose-mid);
    font-style: italic;
  }

  /* PROSE */
  p {
    color: var(--text-secondary);
    margin-bottom: 1rem;
    line-height: 1.8;
  }

  p strong {
    color: var(--text-primary);
    font-weight: 600;
  }

  /* CARDS */
  .card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 1.4rem 1.6rem;
    margin-bottom: 1.2rem;
    transition: border-color 0.2s, box-shadow 0.2s;
  }

  .card:hover {
    border-color: var(--border-strong);
    box-shadow: 0 2px 16px rgba(194, 86, 110, 0.08);
  }

  .card-title {
    font-family: 'IBM Plex Sans', sans-serif;
    font-size: 0.82rem;
    font-weight: 600;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    color: var(--rose-light);
    margin-bottom: 0.8rem;
    display: flex;
    align-items: center;
    gap: 0.5rem;
  }

  .card-title::before {
    content: '';
    display: inline-block;
    width: 16px; height: 2px;
    background: var(--rose-mid);
    border-radius: 2px;
  }

  /* CALLOUT BOXES */
  .callout {
    border-radius: var(--radius);
    padding: 1.2rem 1.4rem;
    margin: 1.4rem 0;
    border-left: 3px solid;
    position: relative;
  }

  .callout-fisio {
    background: rgba(194, 86, 110, 0.07);
    border-color: var(--rose-deep);
  }

  .callout-alert {
    background: rgba(232, 201, 160, 0.07);
    border-color: var(--gold);
  }

  .callout-prova {
    background: rgba(100, 180, 130, 0.07);
    border-color: #5ab87a;
  }

  .callout-label {
    font-family: 'IBM Plex Mono', monospace;
    font-size: 0.65rem;
    font-weight: 500;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    margin-bottom: 0.6rem;
    display: flex;
    align-items: center;
    gap: 0.4rem;
  }

  .callout-fisio .callout-label { color: var(--rose-mid); }
  .callout-alert .callout-label { color: var(--gold); }
  .callout-prova .callout-label { color: #5ab87a; }

  .callout p {
    margin-bottom: 0;
    font-size: 0.9rem;
  }

  /* GRID */
  .grid-2 {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 1rem;
    margin: 1.2rem 0;
  }

  /* PHASE TIMELINE */
  .phase-list {
    display: flex;
    flex-direction: column;
    gap: 0;
    position: relative;
    padding-left: 2rem;
    margin: 1.4rem 0;
  }

  .phase-list::before {
    content: '';
    position: absolute;
    left: 7px; top: 8px; bottom: 8px;
    width: 2px;
    background: linear-gradient(to bottom, var(--rose-deep), var(--surface3));
    border-radius: 2px;
  }

  .phase-item {
    position: relative;
    padding: 0.9rem 0 0.9rem 1.2rem;
    border-bottom: 1px solid var(--border);
  }

  .phase-item:last-child { border-bottom: none; }

  .phase-item::before {
    content: '';
    position: absolute;
    left: -1.7rem;
    top: 1.15rem;
    width: 10px; height: 10px;
    border-radius: 50%;
    border: 2px solid var(--rose-mid);
    background: var(--bg);
  }

  .phase-num {
    font-family: 'IBM Plex Mono', monospace;
    font-size: 0.65rem;
    color: var(--rose-mid);
    letter-spacing: 0.1em;
    margin-bottom: 0.2rem;
  }

  .phase-name {
    font-weight: 600;
    color: var(--text-primary);
    margin-bottom: 0.3rem;
    font-size: 0.95rem;
  }

  .phase-desc {
    font-size: 0.85rem;
    color: var(--text-secondary);
    line-height: 1.6;
  }

  /* SIGN TABLE */
  .sign-table {
    width: 100%;
    border-collapse: collapse;
    margin: 1.2rem 0;
    font-size: 0.88rem;
  }

  .sign-table thead tr {
    background: var(--surface2);
    border-bottom: 2px solid var(--border-strong);
  }

  .sign-table th {
    padding: 0.8rem 1rem;
    text-align: left;
    font-family: 'IBM Plex Mono', monospace;
    font-size: 0.65rem;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: var(--rose-light);
    font-weight: 500;
  }

  .sign-table td {
    padding: 0.75rem 1rem;
    border-bottom: 1px solid var(--border);
    color: var(--text-secondary);
    vertical-align: top;
  }

  .sign-table tr:last-child td { border-bottom: none; }

  .sign-table tr:hover td {
    background: rgba(224, 123, 149, 0.04);
  }

  .sign-name {
    font-weight: 600;
    color: var(--rose-light);
  }

  /* ALVARADO TABLE */
  .alvarado-table {
    width: 100%;
    border-collapse: collapse;
    margin: 1.2rem 0;
    font-size: 0.88rem;
  }

  .alvarado-table thead tr {
    background: var(--surface2);
    border-bottom: 2px solid var(--border-strong);
  }

  .alvarado-table th {
    padding: 0.7rem 0.9rem;
    text-align: left;
    font-family: 'IBM Plex Mono', monospace;
    font-size: 0.63rem;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: var(--rose-light);
    font-weight: 500;
  }

  .alvarado-table td {
    padding: 0.6rem 0.9rem;
    border-bottom: 1px solid var(--border);
    color: var(--text-secondary);
  }

  .alvarado-table tr:last-child td { border-bottom: none; }

  .pts-badge {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-width: 28px;
    height: 24px;
    background: rgba(224, 123, 149, 0.15);
    border: 1px solid var(--border);
    border-radius: 6px;
    font-family: 'IBM Plex Mono', monospace;
    font-size: 0.78rem;
    font-weight: 600;
    color: var(--rose-light);
  }

  .pts-2 {
    background: rgba(224, 123, 149, 0.25);
    border-color: var(--rose-mid);
  }

  /* INTERPRETATION METER */
  .alvarado-interp {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 0.8rem;
    margin: 1.2rem 0;
  }

  .interp-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: var(--radius-sm);
    padding: 1rem;
    text-align: center;
  }

  .interp-score {
    font-family: 'Playfair Display', serif;
    font-size: 1.6rem;
    font-weight: 700;
    display: block;
    margin-bottom: 0.3rem;
  }

  .interp-label {
    font-size: 0.75rem;
    color: var(--text-muted);
    letter-spacing: 0.05em;
  }

  .interp-action {
    font-size: 0.78rem;
    font-weight: 600;
    margin-top: 0.4rem;
    display: block;
  }

  .interp-low .interp-score { color: #5ab87a; }
  .interp-low .interp-action { color: #5ab87a; }

  .interp-mid .interp-score { color: var(--gold); }
  .interp-mid .interp-action { color: var(--gold); }

  .interp-high .interp-score { color: var(--rose-mid); }
  .interp-high .interp-action { color: var(--rose-mid); }

  /* ACCORDION */
  .accordion {
    border: 1px solid var(--border);
    border-radius: var(--radius);
    overflow: hidden;
    margin-bottom: 0.8rem;
  }

  .accordion-header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 1rem 1.3rem;
    cursor: pointer;
    background: var(--surface);
    transition: background 0.2s;
    user-select: none;
  }

  .accordion-header:hover {
    background: var(--surface2);
  }

  .accordion-title {
    font-weight: 600;
    color: var(--text-primary);
    font-size: 0.92rem;
    display: flex;
    align-items: center;
    gap: 0.6rem;
  }

  .accordion-icon {
    font-size: 0.7rem;
    color: var(--rose-mid);
    transition: transform 0.3s;
    font-family: 'IBM Plex Mono', monospace;
  }

  .accordion.open .accordion-icon {
    transform: rotate(180deg);
  }

  .accordion-body {
    display: none;
    padding: 1rem 1.3rem;
    background: var(--surface);
    border-top: 1px solid var(--border);
  }

  .accordion.open .accordion-body {
    display: block;
  }

  .accordion-body p {
    font-size: 0.88rem;
    margin-bottom: 0.6rem;
  }

  .accordion-body p:last-child { margin-bottom: 0; }

  /* REVEAL BUTTON */
  .reveal-btn {
    background: transparent;
    border: 1px solid var(--border);
    border-radius: var(--radius-sm);
    padding: 0.5rem 1rem;
    color: var(--rose-light);
    font-family: 'IBM Plex Mono', monospace;
    font-size: 0.72rem;
    letter-spacing: 0.08em;
    cursor: pointer;
    transition: all 0.2s;
    display: inline-flex;
    align-items: center;
    gap: 0.4rem;
    margin-top: 0.6rem;
  }

  .reveal-btn:hover {
    background: rgba(224, 123, 149, 0.1);
    border-color: var(--rose-mid);
  }

  .reveal-content {
    display: none;
    margin-top: 0.8rem;
    padding: 1rem;
    background: rgba(224, 123, 149, 0.06);
    border-radius: var(--radius-sm);
    border: 1px solid var(--border);
    font-size: 0.88rem;
    color: var(--text-secondary);
    animation: fadeIn 0.3s ease;
  }

  .reveal-content.shown { display: block; }

  @keyframes fadeIn {
    from { opacity: 0; transform: translateY(-6px); }
    to { opacity: 1; transform: translateY(0); }
  }

  /* TAGS */
  .tag {
    display: inline-block;
    background: rgba(224, 123, 149, 0.1);
    border: 1px solid var(--border);
    border-radius: 100px;
    padding: 0.2rem 0.65rem;
    font-family: 'IBM Plex Mono', monospace;
    font-size: 0.65rem;
    color: var(--rose-light);
    font-weight: 500;
    letter-spacing: 0.06em;
    text-transform: uppercase;
    margin-right: 0.3rem;
    margin-bottom: 0.3rem;
  }

  /* DIVIDER */
  .divider {
    border: none;
    border-top: 1px solid var(--border);
    margin: 2rem 0;
  }

  /* =================== SIMULADO =================== */
  #simulado {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 16px;
    padding: 2rem;
    margin-top: 2rem;
  }

  .quiz-header {
    text-align: center;
    margin-bottom: 2rem;
    padding-bottom: 1.5rem;
    border-bottom: 1px solid var(--border);
  }

  .quiz-badge {
    display: inline-block;
    background: rgba(194, 86, 110, 0.12);
    border: 1px solid var(--rose-deep);
    border-radius: 100px;
    padding: 0.3rem 0.9rem;
    font-family: 'IBM Plex Mono', monospace;
    font-size: 0.65rem;
    color: var(--rose-mid);
    letter-spacing: 0.1em;
    text-transform: uppercase;
    margin-bottom: 0.8rem;
  }

  .quiz-title {
    font-family: 'Playfair Display', serif;
    font-size: 1.5rem;
    font-weight: 700;
    color: var(--text-primary);
    margin-bottom: 0.4rem;
  }

  .quiz-desc {
    font-size: 0.85rem;
    color: var(--text-muted);
    max-width: 480px;
    margin: 0 auto;
    line-height: 1.6;
  }

  .question-card {
    background: var(--surface2);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 1.6rem;
    margin-bottom: 1.4rem;
    transition: border-color 0.2s;
  }

  .question-card.answered {
    border-color: var(--border-strong);
  }

  .q-header {
    display: flex;
    align-items: flex-start;
    gap: 1rem;
    margin-bottom: 1rem;
  }

  .q-num {
    flex-shrink: 0;
    width: 32px; height: 32px;
    border-radius: 8px;
    background: rgba(224, 123, 149, 0.12);
    border: 1px solid var(--border);
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: 'IBM Plex Mono', monospace;
    font-size: 0.78rem;
    font-weight: 600;
    color: var(--rose-mid);
  }

  .q-stem {
    font-size: 0.9rem;
    color: var(--text-primary);
    line-height: 1.7;
    font-weight: 500;
  }

  .q-case {
    background: rgba(0,0,0,0.25);
    border-left: 2px solid var(--rose-deep);
    border-radius: 0 var(--radius-sm) var(--radius-sm) 0;
    padding: 0.8rem 1rem;
    margin-bottom: 1rem;
    font-size: 0.85rem;
    color: var(--text-secondary);
    line-height: 1.7;
    font-style: italic;
  }

  .q-question {
    font-size: 0.9rem;
    font-weight: 600;
    color: var(--text-primary);
    margin-bottom: 1rem;
  }

  .options {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
    margin-bottom: 1rem;
  }

  .option {
    display: flex;
    align-items: flex-start;
    gap: 0.8rem;
    padding: 0.75rem 1rem;
    border: 1px solid var(--border);
    border-radius: var(--radius-sm);
    cursor: pointer;
    transition: all 0.2s;
    background: var(--surface);
  }

  .option:hover {
    border-color: var(--rose-mid);
    background: rgba(224, 123, 149, 0.05);
  }

  .option.selected {
    border-color: var(--rose-mid);
    background: rgba(224, 123, 149, 0.08);
  }

  .option.correct {
    border-color: #5ab87a;
    background: rgba(90, 184, 122, 0.08);
  }

  .option.wrong {
    border-color: #d95f6e;
    background: rgba(217, 95, 110, 0.08);
  }

  .option-letter {
    flex-shrink: 0;
    width: 22px; height: 22px;
    border-radius: 5px;
    background: var(--surface3);
    border: 1px solid var(--border);
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: 'IBM Plex Mono', monospace;
    font-size: 0.68rem;
    font-weight: 600;
    color: var(--text-muted);
    transition: all 0.2s;
  }

  .option.selected .option-letter { color: var(--rose-light); border-color: var(--rose-mid); }
  .option.correct .option-letter { color: #5ab87a; border-color: #5ab87a; background: rgba(90, 184, 122, 0.15); }
  .option.wrong .option-letter { color: #d95f6e; border-color: #d95f6e; background: rgba(217, 95, 110, 0.15); }

  .option-text {
    font-size: 0.87rem;
    color: var(--text-secondary);
    line-height: 1.6;
    padding-top: 0.05rem;
  }

  .confirm-btn {
    background: var(--rose-deep);
    border: none;
    border-radius: var(--radius-sm);
    padding: 0.6rem 1.3rem;
    color: white;
    font-family: 'IBM Plex Sans', sans-serif;
    font-size: 0.82rem;
    font-weight: 600;
    cursor: pointer;
    transition: all 0.2s;
    letter-spacing: 0.03em;
  }

  .confirm-btn:hover {
    background: var(--rose-mid);
    transform: translateY(-1px);
  }

  .confirm-btn:disabled {
    background: var(--surface3);
    color: var(--text-muted);
    cursor: not-allowed;
    transform: none;
  }

  .feedback-box {
    display: none;
    margin-top: 1rem;
    padding: 1rem 1.2rem;
    border-radius: var(--radius-sm);
    font-size: 0.86rem;
    line-height: 1.7;
    animation: fadeIn 0.3s ease;
  }

  .feedback-box.correct-fb {
    display: block;
    background: rgba(90, 184, 122, 0.08);
    border: 1px solid rgba(90, 184, 122, 0.3);
    color: #a8e0ba;
  }

  .feedback-box.wrong-fb {
    display: block;
    background: rgba(217, 95, 110, 0.08);
    border: 1px solid rgba(217, 95, 110, 0.3);
    color: #f0a0a8;
  }

  .feedback-label {
    font-weight: 700;
    margin-bottom: 0.4rem;
    font-family: 'IBM Plex Mono', monospace;
    font-size: 0.7rem;
    letter-spacing: 0.1em;
    text-transform: uppercase;
  }

  .correct-fb .feedback-label { color: #5ab87a; }
  .wrong-fb .feedback-label { color: #d95f6e; }

  /* SCORE PANEL */
  #score-panel {
    display: none;
    background: var(--surface2);
    border: 1px solid var(--border-strong);
    border-radius: var(--radius);
    padding: 2rem;
    text-align: center;
    margin-top: 2rem;
    animation: fadeIn 0.5s ease;
  }

  .score-num {
    font-family: 'Playfair Display', serif;
    font-size: 3.5rem;
    font-weight: 900;
    color: var(--rose-light);
    display: block;
    margin-bottom: 0.3rem;
  }

  .score-label {
    color: var(--text-muted);
    font-size: 0.85rem;
    margin-bottom: 1rem;
  }

  .score-msg {
    font-size: 0.92rem;
    color: var(--text-secondary);
    max-width: 400px;
    margin: 0 auto 1.5rem;
    line-height: 1.6;
  }

  .reset-btn {
    background: transparent;
    border: 1px solid var(--border-strong);
    border-radius: var(--radius-sm);
    padding: 0.6rem 1.4rem;
    color: var(--rose-light);
    font-family: 'IBM Plex Sans', sans-serif;
    font-size: 0.82rem;
    cursor: pointer;
    transition: all 0.2s;
    font-weight: 500;
  }

  .reset-btn:hover {
    background: rgba(224, 123, 149, 0.1);
    border-color: var(--rose-mid);
  }

  /* FOOTER */
  footer {
    border-top: 1px solid var(--border);
    padding: 2.5rem 2rem;
    text-align: center;
    color: var(--text-muted);
    font-size: 0.78rem;
    max-width: 900px;
    margin: 0 auto;
  }

  footer .footer-name {
    color: var(--rose-light);
    font-family: 'Playfair Display', serif;
    font-size: 0.95rem;
    font-weight: 600;
    display: block;
    margin-bottom: 0.3rem;
  }

  /* UTILITY */
  ul, ol { padding-left: 1.4rem; color: var(--text-secondary); }
  li { margin-bottom: 0.4rem; font-size: 0.9rem; line-height: 1.7; }
  li strong { color: var(--text-primary); }

  .highlight { color: var(--rose-light); font-weight: 600; }
  .mono { font-family: 'IBM Plex Mono', monospace; }

  @media (max-width: 640px) {
    .nav-links { display: none; }
    .alvarado-interp { grid-template-columns: 1fr; }
    main { padding: 3rem 1.2rem 5rem; }
  }
</style>
</head>
<body>
<div id="progress-bar"></div>

<nav>
  <span class="nav-brand">Apendicite Aguda</span>
  <ul class="nav-links">
    <li><a href="#fisiopatologia">Fisiopatologia</a></li>
    <li><a href="#quadro-clinico">Quadro Clínico</a></li>
    <li><a href="#semiologia">Semiologia</a></li>
    <li><a href="#diagnostico">Diagnóstico</a></li>
    <li><a href="#classificacao">Classificação</a></li>
    <li><a href="#manejo">Manejo</a></li>
    <li><a href="#diferenciais">Diferenciais</a></li>
    <li><a href="#simulado">Simulado</a></li>
  </ul>
</nav>

<!-- HERO -->
<div class="hero">
  <p class="hero-eyebrow">Semiologia I · CENSUPEG · 2026</p>
  <h1 class="hero-title">Apendicite <span>Aguda</span></h1>
  <p class="hero-subtitle">Fisiopatologia, quadro clínico, semiologia, diagnóstico e simulado — construído sob a ótica do raciocínio clínico integrado.</p>
  <div class="author-badge">
    <div class="author-dot"></div>
    <span class="author-name">Kyra Barreneche</span>
  </div>
  <p class="hero-meta">Prof. Dr. João Vitor Galo Esteves · Faculdade CENSUPEG</p>
  <div class="scroll-cue">
    <span>Role para explorar</span>
    <div class="scroll-line"></div>
  </div>
</div>

<main>

<!-- ============================================================ -->
<!-- SEÇÃO 1: FISIOPATOLOGIA -->
<!-- ============================================================ -->
<section id="fisiopatologia">
  <div class="section-header">
    <span class="section-num">01</span>
    <h2 class="section-title">Fisiopatologia — <em>o mecanismo que origina tudo</em></h2>
  </div>

  <p>O apêndice cecal é um órgão tubular localizado na confluência das três tênias cólicas do ceco. A apendicite é um <strong>abdome agudo inflamatório</strong> — a causa mais comum de intervenção cirúrgica de urgência e o paradigma do raciocínio em abdome agudo.</p>

  <div class="callout callout-fisio">
    <div class="callout-label">⬡ Mecanismo central</div>
    <p><strong>Obstrução do lúmen apendicular → alça fechada → sobredistensão → isquemia → necrose → perfuração.</strong> A causa mais frequente de obstrução é o <strong>fecalito</strong> (coprolito calcificado). Outras causas: hiperplasia linfoide, parasitas, corpos estranhos, neoplasias.</p>
  </div>

  <div class="card">
    <div class="card-title">Cascata fisiopatológica detalhada</div>
    <div class="phase-list">
      <div class="phase-item">
        <div class="phase-num">ETAPA 01</div>
        <div class="phase-name">Obstrução luminal</div>
        <div class="phase-desc">O fecalito obstrui o lúmen do apêndice criando um "sistema de alça fechada": secreções continuam sendo produzidas sem via de saída, gerando acúmulo intraluminal progressivo.</div>
      </div>
      <div class="phase-item">
        <div class="phase-num">ETAPA 02</div>
        <div class="phase-name">Sobredistensão e estimulação visceral</div>
        <div class="phase-desc">A distensão estimula fibras aferentes viscerais (T8–T10), gerando <strong>dor visceral difusa, periumbilical/epigástrica</strong>, mal localizada — a dor inicial da apendicite. A pressão intraluminal aumenta gradualmente.</div>
      </div>
      <div class="phase-item">
        <div class="phase-num">ETAPA 03</div>
        <div class="phase-name">Inflamação transmural e invasão bacteriana</div>
        <div class="phase-desc">Com a sobredistensão, a parede do apêndice espessa, edemaciada e hipóxica permite translocação bacteriana. Instala-se inflamação transmural com exsudato fibrino-purulento.</div>
      </div>
      <div class="phase-item">
        <div class="phase-num">ETAPA 04</div>
        <div class="phase-name">Periviricite e dor parietal</div>
        <div class="phase-desc">A inflamação atinge a serosa (periviricite da ponta). O peritônio parietal adjacente é irritado, ativando fibras somáticas (dor bem localizada, em pontada, <strong>migra para FID</strong>). É aqui que surgem os sinais de peritonite.</div>
      </div>
      <div class="phase-item">
        <div class="phase-num">ETAPA 05</div>
        <div class="phase-name">Isquemia, gangrena e perfuração</div>
        <div class="phase-desc">Pressão intraluminal superior à pressão de perfusão venosa → isquemia mural → necrose (gangrena) → perfuração. A perfuração libera conteúdo séptico na cavidade abdominal → peritonite localizada ou difusa.</div>
      </div>
    </div>
  </div>

  <div class="callout callout-prova">
    <div class="callout-label">✦ Frase de prova — Prof. Esteves</div>
    <p>A <strong>migração da dor</strong> (difusa visceral → FID parietal) não é coincidência clínica: ela é a <em>assinatura fisiopatológica</em> da apendicite. Dor que nunca migrou raramente é apendicite clássica. Dor que permaneceu apenas visceral pode indicar fase muito inicial, posição retrocecal (ausência de contato com peritônio parietal) ou outra etiologia.</p>
  </div>

  <div class="card">
    <div class="card-title">Por que surgem os sintomas sistêmicos?</div>
    <div class="accordion">
      <div class="accordion-header" onclick="toggleAccordion(this)">
        <span class="accordion-title">Náuseas, vômitos e anorexia</span>
        <span class="accordion-icon">▼</span>
      </div>
      <div class="accordion-body">
        <p>A distensão do apêndice ativa reflexos viscerais via nervo vago (X par), gerando náuseas, êmese e supressão do apetite. A anorexia precede tipicamente os vômitos, e estes raramente são profusos na apendicite — ao contrário da obstrução intestinal.</p>
      </div>
    </div>
    <div class="accordion">
      <div class="accordion-header" onclick="toggleAccordion(this)">
        <span class="accordion-title">Febre e leucocitose com desvio à esquerda</span>
        <span class="accordion-icon">▼</span>
      </div>
      <div class="accordion-body">
        <p>A invasão bacteriana e a necrose tecidual liberam citocinas pró-inflamatórias (IL-1, IL-6, TNF-α) que atuam no hipotálamo gerando febre. A medula óssea responde com aumento de produção de neutrófilos (leucocitose) e liberação de formas imaturas (desvio à esquerda). Febre geralmente leve (37,5–38,5°C) na fase não complicada — febre alta sugere perfuração ou abscesso.</p>
      </div>
    </div>
  </div>
</section>

<hr class="divider">

<!-- ============================================================ -->
<!-- SEÇÃO 2: QUADRO CLÍNICO -->
<!-- ============================================================ -->
<section id="quadro-clinico">
  <div class="section-header">
    <span class="section-num">02</span>
    <h2 class="section-title">Quadro Clínico — <em>a cronologia que ninguém pode ignorar</em></h2>
  </div>

  <div class="callout callout-alert">
    <div class="callout-label">⚠ Sequência clássica — memorize a ordem</div>
    <p><strong>1° Anorexia</strong> → <strong>2° Dor visceral periumbilical</strong> → <strong>3° Náuseas/vômitos</strong> → <strong>4° Migração da dor para FID</strong> (dor parietal) → <strong>5° Febre e leucocitose</strong>. A inversão da ordem (ex.: vômitos antes da dor) sugere outro diagnóstico.</p>
  </div>

  <div class="grid-2">
    <div class="card">
      <div class="card-title">Fase Inicial — Dor Visceral</div>
      <ul>
        <li>Dor abdominal difusa, inespecífica, periumbilical ou epigástrica</li>
        <li>Caráter visceral: surda, em cólica, mal localizada</li>
        <li>Náuseas e anorexia acompanham</li>
        <li>Febre baixa ou ausente</li>
        <li>Leucocitose pode ser discreta</li>
      </ul>
    </div>
    <div class="card">
      <div class="card-title">Fase Avançada — Dor Parietal</div>
      <ul>
        <li><strong>Migração da dor para FID</strong> (ponto de McBurney)</li>
        <li>Caráter somático: localizada, pontada, piora ao movimento</li>
        <li>Defesa muscular localizada em FID</li>
        <li>Sinais de peritonite positivos</li>
        <li>Febre (tipicamente 37,5–38,5°C) e leucocitose significativa</li>
      </ul>
    </div>
  </div>

  <div class="card">
    <div class="card-title">Sintomas Exóticos — por variação de posição do apêndice</div>
    <p style="font-size:0.86rem; color: var(--text-muted); margin-bottom: 0.8rem;">A ponta do apêndice pode apontar para diferentes regiões, gerando inflamação por contiguidade em estruturas vizinhas. Esses sintomas NÃO excluem apendicite:</p>
    <div class="sign-table" style="overflow-x:auto;">
      <table class="sign-table">
        <thead>
          <tr>
            <th>Posição do apêndice</th>
            <th>Estrutura acometida</th>
            <th>Sintoma exótico</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Pélvico</td>
            <td>Bexiga</td>
            <td>Disúria, urgência miccional</td>
          </tr>
          <tr>
            <td>Pélvico/retrocecal</td>
            <td>Ureter</td>
            <td>Dor lombar irradiada para bolsa escrotal</td>
          </tr>
          <tr>
            <td>Voltado para íleo terminal</td>
            <td>Intestino delgado</td>
            <td>Diarreia</td>
          </tr>
          <tr>
            <td>Voltado para reto</td>
            <td>Reto</td>
            <td>Urgência evacuatória</td>
          </tr>
          <tr>
            <td>Retrocecal</td>
            <td>Psoas</td>
            <td>Sinal do psoas positivo</td>
          </tr>
        </tbody>
      </table>
    </div>
    <div class="callout callout-prova" style="margin-top:1rem; margin-bottom:0;">
      <div class="callout-label">✦ Armadilha de prova</div>
      <p>Diarreia, disúria ou dor lombar em um paciente com história iniciada no periumbilical → migração para FID não exclui apendicite; ao contrário, orienta o raciocínio para a posição do apêndice.</p>
    </div>
  </div>
</section>

<hr class="divider">

<!-- ============================================================ -->
<!-- SEÇÃO 3: SEMIOLOGIA -->
<!-- ============================================================ -->
<section id="semiologia">
  <div class="section-header">
    <span class="section-num">03</span>
    <h2 class="section-title">Semiologia — <em>os sinais e seus mecanismos</em></h2>
  </div>

  <p>Cada sinal de peritonite tem um mecanismo fisiopatológico específico. Não basta saber o que o sinal indica — é preciso saber <strong>por que ele acontece</strong>.</p>

  <div style="overflow-x:auto;">
    <table class="sign-table">
      <thead>
        <tr>
          <th>Sinal</th>
          <th>Manobra</th>
          <th>Mecanismo fisiopatológico</th>
          <th>O que sugere</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td><span class="sign-name">Blumberg</span></td>
          <td>Compressão lenta de FID + descompressão brusca</td>
          <td>A descompressão brusca provoca movimento do peritônio inflamado → irritação peritoneal aguda</td>
          <td>Peritonite parietal localizada</td>
        </tr>
        <tr>
          <td><span class="sign-name">Rovsing</span></td>
          <td>Compressão da FIE → dor em FID</td>
          <td>Compressão empurra gases do cólon esquerdo retrogradamente → distende ceco e apêndice inflamado</td>
          <td>Peritonite localizada em FID</td>
        </tr>
        <tr>
          <td><span class="sign-name">Dunphy</span></td>
          <td>Tosse → dor em FID</td>
          <td>Aumento súbito da pressão intra-abdominal → movimento do peritônio inflamado</td>
          <td>Irritação peritoneal (mesma base do Blumberg)</td>
        </tr>
        <tr>
          <td><span class="sign-name">Sinal do Obturador</span></td>
          <td>Rotação interna da coxa D com joelho fletido → dor abdominal</td>
          <td>O músculo obturador interno, ao rotacionar, pressiona o apêndice em posição pélvica inflamado</td>
          <td>Apêndice em posição pélvica</td>
        </tr>
        <tr>
          <td><span class="sign-name">Sinal do Psoas</span></td>
          <td>Hiperextensão da coxa D (paciente em DLE) → dor abdominal</td>
          <td>O psoas em estiramento pressiona o apêndice retrocecal inflamado</td>
          <td>Apêndice retrocecal</td>
        </tr>
        <tr>
          <td><span class="sign-name">Sinal de Markle / Queda sobre os calcanhares</span></td>
          <td>Paciente se eleva na ponta dos pés e deixa cair sobre os calcanhares → dor em FID</td>
          <td>Percussão indireta do peritônio parietal inflamado</td>
          <td>Irritação peritoneal (equivale a Dunphy)</td>
        </tr>
        <tr>
          <td><span class="sign-name">Lenander</span></td>
          <td>Temperatura retal maior que axilar em &gt;1°C</td>
          <td>Inflamação local do peritônio adjacente ao reto eleva temperatura retal</td>
          <td>Inflamação pélvica/peritoneal</td>
        </tr>
        <tr>
          <td><span class="sign-name">Aaron</span></td>
          <td>Palpação da FID → dor referida em epigástrio</td>
          <td>Referência de dor visceral-somática por compartilhamento de dermátomos</td>
          <td>Peritonite com componente visceral</td>
        </tr>
        <tr>
          <td><span class="sign-name">Ten Horn</span></td>
          <td>Tração do testículo ipsilateral → dor abdominal</td>
          <td>O nervo genitofemoral compartilha inervação com região apendicular via L1</td>
          <td>Irritação retroperitoneal</td>
        </tr>
      </tbody>
    </table>
  </div>

  <div class="callout callout-fisio">
    <div class="callout-label">⬡ Integração ao exame físico</div>
    <p>O exame do abdome na apendicite segue a sequência: <strong>inspeção</strong> (posição antálgica, imobilidade, abdome plano ou distendido) → <strong>ausculta</strong> (redução dos RHA na peritonite) → <strong>percussão</strong> (dor à percussão em FID) → <strong>palpação</strong> (defesa muscular voluntária/involuntária, ponto de McBurney). Na suspeita de peritonite, <strong>não realize palpação profunda intempestiva</strong> antes de mapear os sinais.</p>
  </div>

  <div class="card">
    <div class="card-title">Ponto de McBurney e sua localização</div>
    <p>O Ponto de McBurney corresponde ao <strong>terço lateral da linha que une o umbigo à espinha ilíaca ântero-superior direita</strong>. Representa a projeção cutânea da base do apêndice. A dor à palpação profunda neste ponto é o achado semiótico central da apendicite em posição habitual.</p>
    <button class="reveal-btn" onclick="toggleReveal('rev-mcburney')">▶ Por que exatamente nesse ponto?</button>
    <div id="rev-mcburney" class="reveal-content">
      <p>A base do apêndice origina-se na confluência das três tênias cólicas no ceco. Em indivíduos adultos com anatomia usual, essa confluência projeta-se externamente no ponto de McBurney. A palpação profunda aí provoca compressão direta do apêndice inflamado contra o peritônio parietal posterior, gerando dor parietal localizada. Em posições atípicas (retrocecal, pélvica, sub-hepática), o ponto pode ser negativo mesmo com apendicite — daí a importância dos sinais complementares.</p>
    </div>
  </div>
</section>

<hr class="divider">
<!-- ============================================================ -->
<!-- SEÇÃO 4: DIAGNÓSTICO E EXAMES -->
<!-- ============================================================ -->
<section id="diagnostico">
  <div class="section-header">
    <span class="section-num">04</span>
    <h2 class="section-title">Diagnóstico e Exames — <em>clínico primeiro, imagem quando necessário</em></h2>
  </div>

  <div class="callout callout-alert">
    <div class="callout-label">⚠ Princípio fundamental</div>
    <p>Na <strong>apresentação típica</strong>, o diagnóstico é clínico — sem necessidade de exames complementares de imagem. A imagem está indicada nas situações de <strong>dúvida diagnóstica</strong> (ausência de peritonite em história típica, ou peritonite em história atípica), sobretudo em mulheres em idade fértil e idosos.</p>
  </div>

  <div class="card">
    <div class="card-title">Escore de Alvarado — estratificação objetiva</div>
    <p style="font-size:0.85rem; margin-bottom: 1rem;">O Escore de Alvarado pontua achados clínicos e laboratoriais clássicos da apendicite. É útil para orientar a necessidade de investigação complementar.</p>

    <table class="alvarado-table">
      <thead>
        <tr>
          <th>Categoria</th>
          <th>Critério</th>
          <th>Pontos</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td style="color: var(--text-muted); font-size:0.8rem;">Sintomas</td>
          <td>Migração da dor para FID</td>
          <td><span class="pts-badge">1</span></td>
        </tr>
        <tr>
          <td style="color: var(--text-muted); font-size:0.8rem;">Sintomas</td>
          <td>Anorexia</td>
          <td><span class="pts-badge">1</span></td>
        </tr>
        <tr>
          <td style="color: var(--text-muted); font-size:0.8rem;">Sintomas</td>
          <td>Náuseas ou vômitos</td>
          <td><span class="pts-badge">1</span></td>
        </tr>
        <tr>
          <td style="color: var(--text-muted); font-size:0.8rem;">Sinais</td>
          <td><strong>Defesa no quadrante inferior direito</strong></td>
          <td><span class="pts-badge pts-2">2</span></td>
        </tr>
        <tr>
          <td style="color: var(--text-muted); font-size:0.8rem;">Sinais</td>
          <td>Dor à descompressão brusca (Blumberg)</td>
          <td><span class="pts-badge">1</span></td>
        </tr>
        <tr>
          <td style="color: var(--text-muted); font-size:0.8rem;">Sinais</td>
          <td>Febre (&gt;37,3°C)</td>
          <td><span class="pts-badge">1</span></td>
        </tr>
        <tr>
          <td style="color: var(--text-muted); font-size:0.8rem;">Laboratório</td>
          <td><strong>Leucocitose (&gt;10.000)</strong></td>
          <td><span class="pts-badge pts-2">2</span></td>
        </tr>
        <tr>
          <td style="color: var(--text-muted); font-size:0.8rem;">Laboratório</td>
          <td>Desvio à esquerda</td>
          <td><span class="pts-badge">1</span></td>
        </tr>
      </tbody>
    </table>

    <div class="alvarado-interp">
      <div class="interp-card interp-low">
        <span class="interp-score">≤ 3</span>
        <span class="interp-label">Improvável</span>
        <span class="interp-action">Buscar outro diagnóstico ou reavaliação seriada</span>
      </div>
      <div class="interp-card interp-mid">
        <span class="interp-score">4 – 6</span>
        <span class="interp-label">Dúvida</span>
        <span class="interp-action">Solicitar exame de imagem (USG → TC)</span>
      </div>
      <div class="interp-card interp-high">
        <span class="interp-score">≥ 7</span>
        <span class="interp-label">Provável</span>
        <span class="interp-action">Indicação cirúrgica sem necessidade de imagem</span>
      </div>
    </div>

    <div class="callout callout-prova" style="margin-bottom:0;">
      <div class="callout-label">✦ Armadilha de prova</div>
      <p>A <strong>defesa em FID (2 pontos) e leucocitose (2 pontos)</strong> são os critérios de maior peso. Um paciente com migração da dor + anorexia + náusea + febre + leucocitose + desvio já soma <strong>7 pontos</strong> mesmo sem desvio à esquerda — cirurgia indicada.</p>
    </div>
  </div>

  <div class="card">
    <div class="card-title">Exames Laboratoriais</div>
    <div class="accordion">
      <div class="accordion-header" onclick="toggleAccordion(this)">
        <span class="accordion-title">Leucograma — o que analisar e por quê</span>
        <span class="accordion-icon">▼</span>
      </div>
      <div class="accordion-body">
        <p><strong>Leucocitose (10.000–18.000/mm³)</strong> com <strong>neutrofilia</strong> e <strong>desvio à esquerda</strong> (aumento de bastões/segmentados imaturos) reflete a resposta inflamatória aguda. A medula óssea libera neutrófilos maduros e imaturos em resposta às citocinas (IL-6, G-CSF) liberadas pelo tecido inflamado. Leucocitose isolada NÃO fecha diagnóstico — leucocitose dentro do contexto clínico, sim.</p>
        <p>Leucometria >18.000 com desvio acentuado sugere <strong>perfuração ou gangrena</strong> — apendicite complicada.</p>
      </div>
    </div>
    <div class="accordion">
      <div class="accordion-header" onclick="toggleAccordion(this)">
        <span class="accordion-title">PCR e outros marcadores inflamatórios</span>
        <span class="accordion-icon">▼</span>
      </div>
      <div class="accordion-body">
        <p>A <strong>Proteína C Reativa (PCR)</strong> eleva-se em 6–12 horas após o início da inflamação, com pico em 24–48h. Na apendicite aguda precoce, pode ser normal. Valores elevados de PCR (>10 mg/dL) em conjunto com leucocitose aumentam a especificidade diagnóstica. Tem maior utilidade nas primeiras horas quando a leucocitose ainda não está estabelecida.</p>
      </div>
    </div>
    <div class="accordion">
      <div class="accordion-header" onclick="toggleAccordion(this)">
        <span class="accordion-title">Beta-hCG — atenção obrigatória em mulheres</span>
        <span class="accordion-icon">▼</span>
      </div>
      <div class="accordion-body">
        <p>Em <strong>toda mulher em idade reprodutiva</strong> com dor em FID, o <strong>beta-hCG é obrigatório</strong> — independentemente da história menstrual relatada. A gravidez ectópica é um diagnóstico diferencial crítico que pode levar ao choque hemorrágico. Uma beta-hCG negativa não exclui gravidez muito precoce, mas afasta a ectópica como causa imediata de hemoperitônio. Essa é uma armadilha frequente nas provas do Prof. Esteves.</p>
      </div>
    </div>
  </div>

  <div class="card">
    <div class="card-title">Exames de Imagem — hierarquia diagnóstica</div>

    <div class="accordion">
      <div class="accordion-header" onclick="toggleAccordion(this)">
        <span class="accordion-title">Ultrassonografia abdominal — primeira linha</span>
        <span class="accordion-icon">▼</span>
      </div>
      <div class="accordion-body">
        <p><strong>Exame inicial de escolha</strong> na suspeita de apendicite com dúvida diagnóstica. Vantagens: sem radiação ionizante (preferível em gestantes e crianças), disponível, rápido.</p>
        <p><strong>Achados positivos (alto VPP):</strong> apêndice com diâmetro &gt;6mm, espessura parietal &gt;2mm (sinal do alvo), não compressível, borramento da gordura periapendicular, fecalito intraluminal, líquido livre pericecal.</p>
        <p><strong>Limitação crítica:</strong> <em>baixo valor preditivo negativo</em> — a não visualização do apêndice NÃO exclui apendicite. Se a USG não visualizar o apêndice ou for normal em paciente com dúvida persistente, a investigação deve prosseguir com TC.</p>
      </div>
    </div>

    <div class="accordion">
      <div class="accordion-header" onclick="toggleAccordion(this)">
        <span class="accordion-title">Tomografia computadorizada — padrão-ouro</span>
        <span class="accordion-icon">▼</span>
      </div>
      <div class="accordion-body">
        <p>Exame mais acurado (sensibilidade >94%, especificidade >95%). Achados incluem todos os da USG mais: avaliação de complicações (coleções, abscessos, pneumoperitônio), definição anatômica do apêndice mesmo em posições atípicas, diagnósticos diferenciais.</p>
        <p>Desvantagens: radiação ionizante, custo, uso de contraste IV. Deve ser usada com critério — a indicação clínica precede a decisão de irradiar. Na gestante, substituída preferencialmente pela <strong>Ressonância Magnética</strong>.</p>
      </div>
    </div>

    <div class="accordion">
      <div class="accordion-header" onclick="toggleAccordion(this)">
        <span class="accordion-title">Laparoscopia diagnóstica — quando o exame físico prevalece</span>
        <span class="accordion-icon">▼</span>
      </div>
      <div class="accordion-body">
        <p>Quando há <strong>peritonite em FID com diagnóstico incerto</strong>, a laparoscopia diagnóstica é preferível à acumulação de exames. O raciocínio: "não sei o que é, mas é de operar." A abordagem minimamente invasiva permite diagnóstico e tratamento no mesmo tempo cirúrgico. O cirurgião deve estar preparado para tratar apendicite ou seus diagnósticos diferenciais.</p>
      </div>
    </div>
  </div>

  <div class="callout callout-prova">
    <div class="callout-label">✦ Algoritmo decisório — como o Prof. Esteves cobra</div>
    <p>
      Quadro típico + Alvarado ≥7 → <strong>cirurgia direta</strong><br>
      Quadro com dúvida + Alvarado 4–6 → <strong>USG</strong> (se negativo → TC; se negativo → reavaliação seriada ou laparoscopia)<br>
      Peritonite em FID + dúvida diagnóstica → <strong>laparoscopia diagnóstica</strong><br>
      Alvarado ≤3 → <strong>reavaliação seriada, buscar diferencial</strong>
    </p>
  </div>
</section>

<hr class="divider">

<!-- ============================================================ -->
<!-- SEÇÃO 5: CLASSIFICAÇÃO -->
<!-- ============================================================ -->
<section id="classificacao">
  <div class="section-header">
    <span class="section-num">05</span>
    <h2 class="section-title">Classificação — <em>a fase determina a conduta</em></h2>
  </div>

  <p>A classificação anatomopatológica da apendicite é fundamental porque a <strong>fase da doença determina diretamente o uso e a duração do antibiótico</strong>. Esse é um dos tópicos favoritos em questões de prova.</p>

  <div class="grid-2">
    <div class="card">
      <div class="card-title">Classificação por fases evolutivas</div>
      <div class="phase-list">
        <div class="phase-item">
          <div class="phase-num">FASE 1</div>
          <div class="phase-name">Edematosa (Catarral)</div>
          <div class="phase-desc">Edema da parede, hiperemia, sem necrose. Mucosa intacta. Apendicite não complicada.</div>
        </div>
        <div class="phase-item">
          <div class="phase-num">FASE 2</div>
          <div class="phase-name">Úlcero-flegmonosa</div>
          <div class="phase-desc">Ulceração mucosa, exsudato fibrino-purulento na serosa. Inflamação transmural. Ainda não complicada.</div>
        </div>
        <div class="phase-item">
          <div class="phase-num">FASE 3</div>
          <div class="phase-name">Gangrenosa</div>
          <div class="phase-desc">Necrose mural isquêmica (gangrena). <strong>Complicada.</strong> Risco iminente de perfuração.</div>
        </div>
        <div class="phase-item">
          <div class="phase-num">FASE 4</div>
          <div class="phase-name">Perfurativa</div>
          <div class="phase-desc">Perfuração com extravasamento de conteúdo séptico. Pode gerar peritonite localizada (plastão) ou difusa. <strong>Complicada.</strong></div>
        </div>
      </div>
    </div>
    <div class="card">
      <div class="card-title">Classificação WSES 2015 (complementar)</div>
      <ul>
        <li><strong>Grau 0:</strong> Apêndice normal (achado cirúrgico)</li>
        <li><strong>Grau 1:</strong> Hiperemia e edema (fase edematosa)</li>
        <li><strong>Grau 2:</strong> Exsudato fibrinoso (flegmonosa)</li>
        <li><strong>Grau 3:</strong> Necrose segmentar com base íntegra (gangrenosa)</li>
        <li><strong>Grau 4A:</strong> Abscesso periapendicular</li>
        <li><strong>Grau 4B:</strong> Peritonite regional</li>
        <li><strong>Grau 4C:</strong> Necrose da base</li>
        <li><strong>Grau 5:</strong> Peritonite difusa</li>
      </ul>
    </div>
  </div>

  <div class="callout callout-alert">
    <div class="callout-label">⚠ Critério de complicação — que define o antibiótico</div>
    <p><strong>Não complicada = Fases 1 e 2</strong> → antibiótico profilático (até 24 horas pós-cirurgia)<br>
    <strong>Complicada = Fases 3 e 4 + abscesso cavitário</strong> → antibiótico terapêutico (7 dias)<br>
    A distinção não é clínica — é anatomopatológica (laudo cirúrgico da peça). Cobrir gram-negativos e anaeróbios: ceftriaxona + metronidazol OU amoxicilina-clavulanato OU ciprofloxacino + metronidazol.</p>
  </div>
</section>

<hr class="divider">

<!-- ============================================================ -->
<!-- SEÇÃO 6: MANEJO -->
<!-- ============================================================ -->
<section id="manejo">
  <div class="section-header">
    <span class="section-num">06</span>
    <h2 class="section-title">Manejo — <em>a decisão cirúrgica e seus cenários</em></h2>
  </div>

  <div class="card">
    <div class="card-title">Tratamento padrão</div>
    <p><strong>Apendicectomia de urgência</strong> — preferencialmente por <strong>videolaparoscopia</strong>. Segue os mesmos princípios da apendicectomia aberta: ligadura do mesoapêndice → ligadura da base → ressecção → limpeza da cavidade se necessário.</p>
    <p>Trocartes na videolaparoscopia: cicatriz umbilical, FIE e suprapúbico.</p>
  </div>

  <div class="card">
    <div class="card-title">Escolha da incisão — regra prática</div>
    <div class="accordion">
      <div class="accordion-header" onclick="toggleAccordion(this)">
        <span class="accordion-title">Apendicites iniciais e não complicadas</span>
        <span class="accordion-icon">▼</span>
      </div>
      <div class="accordion-body">
        <p>Videolaparoscopia (preferencial) ou incisões específicas locais (McBurney, Davis Rockey). Qualquer uma é igualmente efetiva nas formas não complicadas confirmadas.</p>
      </div>
    </div>
    <div class="accordion">
      <div class="accordion-header" onclick="toggleAccordion(this)">
        <span class="accordion-title">Apendicites complicadas (com secreção purulenta na cavidade)</span>
        <span class="accordion-icon">▼</span>
      </div>
      <div class="accordion-body">
        <p>Incisões específicas são <strong>contraindicadas</strong> — não permitem exploração e limpeza da cavidade. Usar videolaparoscopia ou laparotomia mediana (quando laparoscopia indisponível).</p>
      </div>
    </div>
    <div class="accordion">
      <div class="accordion-header" onclick="toggleAccordion(this)">
        <span class="accordion-title">Dúvida diagnóstica com peritonite</span>
        <span class="accordion-icon">▼</span>
      </div>
      <div class="accordion-body">
        <p>Exploração diagnóstica <strong>preferencialmente por videolaparoscopia</strong> — permite diagnóstico e tratamento no mesmo ato, com visão da cavidade completa para identificar diagnósticos diferenciais.</p>
      </div>
    </div>
  </div>

  <div class="card">
    <div class="card-title">Cenários especiais — onde as provas costumam cair</div>
    <div class="accordion">
      <div class="accordion-header" onclick="toggleAccordion(this)">
        <span class="accordion-title">Plastrão / Abscesso periapendicular (>7 dias de evolução)</span>
        <span class="accordion-icon">▼</span>
      </div>
      <div class="accordion-body">
        <p><strong>Apendicectomia em dois tempos:</strong> 1° drenagem percutânea (ou transvaginal) do abscesso + antibioticoterapia → 2° apendicectomia de intervalo após 6–8 semanas. Nesse ínterim, <strong>colonoscopia</strong> para excluir neoplasia associada.</p>
        <div class="callout callout-prova" style="margin-top:0.8rem; margin-bottom:0;">
          <div class="callout-label">✦ Armadilha de prova</div>
          <p>O plastão com abscesso periapendicular bem delimitado NÃO é tratado com cirurgia imediata de apendicectomia — o procedimento inicial é a drenagem. A apendicectomia vem depois. Essa inversão de conduta é uma armadilha clássica.</p>
        </div>
      </div>
    </div>
    <div class="accordion">
      <div class="accordion-header" onclick="toggleAccordion(this)">
        <span class="accordion-title">Apendicite em gestantes</span>
        <span class="accordion-icon">▼</span>
      </div>
      <div class="accordion-body">
        <p>A <strong>conduta não muda</strong>: tratamento cirúrgico de urgência. A cirurgia representa menos risco ao binômio materno-fetal do que a apendicite não tratada. Desafios: leucocitose fisiológica na gravidez (menos informativa), apêndice deslocado cranialmente, dores abdominais benignas confundidoras. Imagem: USG primeiro; se necessário → <strong>Ressonância Magnética</strong> (sem radiação, substitui a TC).</p>
      </div>
    </div>
    <div class="accordion">
      <div class="accordion-header" onclick="toggleAccordion(this)">
        <span class="accordion-title">Câncer pós-apendicectomia</span>
        <span class="accordion-icon">▼</span>
      </div>
      <div class="accordion-body">
        <p>Em 0,5–1% das apendicectomias, o anatomopatológico revela neoplasia. Conduta pelo tamanho e fatores de risco:</p>
        <ul>
          <li><strong>Tumor ≤1 cm, ponta/porção média, sem fatores adversos:</strong> apendicectomia foi curativa — apenas seguimento</li>
          <li><strong>Tumor entre 1–2 cm:</strong> avaliar localização (ponta = curativo; base ou mesoapêndice comprometido = hemicolectomia D)</li>
          <li><strong>Tumor >2 cm</strong> OU <strong>invasão linfovascular</strong> OU <strong>margem comprometida</strong>: <strong>hemicolectomia direita oncológica</strong></li>
        </ul>
        <p>Quimioterapia e radioterapia NÃO fazem parte do manejo padrão dos tumores carcinoides apendiculares ressecáveis.</p>
      </div>
    </div>
  </div>
</section>

<hr class="divider">

<!-- ============================================================ -->
<!-- SEÇÃO 7: DIAGNÓSTICOS DIFERENCIAIS -->
<!-- ============================================================ -->
<section id="diferenciais">
  <div class="section-header">
    <span class="section-num">07</span>
    <h2 class="section-title">Diagnósticos Diferenciais — <em>a pista no enunciado</em></h2>
  </div>

  <p>Todo quadro de dor em FID é um potencial diferencial de apendicite. O raciocínio diferencial exige ler as <strong>pistas do enunciado</strong> — epidemiológicas, cronológicas, ginecológicas e associativas.</p>

  <div style="overflow-x:auto;">
    <table class="sign-table">
      <thead>
        <tr>
          <th>Diagnóstico</th>
          <th>Pistas no enunciado</th>
          <th>Mecanismo / Diferencial-chave</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td><span class="sign-name">Linfadenite Mesentérica</span></td>
          <td>Quadro gripal 1–2 semanas antes, pré-adolescente, quadro brando</td>
          <td>Inflamação de linfonodo mesentérico por infecção viral. Doença autolimitada, tratamento de suporte. NÃO cirúrgico.</td>
        </tr>
        <tr>
          <td><span class="sign-name">Apendagite Epiploica</span></td>
          <td>Lesão ovaloide hipodensa/hipoecoica paracólica à imagem, curso benigno</td>
          <td>Inflamação e infarto de apêndice epiploico. Autolimitada. Cirurgia apenas em refratários/complicações.</td>
        </tr>
        <tr>
          <td><span class="sign-name">Febre Tifoide</span></td>
          <td>Febre alta + diarreia intensa + epidemiologia compatível (região endêmica, baixo nível socioeconômico)</td>
          <td>Infecção por Salmonella typhi. Dor em FID marcante. Tratamento: antimicrobianos.</td>
        </tr>
        <tr>
          <td><span class="sign-name">Ileíte de Crohn</span></td>
          <td>Surtos e remissões, disenteria, paciente jovem, comportamento de surto com crises repetidas</td>
          <td>Inflamação transmural do íleo distal. Tratamento clínico (imunossupressores, biológicos). Cirurgia para complicações (estenose, fístula).</td>
        </tr>
        <tr>
          <td><span class="sign-name">Ileíte Infecciosa</span></td>
          <td>Imunossupressão (SIDA, quimioterapia, linfoma, corticoides)</td>
          <td>Infecção bacteriana/viral (CMV) do íleo distal. Tratamento antibiótico/antiviral. Cirurgia para complicações.</td>
        </tr>
        <tr>
          <td><span class="sign-name">Gestação Ectópica</span></td>
          <td>Mulher em idade fértil + atraso menstrual + relação sexual desprotegida + hemoperitônio</td>
          <td>Implantação do zigoto fora do útero (tuba uterina). Beta-hCG positivo. Urgência cirúrgica se rota.</td>
        </tr>
        <tr>
          <td><span class="sign-name">Doença Inflamatória Pélvica (DIP)</span></td>
          <td>Dor hipogástrica + corrimento vaginal + relação desprotegida + febre</td>
          <td>Infecção ascendente de anexos. Tratamento clínico com antibióticos. Cirurgia para abscessos tubo-ovarianos refratários.</td>
        </tr>
      </tbody>
    </table>
  </div>

  <div class="callout callout-fisio">
    <div class="callout-label">⬡ Raciocínio diferencial integrado</div>
    <p>Em mulheres na menacme, o diferencial de dor em FID inclui além da apendicite: cistos ovarianos rotos, gestação ectópica, DIP, torção ovariana. O exame deve incluir toque vaginal, e o beta-hCG é obrigatório. Nas provas do Prof. Esteves, a ausência de investigação ginecológica em mulher com dor em FID é uma armadilha frequente.</p>
  </div>
</section>

<hr class="divider">
<!-- ============================================================ -->
<!-- SIMULADO -->
<!-- ============================================================ -->
<section id="simulado">
  <div class="section-header">
    <span class="section-num">08</span>
    <h2 class="section-title">Simulado — <em>no estilo Prof. Dr. João Vitor Esteves</em></h2>
  </div>

  <div id="simulado">
    <div class="quiz-header">
      <div class="quiz-badge">Simulado Clínico · Nível Difícil</div>
      <h3 class="quiz-title">Apendicite Aguda</h3>
      <p class="quiz-desc">Questões com casos clínicos completos e alternativas plausíveis — exigem raciocínio mecanicista, não eliminação por exclusão óbvia.</p>
    </div>

    <!-- Q1 -->
    <div class="question-card" id="qcard-1">
      <div class="q-header">
        <div class="q-num">Q1</div>
        <div class="q-stem">Uma adolescente de 16 anos, previamente hígida, é trazida ao PS às 22h com dor abdominal iniciada há 9 horas. Descreve que a dor surgiu "em volta do umbigo", acompanhada de uma náusea e hiporexia. Nas últimas 3 horas, a dor migrou e intensificou-se na fossa ilíaca direita. Ao exame: temperatura 37,8°C, FC 94 bpm, PA 112/70 mmHg. Abdome com dor à palpação profunda em FID, defesa voluntária localizada e Blumberg positivo. Sem sinais de irritação peritoneal difusa. Leucocitose de 15.200/mm³ com 82% de neutrófilos.</div>
      </div>
      <div class="q-question">Qual é a conduta mais adequada, considerando o escore de Alvarado e os achados clínicos?</div>
      <div class="options">
        <div class="option" onclick="selectOption(this, 1)" data-opt="A">
          <div class="option-letter">A</div>
          <div class="option-text">Solicitar tomografia computadorizada de abdome com contraste antes de qualquer decisão cirúrgica, pois a ausência de desvio à esquerda documentado impede calcular o escore de Alvarado corretamente.</div>
        </div>
        <div class="option" onclick="selectOption(this, 1)" data-opt="B">
          <div class="option-letter">B</div>
          <div class="option-text">Solicitar ultrassonografia abdominal imediatamente, pois em adolescentes do sexo feminino a conduta padrão exige confirmação por imagem antes de indicar cirurgia, independente do escore clínico.</div>
        </div>
        <div class="option" onclick="selectOption(this, 1)" data-opt="C">
          <div class="option-letter">C</div>
          <div class="option-text">Indicar apendicectomia videolaparoscópica de urgência, pois o escore de Alvarado ≥7 e a presença de peritonite localizada em FID dispensam a confirmação por imagem.</div>
        </div>
        <div class="option" onclick="selectOption(this, 1)" data-opt="D">
          <div class="option-letter">D</div>
          <div class="option-text">Realizar reavaliação seriada a cada 2 horas, iniciando analgesia e antibioticoterapia empírica, pois a ausência de febre alta e de peritonite difusa contraindica cirurgia imediata.</div>
        </div>
        <div class="option" onclick="selectOption(this, 1)" data-opt="E">
          <div class="option-letter">E</div>
          <div class="option-text">Solicitar beta-hCG e, após resultado negativo, indicar apendicectomia por laparotomia mediana, pois essa incisão é preferida nas apendicites em adolescentes por permitir melhor exploração da cavidade.</div>
        </div>
      </div>
      <button class="confirm-btn" onclick="confirmAnswer(1, 'C')" id="btn-1">Confirmar resposta</button>
      <div class="feedback-box" id="fb-1"></div>
    </div>

    <!-- Q2 -->
    <div class="question-card" id="qcard-2">
      <div class="q-header">
        <div class="q-num">Q2</div>
        <div class="q-stem">Um homem de 42 anos chega ao pronto-socorro com quadro de dor em FID há 9 dias, sem diagnóstico prévio. Relata piora progressiva, episódios febris (até 38,7°C) e perda de apetite. Ao exame físico: abdome com massa palpável dolorosa em FID, endurecida, de bordas imprecisas, sem peritonite difusa. Sem sinais de resposta inflamatória sistêmica grave. Leucocitose de 13.000. TC revela coleção periapendicular de 4 cm com apêndice não visualizado individualmente.</div>
      </div>
      <div class="q-question">Qual a conduta mais adequada neste momento?</div>
      <div class="options">
        <div class="option" onclick="selectOption(this, 2)" data-opt="A">
          <div class="option-letter">A</div>
          <div class="option-text">Apendicectomia videolaparoscópica de urgência, pois a presença de coleção periapendicular documentada por TC obriga a remoção imediata do foco infeccioso.</div>
        </div>
        <div class="option" onclick="selectOption(this, 2)" data-opt="B">
          <div class="option-letter">B</div>
          <div class="option-text">Laparotomia exploradora de urgência por incisão de McBurney, pois as incisões locais são as mais indicadas quando há massa palpável em FID com diagnóstico provável de apendicite complicada.</div>
        </div>
        <div class="option" onclick="selectOption(this, 2)" data-opt="C">
          <div class="option-letter">C</div>
          <div class="option-text">Drenagem percutânea guiada por imagem + antibioticoterapia sistêmica, seguida de apendicectomia de intervalo após 6–8 semanas, com colonoscopia no período intermediário para excluir neoplasia.</div>
        </div>
        <div class="option" onclick="selectOption(this, 2)" data-opt="D">
          <div class="option-letter">D</div>
          <div class="option-text">Antibioticoterapia exclusiva por 14 dias, com reavaliação clínica e de imagem, reservando a cirurgia apenas para os casos refratários ao tratamento clínico após esse período.</div>
        </div>
        <div class="option" onclick="selectOption(this, 2)" data-opt="E">
          <div class="option-letter">E</div>
          <div class="option-text">Alta hospitalar com antibioticoterapia oral e retorno ambulatorial em 72 horas, pois o quadro está localizado, o paciente encontra-se estável e a ausência de peritonite difusa permite manejo ambulatorial.</div>
        </div>
      </div>
      <button class="confirm-btn" onclick="confirmAnswer(2, 'C')" id="btn-2">Confirmar resposta</button>
      <div class="feedback-box" id="fb-2"></div>
    </div>

    <!-- Q3 -->
    <div class="question-card" id="qcard-3">
      <div class="q-header">
        <div class="q-num">Q3</div>
        <div class="q-stem">Um rapaz de 17 anos, previamente hígido, apresenta quadro de 11 horas de dor abdominal com as seguintes características: dor em cólica periumbilical há 5 horas que migrou para FID há 6 horas, náuseas, hiporexia e um episódio de vômito. Temperatura 38,1°C. Ao exame físico: palpação profunda dolorosa em FID, Blumberg positivo, Rovsing positivo. Sinal do psoas negativo. Leucocitose de 16.800 com 78% neutrófilos e desvio à esquerda.</div>
      </div>
      <div class="q-question">Qual o mecanismo fisiopatológico responsável pelo Sinal de Rovsing positivo neste paciente?</div>
      <div class="options">
        <div class="option" onclick="selectOption(this, 3)" data-opt="A">
          <div class="option-letter">A</div>
          <div class="option-text">A compressão da FIE causa distensão do cólon sigmoide, que por adjacência anatômica direta, transmite pressão ao apêndice cecal inflamado via peritônio parietal posterior.</div>
        </div>
        <div class="option" onclick="selectOption(this, 3)" data-opt="B">
          <div class="option-letter">B</div>
          <div class="option-text">A compressão manual da FIE provoca retorno retrógrado de gases do cólon esquerdo para o ceco, distendendo o apêndice inflamado e produzindo dor referida em FID.</div>
        </div>
        <div class="option" onclick="selectOption(this, 3)" data-opt="C">
          <div class="option-letter">C</div>
          <div class="option-text">A palpação profunda da FIE descomprime transitoriamente o apêndice, permitindo o refluxo de material inflamatório para o ceco, que ao ser recomprimido pelo peritônio, gera dor em FID.</div>
        </div>
        <div class="option" onclick="selectOption(this, 3)" data-opt="D">
          <div class="option-letter">D</div>
          <div class="option-text">A compressão da FIE ativa reflexos viscerais segmentares via plexo celíaco, que se manifestam como dor referida em FID por compartilhamento de dermátomos T10–T12 bilateralmente.</div>
        </div>
        <div class="option" onclick="selectOption(this, 3)" data-opt="E">
          <div class="option-letter">E</div>
          <div class="option-text">A pressão exercida na FIE eleva a pressão intra-abdominal global, que se transmite isotropicamente pela cavidade peritoneal, amplificando a sensibilidade do peritônio já inflamado em FID.</div>
        </div>
      </div>
      <button class="confirm-btn" onclick="confirmAnswer(3, 'B')" id="btn-3">Confirmar resposta</button>
      <div class="feedback-box" id="fb-3"></div>
    </div>

    <!-- Q4 -->
    <div class="question-card" id="qcard-4">
      <div class="q-header">
        <div class="q-num">Q4</div>
        <div class="q-stem">Uma mulher de 28 anos, professora, G0P0, ciclos menstruais regulares, último período há 18 dias, sem uso de anticoncepcional, procura o PA com dor em FID há 6 horas, de início gradual, associada a náuseas e temperatura de 37,9°C. Ao exame: Blumberg positivo, Rovsing positivo, defesa localizada em FID. Leucocitose de 14.500. A residente de plantão considera o escore de Alvarado elevado e deseja encaminhar diretamente à cirurgia.</div>
      </div>
      <div class="q-question">Qual é a etapa diagnóstica que DEVE ser realizada antes de qualquer decisão terapêutica definitiva neste caso, e por quê?</div>
      <div class="options">
        <div class="option" onclick="selectOption(this, 4)" data-opt="A">
          <div class="option-letter">A</div>
          <div class="option-text">Ultrassonografia transvaginal, pois é o método de maior sensibilidade para diagnóstico diferencial ginecológico em mulheres em idade fértil com dor em FID e quadro clínico compatível com apendicite.</div>
        </div>
        <div class="option" onclick="selectOption(this, 4)" data-opt="B">
          <div class="option-letter">B</div>
          <div class="option-text">Dosagem de beta-hCG sérico, pois a possibilidade de gestação ectópica em mulher sem anticoncepcional, com último período há 18 dias, é clinicamente relevante e a conduta cirúrgica seria equivocada sem sua exclusão.</div>
        </div>
        <div class="option" onclick="selectOption(this, 4)" data-opt="C">
          <div class="option-letter">C</div>
          <div class="option-text">Tomografia computadorizada de abdome com contraste, pois a TC tem maior acurácia que o exame físico e o escore de Alvarado para diferenciação entre apendicite e patologias ginecológicas em mulheres jovens.</div>
        </div>
        <div class="option" onclick="selectOption(this, 4)" data-opt="D">
          <div class="option-letter">D</div>
          <div class="option-text">Nenhuma etapa adicional é necessária: o Alvarado ≥7 com peritonite localizada em FID tem indicação cirúrgica independente do sexo do paciente, e a eventual patologia ginecológica seria identificada na exploração laparoscópica.</div>
        </div>
        <div class="option" onclick="selectOption(this, 4)" data-opt="E">
          <div class="option-letter">E</div>
          <div class="option-text">Dosagem de CA-125 sérico, pois mulheres em idade fértil com dor em FID e leucocitose têm maior probabilidade de torção ovariana, cujo marcador tumoral eleva-se precocemente na isquemia do ovário.</div>
        </div>
      </div>
      <button class="confirm-btn" onclick="confirmAnswer(4, 'B')" id="btn-4">Confirmar resposta</button>
      <div class="feedback-box" id="fb-4"></div>
    </div>

    <!-- Q5 -->
    <div class="question-card" id="qcard-5">
      <div class="q-header">
        <div class="q-num">Q5</div>
        <div class="q-stem">Um homem de 33 anos é submetido a apendicectomia videolaparoscópica de urgência por quadro de 14 horas de evolução com peritonite em FID. O laudo anatomopatológico da peça cirúrgica descreve: "apêndice com necrose segmentar isquêmica, ausência de perfuração macroscópica, base do apêndice íntegra. Exsudato fibrino-purulento na serosa. Ausência de neoplasia."</div>
      </div>
      <div class="q-question">Com base no laudo anatomopatológico, qual é a fase anatomopatológica e qual deve ser a conduta com antibióticos no pós-operatório?</div>
      <div class="options">
        <div class="option" onclick="selectOption(this, 5)" data-opt="A">
          <div class="option-letter">A</div>
          <div class="option-text">Fase 2 (úlcero-flegmonosa); antibiótico profilático até 24 horas, pois ainda não há necrose mural completa e o exsudato fibrinoso na serosa é critério de apendicite não complicada.</div>
        </div>
        <div class="option" onclick="selectOption(this, 5)" data-opt="B">
          <div class="option-letter">B</div>
          <div class="option-text">Fase 3 (gangrenosa); antibiótico terapêutico por 7 dias, pois a presença de necrose segmentar classifica a apendicite como complicada, independentemente da ausência de perfuração macroscópica.</div>
        </div>
        <div class="option" onclick="selectOption(this, 5)" data-opt="C">
          <div class="option-letter">C</div>
          <div class="option-text">Fase 4 (perfurativa); antibiótico terapêutico por 14 dias, pois a necrose isquêmica segmentar corresponde necessariamente à perfuração microscópica, que exige tratamento antibiótico prolongado.</div>
        </div>
        <div class="option" onclick="selectOption(this, 5)" data-opt="D">
          <div class="option-letter">D</div>
          <div class="option-text">Fase 2 (úlcero-flegmonosa); antibiótico terapêutico por 7 dias, pois a presença de exsudato fibrinoso na serosa indica contaminação da cavidade e classifica o caso como apendicite complicada.</div>
        </div>
        <div class="option" onclick="selectOption(this, 5)" data-opt="E">
          <div class="option-letter">E</div>
          <div class="option-text">Fase 3 (gangrenosa); antibiótico profilático até 24 horas, pois a ausência de perfuração e de contaminação cavitária com conteúdo fecal mantém o caso como apendicite não complicada para fins de antibioticoterapia.</div>
        </div>
      </div>
      <button class="confirm-btn" onclick="confirmAnswer(5, 'B')" id="btn-5">Confirmar resposta</button>
      <div class="feedback-box" id="fb-5"></div>
    </div>

    <!-- Q6 -->
    <div class="question-card" id="qcard-6">
      <div class="q-header">
        <div class="q-num">Q6</div>
        <div class="q-stem">Um pré-adolescente de 13 anos apresenta quadro de 5 dias de evolução de dor abdominal em FID de moderada intensidade, sem piora progressiva. Refere infecção de vias aéreas superiores (coriza, febre baixa, odinofagia) há 10 dias, resolvida espontaneamente. Sem anorexia ou vômitos. Temperatura atual 37,4°C. Ao exame: dor discreta à palpação profunda em FID sem defesa muscular. Blumberg negativo. Leucograma: 9.800/mm³. Escore de Alvarado: 3 pontos.</div>
      </div>
      <div class="q-question">Qual é o diagnóstico mais provável e qual a conduta adequada?</div>
      <div class="options">
        <div class="option" onclick="selectOption(this, 6)" data-opt="A">
          <div class="option-letter">A</div>
          <div class="option-text">Apendicite aguda em fase inicial (edematosa); deve-se solicitar ultrassonografia e, se negativa, realizar tomografia computadorizada para não perder o diagnóstico em fase precoce.</div>
        </div>
        <div class="option" onclick="selectOption(this, 6)" data-opt="B">
          <div class="option-letter">B</div>
          <div class="option-text">Linfadenite mesentérica; trata-se de doença autolimitada, decorrente de inflamação de linfonodos mesentéricos após infecção viral recente, com tratamento de suporte e sem indicação cirúrgica.</div>
        </div>
        <div class="option" onclick="selectOption(this, 6)" data-opt="C">
          <div class="option-letter">C</div>
          <div class="option-text">Doença de Crohn em fase inicial; a dor em FID crônica em adolescente com infecção recente e Alvarado baixo orienta para diagnóstico inflamatório intestinal, indicando colonoscopia.</div>
        </div>
        <div class="option" onclick="selectOption(this, 6)" data-opt="D">
          <div class="option-letter">D</div>
          <div class="option-text">Apendagite epiploica; lesão inflamatória autolimitada do apêndice epiploico, que pode ser confirmada por imagem, e é tratada clinicamente com anti-inflamatórios.</div>
        </div>
        <div class="option" onclick="selectOption(this, 6)" data-opt="E">
          <div class="option-letter">E</div>
          <div class="option-text">Apendicite subaguda; o longo período de evolução (5 dias) sem piora configura apendicite arrastada, com indicação de antibioticoterapia oral e reavaliação ambulatorial em 48 horas.</div>
        </div>
      </div>
      <button class="confirm-btn" onclick="confirmAnswer(6, 'B')" id="btn-6">Confirmar resposta</button>
      <div class="feedback-box" id="fb-6"></div>
    </div>

    <!-- Q7 -->
    <div class="question-card" id="qcard-7">
      <div class="q-header">
        <div class="q-num">Q7</div>
        <div class="q-stem">Dois pacientes chegam ao PS com dor em FID. Paciente A: homem de 25 anos, dor há 10 horas migrada de periumbilical para FID, anorexia, náuseas, temperatura 38°C, Blumberg positivo, leucocitose 15.200 com desvio. Paciente B: homem de 40 anos, dor em FID há 3 horas, sem migração prévia, sem anorexia, episódios prévios de dor semelhante, temperatura 37,2°C, Blumberg duvidoso, leucocitose 11.000 sem desvio. Em TC do Paciente B: lesão ovaloide hipodensa paracólica direita de 1,8 cm com centro hiperdenso e halo inflamatório, sem visualização de apêndice anormal.</div>
      </div>
      <div class="q-question">Qual é a interpretação mais precisa dos dois casos e a conduta distinta indicada para cada um?</div>
      <div class="options">
        <div class="option" onclick="selectOption(this, 7)" data-opt="A">
          <div class="option-letter">A</div>
          <div class="option-text">Paciente A: apendicite aguda — apendicectomia de urgência. Paciente B: apendicite crônica — apendicectomia eletiva com intervalo de 4 semanas após antibioticoterapia.</div>
        </div>
        <div class="option" onclick="selectOption(this, 7)" data-opt="B">
          <div class="option-letter">B</div>
          <div class="option-text">Paciente A: apendicite aguda — apendicectomia videolaparoscópica de urgência. Paciente B: apendagite epiploica — tratamento conservador com anti-inflamatórios e analgésicos, cirurgia apenas se complicações.</div>
        </div>
        <div class="option" onclick="selectOption(this, 7)" data-opt="C">
          <div class="option-letter">C</div>
          <div class="option-text">Paciente A: apendicite aguda — solicitar TC para confirmar antes de operar, pois a leucocitose sem desvio à esquerda explícito não garante diagnóstico definitivo. Paciente B: apendagite epiploica — tratamento conservador.</div>
        </div>
        <div class="option" onclick="selectOption(this, 7)" data-opt="D">
          <div class="option-letter">D</div>
          <div class="option-text">Ambos os pacientes têm apresentação de dor em FID e devem ser submetidos ao mesmo protocolo: TC de abdome e, se confirmar apendicite em qualquer estágio, apendicectomia de urgência.</div>
        </div>
        <div class="option" onclick="selectOption(this, 7)" data-opt="E">
          <div class="option-letter">E</div>
          <div class="option-text">Paciente A: linfadenite mesentérica — tratamento de suporte, pois não há desvio à esquerda confirmado. Paciente B: apendagite epiploica — laparoscopia diagnóstica para confirmação antes do tratamento conservador.</div>
        </div>
      </div>
      <button class="confirm-btn" onclick="confirmAnswer(7, 'B')" id="btn-7">Confirmar resposta</button>
      <div class="feedback-box" id="fb-7"></div>
    </div>

    <!-- Q8 -->
    <div class="question-card" id="qcard-8">
      <div class="q-header">
        <div class="q-num">Q8</div>
        <div class="q-stem">Um homem de 58 anos é submetido a apendicectomia videolaparoscópica de urgência por apendicite com 18 horas de evolução. O procedimento ocorre sem intercorrências. O laudo anatomopatológico, disponível no 7° dia de pós-operatório, revela: "tumor carcinoide (neuroendócrino bem diferenciado) na ponta do apêndice, medindo 1,3 cm em maior eixo. Margens cirúrgicas livres. Ausência de invasão angiolinfática. Sem comprometimento do mesoapêndice. Ausência de linfonodos comprometidos."</div>
      </div>
      <div class="q-question">Qual é a conduta correta para este paciente no retorno ambulatorial?</div>
      <div class="options">
        <div class="option" onclick="selectOption(this, 8)" data-opt="A">
          <div class="option-letter">B</div>
          <div class="option-text">Hemicolectomia direita oncológica complementar, pois qualquer tumor carcinoide apendicular com tamanho entre 1 e 2 cm tem indicação mandatória de ampliação cirúrgica para reduzir o risco de recorrência linfonodal.</div>
        </div>
        <div class="option" onclick="selectOption(this, 8)" data-opt="B">
          <div class="option-letter">A</div>
          <div class="option-text">Nenhuma intervenção adicional é necessária — a apendicectomia foi curativa. O tumor está na ponta, mede 1,3 cm, tem margens livres, sem invasão angiolinfática e sem comprometimento do mesoapêndice, configurando critérios de ressecção adequada.</div>
        </div>
        <div class="option" onclick="selectOption(this, 8)" data-opt="C">
          <div class="option-letter">C</div>
          <div class="option-text">Encaminhar para oncologia para iniciação de quimioterapia adjuvante com estreptozocina, pois tumores neuroendócrinos bem diferenciados do apêndice com >1 cm têm indicação de tratamento sistêmico complementar.</div>
        </div>
        <div class="option" onclick="selectOption(this, 8)" data-opt="D">
          <div class="option-letter">D</div>
          <div class="option-text">Radioterapia abdominal adjuvante seguida de octreotida de depósito, pois tumores carcinoides apendiculares exigem supressão hormonal crônica independentemente do estadiamento.</div>
        </div>
        <div class="option" onclick="selectOption(this, 8)" data-opt="E">
          <div class="option-letter">E</div>
          <div class="option-text">Colonoscopia de controle em 6 meses para rastreamento de lesões sincronicas e, se normal, seguimento com tomografia semestral por 5 anos para monitorar metástases hepáticas tardias.</div>
        </div>
      </div>
      <button class="confirm-btn" onclick="confirmAnswer(8, 'B')" id="btn-8">Confirmar resposta</button>
      <div class="feedback-box" id="fb-8"></div>
    </div>

    <!-- Q9 -->
    <div class="question-card" id="qcard-9">
      <div class="q-header">
        <div class="q-num">Q9</div>
        <div class="q-stem">Uma gestante de 22 semanas, G2P1, apresenta dor abdominal há 8 horas, predominantemente no flanco e hipocôndrio direito, sem localização clara em FID. Afebril. Leucocitose de 16.000 (a paciente informa que o obstetra já havia identificado leucocitose leve de 12.000 no pré-natal recente). Sem corrimento ou sangramento vaginal. Beta-hCG: positivo (gestação confirmada). Ultrassonografia obstétrica demonstra feto com 22 semanas eutrófico, sem alterações. A ultrassonografia abdominal não visualizou o apêndice.</div>
      </div>
      <div class="q-question">Qual é a próxima etapa diagnóstica mais adequada e qual o raciocínio que a justifica?</div>
      <div class="options">
        <div class="option" onclick="selectOption(this, 9)" data-opt="A">
          <div class="option-letter">A</div>
          <div class="option-text">Tomografia computadorizada de abdome sem contraste, pois a dose de radiação de uma única TC abdominal está dentro dos limites seguros estabelecidos para gestantes acima de 20 semanas e supera a ressonância em acurácia para apendicite.</div>
        </div>
        <div class="option" onclick="selectOption(this, 9)" data-opt="B">
          <div class="option-letter">B</div>
          <div class="option-text">Ressonância magnética de abdome sem contraste, pois é o método de escolha na gestante quando a ultrassonografia é inconclusiva — sem radiação ionizante, com alta acurácia para apendicite e sem risco documentado para o feto.</div>
        </div>
        <div class="option" onclick="selectOption(this, 9)" data-opt="C">
          <div class="option-letter">C</div>
          <div class="option-text">Laparoscopia diagnóstica imediata, pois a não visualização do apêndice à USG em gestante com dor e leucocitose configura peritonite até prova em contrário, e o benefício cirúrgico supera os riscos do procedimento.</div>
        </div>
        <div class="option" onclick="selectOption(this, 9)" data-opt="D">
          <div class="option-letter">D</div>
          <div class="option-text">Observação clínica com nova ultrassonografia em 6 horas, pois a leucocitose é fisiológica na gestação e a dor pode ser decorrente de alterações uterinas compressivas esperadas para a 22ª semana.</div>
        </div>
        <div class="option" onclick="selectOption(this, 9)" data-opt="E">
          <div class="option-letter">E</div>
          <div class="option-text">Tomografia de abdome com contraste iodado endovenoso, pois o diagnóstico preciso da apendicite em gestante justifica o uso de contraste, e o gadolínio (contraste de RM) está contraindicado no segundo trimestre.</div>
        </div>
      </div>
      <button class="confirm-btn" onclick="confirmAnswer(9, 'B')" id="btn-9">Confirmar resposta</button>
      <div class="feedback-box" id="fb-9"></div>
    </div>

    <!-- Q10 -->
    <div class="question-card" id="qcard-10">
      <div class="q-header">
        <div class="q-num">Q10</div>
        <div class="q-stem">Um homem de 38 anos com dor em FID há 16 horas, típica migração periumbilical, febre 38,3°C, Blumberg positivo, leucocitose 17.200 com desvio. Escore de Alvarado: 9. Ao ser submetido a apendicectomia videolaparoscópica de urgência, o cirurgião encontra apêndice com aspecto flegmonoso e exsudato fibrinoso periapendicular, sem perfuração, coleções ou secreção purulenta livre na cavidade. O laudo anatomopatológico posterior é: "Fase 2 — úlcero-flegmonosa; exsudato fibrino-purulento. Mucosa com úlceras. Serosa com exsudato fibrinoso. Ausência de necrose mural. Margens livres. Sem neoplasia."</div>
      </div>
      <div class="q-question">Qual é a conduta correta com antibiótico no pós-operatório imediato com base no laudo final?</div>
      <div class="options">
        <div class="option" onclick="selectOption(this, 10)" data-opt="A">
          <div class="option-letter">A</div>
          <div class="option-text">Manter antibiótico terapêutico (ceftriaxona + metronidazol) por 7 dias, pois a presença de exsudato fibrino-purulento periapendicular na peça cirúrgica caracteriza apendicite complicada, independente da ausência de perfuração.</div>
        </div>
        <div class="option" onclick="selectOption(this, 10)" data-opt="B">
          <div class="option-letter">B</div>
          <div class="option-text">Manter antibiótico terapêutico por 5 dias, pois a úlcera mucosa com exsudato seroso é critério de apendicite em fase intermediária, que requer tratamento por período reduzido em relação à fase gangrenosa ou perfurativa.</div>
        </div>
        <div class="option" onclick="selectOption(this, 10)" data-opt="C">
          <div class="option-letter">C</div>
          <div class="option-text">Suspender o antibiótico nas primeiras 24 horas do pós-operatório, pois a apendicite úlcero-flegmonosa (Fase 2) é classificada como não complicada, e o antibiótico pré e intraoperatório cumpriu função profilática.</div>
        </div>
        <div class="option" onclick="selectOption(this, 10)" data-opt="D">
          <div class="option-letter">D</div>
          <div class="option-text">Iniciar antibioticoterapia oral e manter por 10 dias, pois o exsudato purulento na serosa indica translocação bacteriana com necessidade de cobertura prolongada para prevenir abscesso intra-abdominal tardio.</div>
        </div>
        <div class="option" onclick="selectOption(this, 10)" data-opt="E">
          <div class="option-letter">E</div>
          <div class="option-text">Manter antibiótico terapêutico por 7 dias, pois a leucocitose pré-operatória de 17.200 com desvio à esquerda indica resposta inflamatória sistêmica grave que classifica o caso como complicado independentemente do laudo anatomopatológico.</div>
        </div>
      </div>
      <button class="confirm-btn" onclick="confirmAnswer(10, 'C')" id="btn-10">Confirmar resposta</button>
      <div class="feedback-box" id="fb-10"></div>
    </div>

    <!-- SCORE PANEL -->
    <div id="score-panel">
      <span class="score-num" id="score-display">0/10</span>
      <p class="score-label">questões corretas</p>
      <p class="score-msg" id="score-msg"></p>
      <button class="reset-btn" onclick="resetQuiz()">↺ Reiniciar simulado</button>
    </div>
  </div>
</section>

</main>

<footer>
  <span class="footer-name">Kyra Barreneche</span>
  <span>Semiologia I · CENSUPEG · Joinville, SC</span><br>
  <span style="display:inline-block; margin-top:0.4rem; font-family: 'IBM Plex Mono', monospace; font-style: italic; color: var(--rose-deep);">"O paciente não espera que você se lembre. Ele espera que você raciocine." — Prof. Dr. João Vitor Galo Esteves</span>
</footer>

<script>
// Progress bar
window.addEventListener('scroll', () => {
  const scrollTop = window.scrollY;
  const docHeight = document.documentElement.scrollHeight - window.innerHeight;
  const pct = docHeight > 0 ? (scrollTop / docHeight) * 100 : 0;
  document.getElementById('progress-bar').style.width = pct + '%';
});

// Accordion
function toggleAccordion(header) {
  const accordion = header.parentElement;
  accordion.classList.toggle('open');
}

// Reveal
function toggleReveal(id) {
  const el = document.getElementById(id);
  const btn = el.previousElementSibling;
  if (el.classList.contains('shown')) {
    el.classList.remove('shown');
    btn.textContent = btn.textContent.replace('▼', '▶');
  } else {
    el.classList.add('shown');
    btn.textContent = btn.textContent.replace('▶', '▼');
  }
}

// Quiz
let answers = {};
let answered = {};
let correctCount = 0;

const feedbacks = {
  1: {
    correct: '<span class="feedback-label">✓ Correto</span>O escore de Alvarado desta paciente é: migração da dor (1) + anorexia (1) + náusea (1) + defesa em FID (2) + Blumberg (1) + febre (1) + leucocitose (2) = <strong>9 pontos</strong>. Com Alvarado ≥7 e peritonite localizada documentada, a indicação cirúrgica é direta — sem necessidade de imagem. A videolaparoscopia é a via preferencial. O beta-hCG, embora relevante em mulheres, não foi a pergunta-foco aqui — a alternativa E também peca por indicar laparotomia mediana sem justificativa em caso inicial não complicado.',
    wrong: '<span class="feedback-label">✗ Incorreto</span>Revise o Escore de Alvarado: com 9 pontos, o quadro tem indicação cirúrgica direta. A TC (alternativa A) está indicada nos casos com Alvarado 4–6, não em Alvarado ≥7. A ultrassonografia em adolescentes do sexo feminino (alternativa B) seria pertinente se houvesse dúvida diagnóstica — mas o escore aqui é definitivo. A reavaliação seriada (alternativa D) é para casos muito precoces sem peritonite estabelecida, não para Alvarado 9 com Blumberg positivo.'
  },
  2: {
    correct: '<span class="feedback-label">✓ Correto</span>O cenário clássico do <strong>plastrão apendicular</strong> com abscesso periapendicular: mais de 7 dias de evolução, massa palpável em FID, coleção na TC. A conduta é <strong>tratamento não operatório inicial</strong> — drenagem percutânea + antibioticoterapia, seguida de apendicectomia de intervalo após 6–8 semanas. A colonoscopia no período intermediário é obrigatória para excluir neoplasia associada ao apêndice. A apendicectomia imediata (A ou B) aumenta morbidade nesse cenário.',
    wrong: '<span class="feedback-label">✗ Incorreto</span>Este é o cenário do plastrão com abscesso periapendicular — conduta NÃO é cirurgia imediata. A apendicectomia de urgência (A e B) nesse contexto tem alto risco de lesão de estruturas adjacentes aderidas ao plastrão. A alternativa D (antibiótico exclusivo sem drenagem) é insuficiente para coleção de 4 cm. A alta (E) é perigosa. A resposta C é a conduta correta: drenagem + antibioticoterapia → colonoscopia → apendicectomia de intervalo.'
  },
  3: {
    correct: '<span class="feedback-label">✓ Correto</span>O Sinal de Rovsing deve ser compreendido mecanisticamente: a compressão manual da fossa ilíaca esquerda empurra os gases do cólon esquerdo <strong>retrogradamente</strong> — contra a peristalse normal — até o ceco, distendendo o ceco e o apêndice inflamado. Essa distensão do apêndice já inflamado gera dor referida em FID. É uma "sensibilidade rebote referida contralateral" por mecanismo gasoso, não por pressão direta.',
    wrong: '<span class="feedback-label">✗ Incorreto</span>As alternativas A, C, D e E confundem o mecanismo do Rovsing. A (transmissão por adjacência anatômica direta) não é o mecanismo correto — o cólon sigmoide não é "adjacente direto" ao apêndice. C (refluxo de material inflamatório) é anatomicamente impossível. D (reflexo segmentar via plexo celíaco) descreve um mecanismo visceral, não o do Rovsing. E (elevação global da pressão intra-abdominal) seria inespecífico — qualquer compressão causaria isso. O mecanismo real é a compressão retrógrada de gases.'
  },
  4: {
    correct: '<span class="feedback-label">✓ Correto</span>Em toda mulher em idade reprodutiva com dor em FID, o <strong>beta-hCG é obrigatório</strong>, independentemente da regularidade menstrual ou da aparência do escore de Alvarado. A gestação ectópica é um diagnóstico que pode mimetizar apendicite e, se rota, leva ao choque hemorrágico. Com último período há 18 dias e sem anticoncepcional, a possibilidade de gestação precoce não pode ser descartada clinicamente. A USG transvaginal (A) seria adequada após o beta-hCG. A TC (C) viria depois. A laparoscopia direta (D) em mulher sem beta-hCG seria erro grave.',
    wrong: '<span class="feedback-label">✗ Incorreto</span>A alternativa B é a correta. Nenhuma decisão cirúrgica deve ser tomada em mulher em idade fértil com dor em FID sem beta-hCG. O CA-125 (E) não é o marcador de torção ovariana na fase aguda — e mesmo que fosse, não excluiria gestação ectópica. A TC (C) expõe à radiação sem necessidade se o diagnóstico diferencial prioritário (gestação ectópica) ainda não foi excluído por exame simples.'
  },
  5: {
    correct: '<span class="feedback-label">✓ Correto</span>O laudo descreve <strong>necrose segmentar isquêmica com base íntegra e ausência de perfuração macroscópica</strong> — isso corresponde exatamente à <strong>Fase 3 (gangrenosa)</strong> da classificação anatomopatológica. A fase gangrenosa é considerada <strong>apendicite complicada</strong>, independentemente da ausência de perfuração. Portanto, a conduta correta é antibiótico <strong>terapêutico por 7 dias</strong> cobrindo gram-negativos e anaeróbios. A alternativa E erra ao dizer que ausência de perfuração mantém o caso como não complicado — a necrose mural já classifica como complicado.',
    wrong: '<span class="feedback-label">✗ Incorreto</span>O erro frequente é confundir ausência de perfuração com ausência de complicação. A necrose mural (fase gangrenosa) JÁ configura apendicite complicada, exigindo 7 dias de antibiótico terapêutico. A alternativa C erra ao suspender após 24h como se fosse profilático. As alternativas A e D confundem a fase correta. O laudo é claro: necrose segmentar = Fase 3 = complicada = 7 dias de terapêutico.'
  },
  6: {
    correct: '<span class="feedback-label">✓ Correto</span>O conjunto de pistas é claro: <strong>pré-adolescente + quadro gripal 1–2 semanas antes + dor branda em FID sem peritonite + Alvarado ≤3 + leucograma normal</strong> — o diagnóstico é <strong>linfadenite mesentérica</strong>. Trata-se de inflamação de linfonodos mesentéricos após infecção viral, autolimitada, sem necessidade de cirurgia. O tratamento é de suporte. Alvarado ≤3 fala fortemente contra apendicite. A Doença de Crohn (C) teria história de surtos prévios. A apendagite (D) seria em adulto com imagem característica.',
    wrong: '<span class="feedback-label">✗ Incorreto</span>As pistas no enunciado são clássicas de linfadenite mesentérica: adolescente, quadro viral recente, dor branda, sem peritonite, Alvarado ≤3. A apendicite (A e E) seria improvável com esse escore e sem defesa/Blumberg. A Doença de Crohn (C) requereria história de surtos prévios e achados endoscópicos. A apendagite (D) tem imagem típica (lesão ovaloide hipodensa paracólica) e ocorre mais em adultos obesos — o enunciado não descreve imagem.'
  },
  7: {
    correct: '<span class="feedback-label">✓ Correto</span>Paciente A: quadro clássico de apendicite com Alvarado alto — <strong>apendicectomia videolaparoscópica de urgência</strong>, sem necessidade de imagem. Paciente B: a TC revela <strong>lesão ovaloide hipodensa paracólica</strong> com centro hiperdenso e halo inflamatório — achado patognomônico de <strong>apendagite epiploica</strong>. Trata-se de inflamação e infarto de apêndice epiploico, doença autolimitada, com tratamento conservador (anti-inflamatórios + analgesia) e sem indicação cirúrgica na ausência de complicações. A diferenciação entre os dois diagnósticos é o exercício central desta questão.',
    wrong: '<span class="feedback-label">✗ Incorreto</span>A alternativa B é a correta. O erro mais frequente é não reconhecer a apendagite epiploica pela imagem TC característica (lesão ovaloide hipodensa paracólica). A alternativa A erra ao classificar o Paciente B como "apendicite crônica". A alternativa C erra ao pedir TC para o Paciente A com Alvarado alto e peritonite clara. A alternativa D erra ao aplicar o mesmo protocolo para dois quadros completamente distintos.'
  },
  8: {
    correct: '<span class="feedback-label">✓ Correto</span>Aplicando os critérios para tumor carcinoide apendicular: tumor na ponta do apêndice, 1,3 cm, margens livres, sem invasão angiolinfática, sem comprometimento de mesoapêndice, sem linfonodos comprometidos. Esse perfil configura <strong>ressecção cirúrgica adequada</strong> — a apendicectomia foi curativa. Hemicolectomia direita está indicada apenas em tumores >2 cm OU com fatores adversos (invasão linfovascular, base comprometida, mesoapêndice acometido, linfonodos positivos). Quimioterapia e radioterapia não fazem parte do manejo padrão nesses casos.',
    wrong: '<span class="feedback-label">✗ Incorreto</span>Atenção aos critérios de hemicolectomia: são necessários tumor >2 cm OU fatores adversos (invasão angiolinfática, base comprometida, mesoapêndice acometido). Este tumor tem 1,3 cm, está na ponta, sem qualquer fator adverso — critérios que classicamente indicam apendicectomia como tratamento definitivo. Quimioterapia (C) e radioterapia (D) não são partes do manejo de tumores carcinoides apendiculares ressecáveis.'
  },
  9: {
    correct: '<span class="feedback-label">✓ Correto</span>Na gestante com USG inconclusiva (apêndice não visualizado), o próximo passo é a <strong>Ressonância Magnética</strong> — sem radiação ionizante, alta acurácia para apendicite (sensibilidade >90%), segura no segundo trimestre. A TC (A e E) usa radiação ionizante, que deve ser evitada na gestação, especialmente quando existe alternativa de igual ou maior acurácia. A laparoscopia imediata (C) sem confirmação diagnóstica em gestante sem peritonite não é a conduta adequada. A observação (D) seria perigosa com quadro de dor evolutiva e leucocitose elevada.',
    wrong: '<span class="feedback-label">✗ Incorreto</span>Na gestante com USG inconclusiva, a RM é o padrão para investigação abdominal adicional — sem radiação, segura, acurada. A TC (A e E) expõe a feto à radiação sem necessidade. A alternativa E ainda menciona gadolínio contraindicado — na verdade, contraste de RM (gadolínio) é de uso restrito na gestação, mas a RM sem contraste já tem alta acurácia para apendicite. A laparoscopia (C) sem diagnóstico prévio em gestante estável não é adequada.'
  },
  10: {
    correct: '<span class="feedback-label">✓ Correto</span>O laudo anatomopatológico define: <strong>Fase 2 (úlcero-flegmonosa) = apendicite NÃO complicada</strong>. Não há necrose mural, não há perfuração, não há coleção cavitária. O critério para antibiótico é determinado pelo laudo anatomopatológico, não pela leucocitose ou pela apresentação clínica pré-operatória. Fase 2 → profilático → <strong>suspender antibiótico em até 24 horas do pós-operatório</strong>. A alternativa E comete o erro de usar critério clínico (leucocitose) em vez do anatomopatológico para classificar a fase. As alternativas A, B e D classificam erroneamente o exsudato fibrinoso como "complicado".',
    wrong: '<span class="feedback-label">✗ Incorreto</span>A armadilha aqui é usar a leucocitose pré-operatória ou o exsudato periapendicular como critério de complicação. A classificação da apendicite para fins de antibiótico é <strong>anatomopatológica</strong>: Fases 1 e 2 = não complicada = profilático (até 24h). Fases 3 e 4 = complicada = terapêutico (7 dias). O exsudato fibrinoso na serosa é compatível com Fase 2 — ainda não há necrose, que definiria a Fase 3. A leucocitose elevada é esperada em qualquer processo inflamatório e não altera a classificação da fase.'
  }
};

function selectOption(el, qNum) {
  if (answered[qNum]) return;
  const parent = el.closest('.options');
  parent.querySelectorAll('.option').forEach(o => o.classList.remove('selected'));
  el.classList.add('selected');
  answers[qNum] = el.dataset.opt;
  document.getElementById('btn-' + qNum).disabled = false;
}

function confirmAnswer(qNum, correct) {
  if (answered[qNum]) return;
  const selected = answers[qNum];
  if (!selected) { alert('Selecione uma alternativa primeiro.'); return; }
  answered[qNum] = true;
  const card = document.getElementById('qcard-' + qNum);
  const fb = document.getElementById('fb-' + qNum);
  const btn = document.getElementById('btn-' + qNum);
  btn.disabled = true;
  card.classList.add('answered');
  card.querySelectorAll('.option').forEach(o => {
    o.style.pointerEvents = 'none';
    if (o.dataset.opt === correct) o.classList.add('correct');
    else if (o.dataset.opt === selected && selected !== correct) o.classList.add('wrong');
  });
  const isCorrect = selected === correct;
  if (isCorrect) correctCount++;
  fb.innerHTML = feedbacks[qNum][isCorrect ? 'correct' : 'wrong'];
  fb.className = 'feedback-box ' + (isCorrect ? 'correct-fb' : 'wrong-fb');
  if (Object.keys(answered).length === 10) showScore();
}

function showScore() {
  const panel = document.getElementById('score-panel');
  panel.style.display = 'block';
  document.getElementById('score-display').textContent = correctCount + '/10';
  let msg = '';
  if (correctCount >= 9) msg = 'Excelente! Domínio sólido do conteúdo — você raciocina clinicamente, não apenas memoriza.';
  else if (correctCount >= 7) msg = 'Muito bom! Alguns mecanismos ainda merecem revisão, mas a base está bem construída.';
  else if (correctCount >= 5) msg = 'Bom início. Revise os feedbacks das questões erradas com atenção ao mecanismo de cada erro.';
  else msg = 'Revise o material com foco em fisiopatologia e critérios de classificação — o raciocínio clínico integrado precisa ser fortalecido.';
  document.getElementById('score-msg').textContent = msg;
  panel.scrollIntoView({ behavior: 'smooth', block: 'center' });
}

function resetQuiz() {
  answers = {}; answered = {}; correctCount = 0;
  document.querySelectorAll('.question-card').forEach(c => {
    c.classList.remove('answered');
    c.querySelectorAll('.option').forEach(o => {
      o.className = 'option';
      o.style.pointerEvents = '';
    });
    const num = c.id.split('-')[1];
    const fb = document.getElementById('fb-' + num);
    fb.className = 'feedback-box';
    fb.innerHTML = '';
    const btn = document.getElementById('btn-' + num);
    btn.disabled = false;
  });
  document.getElementById('score-panel').style.display = 'none';
  document.getElementById('simulado').scrollIntoView({ behavior: 'smooth' });
}
</script>
</body>
</html>
