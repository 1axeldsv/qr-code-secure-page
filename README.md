# qr-code-secure-page
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Demande de code</title>
</head>
<body>
    <h2>Entrez le code secret : (Un indice ? 🗼🗼)</h2>
    <form id="codeForm">
        <input type="text" id="codeInput" placeholder="Code secret">
        <button type="submit">Soumettre</button>
    </form>

    <script>
        document.getElementById('codeForm').addEventListener('submit', function(event) {
            event.preventDefault();
            var codeSaisi = document.getElementById('codeInput').value;
            // Vérifiez ici si le code saisi est correct
            if (codeSaisi === '11/09/2019') {
                window.location.href = 'page_image.html'; // Redirection vers la deuxième page si le code est correct
            } else {
                alert('Code incorrect. Veuillez réessayer.');
            }
        });
    </script>
</body>
 Un indice ? 🗼🗼
</html>
