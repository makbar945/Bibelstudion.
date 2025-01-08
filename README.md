<!DOCTYPE html>
<html lang="sv">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Bibelstudion</title>
  <style>
    /* Grundläggande stilmallar */
    body {
      background-color: #000000; /* Svart bakgrund */
      color: #FFFFFF; /* Vit text */
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }

    /* Länkar */
    a {
      color: #9C4BFF; /* Accentfärg (lila) */
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    /* Huvudrubrik och navigering */
    header {
      text-align: center;
      padding: 20px 10px;
      background-color: #9C4BFF; /* Accentfärg */
      color: #FFFFFF;
    }

    nav {
      text-align: center;
      margin: 10px 0;
    }

    nav a {
      margin: 0 15px;
      font-size: 18px;
    }

    /* Sidfot */
    footer {
      background-color: #D8B2FF; /* Ljuslila */
      text-align: center;
      padding: 15px;
      color: #000000; /* Svart text för kontrast */
    }

    /* VIP-inloggningssektionen */
    .vip-login {
      margin-top: 20px;
      text-align: center;
    }

    .vip-login form {
      display: inline-block;
      text-align: left;
    }

    .vip-login label, 
    .vip-login input, 
    .vip-login button {
      display: block;
      margin-bottom: 10px;
      font-size: 16px;
    }

    .vip-login button {
      background-color: #9C4BFF; /* Accentfärg */
      color: #FFFFFF;
      border: none;
      padding: 10px 20px;
      cursor: pointer;
    }

    .vip-login button:hover {
      background-color: #D8B2FF; /* Ljuslila för hover */
    }
  </style>
</head>
<body>

<!-- Header -->
<header>
  <h1>Bibelstudion</h1>
  <nav>
    <a href="index.html">Startsida</a>
    <a href="nyhetsbrev.html">Nyhetsbrev</a>
    <a href="studier.html">Studier</a>
    <a href="bibel-quiz.html">Bibel & quiz</a>
    <a href="om-oss.html">Om oss</a>
    <a href="kontakt.html">Kontakt</a>
    <a href="live.html">Live</a>
  </nav>
</header>

<!-- Huvudinnehåll -->
<main>
  <h2>Välkommen till Bibelstudion!</h2>
  <p>Logga in med din VIP-kod för att komma åt exklusivt innehåll.</p>

  <div class="vip-login">
    <form>
      <label for="vip-code">Ange din VIP-kod:</label>
      <input type="text" id="vip-code" name="vip-code" placeholder="VIP-kod">
      <button type="submit">Logga in</button>
    </form>
  </div>
</main>

<!-- Sidfot -->
<footer>
  <p>© 2025 Bibelstudion. Alla rättigheter förbehållna.</p>
</footer>

</body>
</html>
