<!DOCTYPE html>
<html lang="sv">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Bibelstudion - Registrering</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>

<!-- Header -->
<header>
  <h1>Bibelstudion</h1>
  <nav>
    <a href="index.html">Startsida</a>
    <a href="registrering.html">Registrera dig</a>
    <a href="nyhetsbrev.html">Nyhetsbrev</a>
    <a href="studier.html">Studier</a>
  </nav>
</header>

<!-- Registreringsformulär -->
<main>
  <div class="form-container">
    <h2>Registrera dig</h2>
    <form id="registrationForm">
      <label for="name">Namn:</label>
      <input type="text" id="name" name="name" placeholder="Ange ditt namn" required>
      
      <label for="email">E-post:</label>
      <input type="email" id="email" name="email" placeholder="Ange din e-postadress" required>
      
      <button type="submit">Registrera dig</button>
    </form>
    <p id="message" style="display: none;">Din VIP-kod skickas till din Gmail!</p>
  </div>
</main>

<!-- Sidfot -->
<footer>
  <p>© 2025 Bibelstudion. Alla rättigheter förbehållna.</p>
</footer>

<script src="script.js"></script>
</body>
</html>


/* Grundinställningar */
body {
  background-color: #000000; /* Svart bakgrund */
  color: #FFFFFF; /* Vit text */
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}

a {
  color: #FFFFFF; /* Vit text för länkar */
  text-decoration: none;
}

a:hover {
  text-decoration: underline;
}

header {
  text-align: center;
  padding: 20px 10px;
  background-color: #000000; /* Svart bakgrund */
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

/* Formulär */
.form-container {
  max-width: 400px;
  margin: 50px auto;
  padding: 20px;
  background-color: #1A1A1A; /* Mörkare bakgrund */
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(255, 255, 255, 0.3);
}

.form-container h2 {
  text-align: center;
  margin-bottom: 20px;
}

.form-container label, 
.form-container input, 
.form-container button {
  display: block;
  width: 100%;
  margin-bottom: 15px;
  font-size: 16px;
}

.form-container input {
  padding: 10px;
  border: 1px solid #FFFFFF;
  background-color: #000000;
  color: #FFFFFF;
  border-radius: 5px;
}

.form-container button {
  background-color: #000000; /* Svart knapp */
  color: #FFFFFF; /* Vit text */
  border: 1px solid #FFFFFF;
  padding: 10px;
  cursor: pointer;
  border-radius: 5px;
}

.form-container button:hover {
  background-color: #D8B2FF; /* Ljuslila */
  color: #000000; /* Svart text */
}

/* Sidfot */
footer {
  background-color: #D8B2FF; /* Ljuslila */
  text-align: center;
  padding: 15px;
  color: #000000; /* Svart text */
}

// Hantera formulärets inlämning
document.getElementById("registrationForm").addEventListener("submit", function (event) {
  event.preventDefault(); // Förhindra siduppdatering
  
  const name = document.getElementById("name").value;
  const email = document.getElementById("email").value;

  // Simulera att VIP-kod skickas
  alert(`Tack för registreringen, ${name}! Din VIP-kod har skickats till ${email}.`);
  
  // Visa ett meddelande till användaren
  const message = document.getElementById("message");
  message.style.display = "block";
});
