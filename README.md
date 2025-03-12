<!DOCTYPE html>
<html lang="fr">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Formulaire de Rénovation</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f9f9f9;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }

    .container {
      background: white;
      padding: 40px;
      border-radius: 16px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
      max-width: 500px;
      width: 100%;
    }

    h1 {
      text-align: center;
      color: #333;
    }

    label {
      display: block;
      margin: 15px 0 5px;
      font-weight: bold;
    }

    input, select {
      width: 100%;
      padding: 10px;
      margin-bottom: 10px;
      border: 1px solid #ccc;
      border-radius: 8px;
      box-sizing: border-box;
    }

    button {
      background-color: #4CAF50;
      color: white;
      padding: 12px 20px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      width: 100%;
    }

    button:hover {
      background-color: #45a049;
    }
  </style>
</head>

<body>
  <div class="container">
    <h1>Formulaire de Rénovation</h1>
    <form action="https://formspree.io/f/{TON_EMAIL}" method="POST">
      <label for="nom">Nom :</label>
      <input type="text" id="nom" name="nom" required>

      <label for="prenom">Prénom :</label>
      <input type="text" id="prenom" name="prenom" required>

      <label for="codePostal">Code postal :</label>
      <input type="text" id="codePostal" name="codePostal" required>

      <label for="telephone">Numéro de téléphone :</label>
      <input type="text" id="telephone" name="telephone" required>

      <label for="surface">Type de surface habitable :</label>
      <input type="text" id="surface" name="surface" required>

      <label for="combles">Combles :</label>
      <select id="combles" name="combles" required>
        <option value="perdus">Perdus</option>
        <option value="amenageables">Aménageables</option>
      </select>

      <label for="isolation">Isolation extérieure :</label>
      <select id="isolation" name="isolation" required>
        <option value="oui">Oui</option>
        <option value="non">Non</option>
      </select>

      <label for="sousSol">Sous-sol, cave ou garage :</label>
      <select id="sousSol" name="sousSol" required>
        <option value="sous-sol">Sous-sol</option>
        <option value="cave">Cave</option>
        <option value="garage">Garage</option>
        <option value="videSanitaire">Vide sanitaire</option>
        <option value="aucun">Aucun</option>
      </select>

      <label for="chauffage">Y a-t-il une pièce chauffée au-dessus ?</label>
      <select id="chauffage" name="chauffage" required>
        <option value="oui">Oui</option>
        <option value="non">Non</option>
      </select>

      <label for="modeChauffage">Mode de chauffage :</label>
      <input type="text" id="modeChauffage" name="modeChauffage" required>

      <button type="submit">Envoyer</button>
    </form>
  </div>
</body>

</html>
