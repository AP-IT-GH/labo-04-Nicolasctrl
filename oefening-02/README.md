Maak het afbeeldingsbestand in bijlage na. Gebruik de juiste HTML-elementen en volg de eerder gemaakte afspraken.

Hier moet je een genummerde lijst gebruiken. De bullets zouden automatisch genummerd moeten zijn, de tekst van de lijstitems (bijvoorbeeld "Item 1") mag je wel zelf invullen.

Gebruik de `:even` en `:odd` pseudoklassen om verschillende stijlen toe te passen op even en oneven genummerde items in de lijst.
_______________
index.html     |
_______________|

<!DOCTYPE html>
<html lang="nl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Even en oneven items lijst</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <h1>Even en oneven items lijst</h1>

    <ol>
        <li>Item 1</li>
        <li>Item 2</li>
        <li>Item 3</li>
        <li>Item 4</li>
        <li>Item 5</li>
    </ol>

</body>
</html>
_______________
style.css      |
_______________|

body {
    font-family: Arial, sans-serif;
    margin: 50px;
}

h1 {
    font-size: 32px;
    font-weight: bold;
    margin-bottom: 30px;
}

ol {
    list-style-type: decimal;
    padding-left: 0;
    width: 300px;
    border: 1px solid #ccc;
}

ol li {
    padding: 10px;
    font-size: 18px;
    border-top: 1px solid #ccc;
}

/* Stijl voor ONEVEN items (1, 3, 5, ...) */
ol li:odd {
    background-color: white;
    color: #007bff; /* Blauwe tekstkleur, vergelijkbaar met de afbeelding */
}

/* Stijl voor EVEN items (2, 4, 6, ...) */
ol li:even {
    background-color: #f0f0f0; /* Lichtgrijze achtergrond */
    color: black;
}

/* Verwijder de bovenste rand van het eerste element, want de rand zit al op de OL */
ol li:first-child {
    border-top: none;
}
