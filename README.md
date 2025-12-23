Skip to content
Copilot navigation
Quick links
New chat
Agents
Spaces
Spark
Preview
Chats
Today
Mejoras en HTML y accesibilidad

Collapse


rodrigoratouu-code
Copilot Free
Condense sidebar

Mejoras en HTML y accesibilidad


Workbench

README.md

README.md
Press Delete to close.


354 lines · 11 KB

README.md file contents
  1
  2
  3
  4
  5
  6
  7
  8
  9
 10
 11
 12
 13
 14
 15
 16
 17
 18
 19
 20
 21
 22
 23
 24
 25
 26
 27
 28
 29
 30
 31
 32
 33
 34
 35
 36
 37
 38
 39
 40
 41
 42
 43
 44
 45
 46
 47
 48
 49
 50
 51
 52
 53
 54
 55
 56
 57
 58
 59
 60
 61
 62
 63
 64
 65
 66
 67
 68
 69
 70
 71
 72
 73
 74
 75
 76
 77
 78
 79
 80
 81
 82
 83
 84
 85
 86
 87
<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <meta name="description" content="TuNoSaBeNa - Playlist y vídeos recomendados por Rodri. Catálogo SIMON 270 2025." />
  <meta name="theme-color" content="#0044ff" />
  <title>TuNoSaBeNa — FONTANERO MUSIC</title>

  <style>
    /* Variables y reset ligero */
    :root{
      --bg-start: #0044ff;
      --bg-end: #ff0033;
      --glass-bg: rgba(255,255,255,0.55);
      --glass-strong: rgba(255,255,255,0.8);
      --text: #111;
      --muted-text: rgba(17,17,17,0.75);
      --accent-1: #0072ff;
      --accent-2: #00c6ff;
      --radius: 12px;
      --card-radius: 16px;
      --max-width: 900px;
      --gap: 1rem;
      font-family: "Segoe UI", Roboto, system-ui, -apple-system, "Helvetica Neue", Arial, sans-serif;
    }

    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      min-height:100vh;
      color:var(--text);
      background: linear-gradient(135deg, var(--bg-start) 0%, var(--bg-end) 100%);
      background-attachment: fixed;
      background-size: cover;
      padding:2rem;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
    }

    header{
      max-width:var(--max-width);
      margin:0 auto 1.5rem;
      padding:1.25rem;
      text-align:center;
      background: rgba(255,255,255,0.12);
      border-radius:var(--card-radius);
      color: white;
      box-shadow: 0 6px 24px rgba(0,0,0,0.18);
      backdrop-filter: blur(8px) saturate(140%);
      border: 1px solid rgba(255,255,255,0.08);
    }

    main{
      max-width:var(--max-width);
      margin:0 auto;
      display:grid;
      gap:1.25rem;
    }

    section{
      padding:1.25rem;
      border-radius:var(--card-radius);
      background: var(--glass-bg);
      color: #fff;
      backdrop-filter: blur(14px) saturate(150%);
      border: 1px solid rgba(255,255,255,0.12);
      box-shadow: 0 6px 20px rgba(0,0,0,0.12);
      transition: transform .18s ease, box-shadow .18s ease;
    }

    section:hover{ transform: translateY(-4px); box-shadow: 0 10px 34px rgba(0,0,0,0.18); }

    h1,h2,h3{ margin:0 0 .5rem; color: #fff; }
    p{ margin:.25rem 0 .75rem; color: rgba(255,255,255,0.9); }

    /* Playlist (audio) */
    .playlist{
      display:grid;
      gap:.75rem;
      grid-template-columns: 1fr;
    }
    .track{
      background: rgba(255,255,255,0.06);
      padding:.75rem;
      border-radius:12px;
