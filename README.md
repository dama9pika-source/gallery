
<!doctype html>
<html lang="no">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Mørk galleri</title>
  <style>
    /* Основні кольори теми */
    :root {
      --bg: #0f172a;
      --card: #1e293b;
      --accent: #3b82f6;
      --text: #f1f5f9;
      --muted: #94a3b8;
    }

    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: var(--bg);
      color: var(--text);
      display: flex;
      flex-direction: column;
      min-height: 100vh;
    }

    header {
      text-align: center;
      padding: 2rem 1rem;
      background: linear-gradient(180deg, #1e293b, #0f172a);
      box-shadow: 0 2px 10px rgba(0,0,0,0.6);
    }

    header h1 {
      font-size: 2rem;
      margin-bottom: 0.5rem;
    }

    header p {
      color: var(--muted);
    }

    main {
      display: grid;
      grid-template-columns: 1fr;
      gap: 1rem;
      padding: 1rem;
      max-width: 1200px;
      margin: auto;
      width: 100%;
    }

    /* Галерея – карточки */
    .card {
      background-color: var(--card);
      border-radius: 12px;
      overflow: hidden;
      box-shadow: 0 6px 18px rgba(0,0,0,0.5);
      transition: transform 0.3s, box-shadow 0.3s;
    }

    .card:hover {
      transform: translateY(-6px);
      box-shadow: 0 10px 28px rgba(0,0,0,0.6);
    }

    .card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
    }

    .card-content {
      padding: 1rem;
    }

    .card-content h2 {
      font-size: 1.1rem;
      margin: 0 0 0.3rem;
    }

    .card-content p {
      color: var(--muted);
      font-size: 0.9rem;
      margin: 0;
    }

    /* Grid адаптивність */
    @media (min-width: 600px) {
      main {
        grid-template-columns: repeat(2, 1fr);
      }
    }

    @media (min-width: 900px) {
      main {
        grid-template-columns: repeat(3, 1fr);
      }
    }

    footer {
      text-align: center;
      padding: 1rem;
      color: var(--muted);
      font-size: 0.9rem;
      margin-top: auto;
      border-top: 1px solid #1e293b;
    }
  </style>
</head>
<body>
  <header>
    <h1>Galleri</h1>
    <p>En enkel, responsiv bildegalleri i mørke toner</p>
  </header>

  <main>
    <div class="card">
      <img src="https://i.pinimg.com/736x/7c/5e/6d/7c5e6defba9551c6509528f023a52e8e.jpg" alt="Fjell">
      <div class="card-content">
        <h2>Fjell</h2>
        <p>Vakre fjell i solnedgangen.</p>
      </div>
    </div>

    <div class="card">
      <img src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e?auto=format&fit=crop&w=800&q=80" alt="Hav">
      <div class="card-content">
        <h2>Hav</h2>
        <p>Rolige bølger og mørk himmel.</p>
      </div>
    </div>

    <div class="card">
      <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=800&q=80" alt="Skog">
      <div class="card-content">
        <h2>Skog</h2>
        <p>Tåke over furutrærne.</p>
      </div>
    </div>

    <div class="card">
      <img src="https://images.unsplash.com/photo-1501785888041-af3ef285b470?auto=format&fit=crop&w=800&q=80" alt="Nordlys">
      <div class="card-content">
        <h2>Nordlys</h2>
        <p>Magiske lys over Arktis.</p>
      </div>
    </div>

    <div class="card">
      <img src="https://images.unsplash.com/photo-1469474968028-56623f02e42e?auto=format&fit=crop&w=800&q=80" alt="By">
      <div class="card-content">
        <h2>By</h2>
        <p>Nattens lys i byen.</p>
      </div>
    </div>

    <div class="card">
      <img src="https://i.pinimg.com/1200x/2e/ee/56/2eee566424c1f35fbeacf85496b4b6e7.jpg" alt="Landskap">
      <div class="card-content">
        <h2>Landskap</h2>
        <p>Kontraster mellom fjell og vann.</p>
      </div>
    </div>
  </main>

  <footer>
    © 2025 Galleri – Laget med CSS Grid
  </footer>
</body>
</html>
