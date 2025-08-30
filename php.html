<?php
// On définit une variable pour stocker le message de confirmation ou d'erreur
$message = '';
$isSuccess = false;

// Ce bloc de code ne s'exécute que lorsque le formulaire est soumis
if ($_SERVER["REQUEST_METHOD"] == "POST") {
    // Nettoie les données pour éviter les problèmes de sécurité
    $number = htmlspecialchars($_POST['number']);
    $reason = htmlspecialchars($_POST['reason']);

    // Validation côté serveur : on s'assure que les champs ne sont pas vides
    if (empty($number) || empty($reason)) {
        $message = "Veuillez remplir tous les champs.";
    } else {
        // Validation du format du numéro de téléphone
        $phoneRegex = "/^\+[1-9]\d{1,14}$/";
        if (!preg_match($phoneRegex, $number)) {
            $message = "Le format du numéro de téléphone est incorrect.";
        } else if (strlen($reason) < 50) {
            $message = "La raison doit contenir au moins 50 caractères.";
        } else {
            // Toutes les validations sont passées, on prépare l'email
            $to = "support@whatsapp.com";
            $subject = "Signalement de compte WhatsApp - Rapport par un utilisateur";
            $body = "Bonjour l'équipe de support de WhatsApp,\n\n"
                  . "Je soumets ce rapport concernant une violation des conditions d'utilisation.\n\n"
                  . "Numéro de compte signalé : " . $number . "\n\n"
                  . "Détails du problème :\n" . $reason . "\n\n"
                  . "Cordialement,\nUn utilisateur concerné";
            
            // Pour que la fonction mail() fonctionne, votre serveur doit être configuré
            // avec un service d'envoi d'emails.
            $headers = "From: webmaster@monsite.com"; // Remplacer par votre propre email de contact
            
            // Tente d'envoyer l'email
            if (mail($to, $subject, $body, $headers)) {
                $message = "Votre rapport a été envoyé avec succès ! Merci pour votre collaboration.";
                $isSuccess = true;
            } else {
                $message = "Une erreur est survenue lors de l'envoi du rapport. Veuillez réessayer plus tard.";
            }
        }
    }
}
?>

<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Power X Ban - Service de Signalement PHP</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
  <style>
    body {
      background: linear-gradient(to right, #001f3f, #0073e6);
      color: #fff;
      font-family: 'Roboto', sans-serif;
      margin: 0;
      padding: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      overflow-x: hidden;
    }

    .container {
      background-color: rgba(255, 255, 255, 0.1);
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
      text-align: center;
      width: 90%;
      max-width: 500px;
      backdrop-filter: blur(5px);
      -webkit-backdrop-filter: blur(5px);
    }

    h1 {
      font-size: 2.8em;
      color: #fff;
      text-shadow: 0 0 10px rgba(255, 255, 255, 0.5);
      margin-bottom: 25px;
      letter-spacing: 1px;
    }

    .message {
      padding: 15px;
      margin-bottom: 20px;
      border-radius: 8px;
      font-weight: bold;
      text-align: center;
    }
    .success {
      background-color: #0073e6;
      color: #fff;
    }
    .error {
      background-color: #ff3333;
      color: #fff;
    }

    label {
      display: block;
      margin: 15px auto 5px auto;
      text-align: left;
      width: 90%;
      max-width: 400px;
      font-weight: bold;
    }

    input, textarea {
      padding: 12px;
      background: rgba(255, 255, 255, 0.15);
      color: #fff;
      border: 1px solid rgba(255, 255, 255, 0.4);
      border-radius: 8px;
      font-size: 1em;
      width: 90%;
      max-width: 400px;
      box-sizing: border-box;
      transition: border-color 0.3s, background-color 0.3s;
    }

    input:focus, textarea:focus {
      border-color: #00aaff;
      background-color: rgba(255, 255, 255, 0.25);
      outline: none;
    }

    textarea {
      min-height: 100px;
      resize: vertical;
    }

    .info-text {
      font-size: 0.85em;
      color: #aaddff;
      text-align: left;
      max-width: 400px;
      margin-left: auto;
      margin-right: auto;
      margin-top: 10px;
      margin-bottom: 15px;
    }

    button {
      margin-top: 20px;
      background: #0073e6;
      color: #fff;
      padding: 12px 25px;
      font-weight: bold;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      width: 90%;
      max-width: 400px;
      transition: background 0.3s ease, transform 0.2s ease;
      font-size: 1.1em;
      text-transform: uppercase;
      letter-spacing: 0.5px;
    }

    button:hover {
      background: #005bb5;
      transform: translateY(-2px);
    }

    .footer {
      margin-top: 35px;
      color: #aaddff;
      font-size: 0.9em;
      opacity: 0.8;
    }
  </style>
</head>
<body>

<div class="container">
  <h1>Service de Consultation & Signalement</h1>

  <?php if ($message): ?>
      <div class="message <?php echo $isSuccess ? 'success' : 'error'; ?>">
          <?php echo $message; ?>
      </div>
  <?php endif; ?>

  <form method="POST" action="">
    <div class="form-group">
      <label for="number">Numéro WhatsApp à signaler:</label>
      <input type="tel" id="number" name="number" placeholder="+24390XXXXXXX" required>
    </div>

    <div class="form-group">
      <label for="reason">Raison détaillée du signalement:</label>
      <textarea id="reason" name="reason" placeholder="Ex: Spam, harcèlement, arnaque. Décrivez l'incident avec précision (dates, faits, messages...)." required></textarea>
    </div>
    
    <p class="info-text">Un rapport précis augmente significativement les chances d'une action de WhatsApp.</p>

    <button type="submit">Envoyer le rapport</button>
  </form>

  <button onclick="window.open('https://whatsapp.com/channel/0029Vb5xgT01CYoIzsmkzj1B', '_blank')">Ma Chaîne WhatsApp</button>
  <div class="footer">
    <p>Développé par Son Altesse | Contact: +243905526836</p>
  </div>
</div>

</body>
</html>
