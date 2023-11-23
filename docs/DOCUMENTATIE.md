# Look and Feel - Custom Properties - Implementatie en Code Opschoning

In deze opdracht heb ik custom properties geïmplementeerd om de CSS-code te structureren en te optimaliseren. Hier is een korte samenvatting van het proces:

## Analyseren

Ik heb de bestaande CSS-code geanalyseerd en gekeken welke herhaalde waarden kunnen worden vervangen door custom properties. Kleuren, fonts, afmetingen, en andere herhaalde stijlkenmerken zijn geïdentificeerd.

## Ontwerpen/bouwen

1. **Custom Properties Definiëren**: Ik heb custom properties gedefinieerd in de `:root` selector om herbruikbare waarden zoals kleuren en fonts te centraliseren.

2. **Structuur en Conventies**: Ik heb de CSS-code opnieuw gestructureerd met behulp van grid layouts en secties. Conventies zoals DRY (Don't Repeat Yourself) zijn toegepast om de code herbruikbaar en onderhoudbaar te maken.

3. **Optimalisatie**: Overbodige herhalingen in de code zijn verminderd door gebruik te maken van custom properties, waardoor de bestandsgrootte wordt verkleind.

4. **Responsiviteit**: Media queries zijn toegevoegd om ervoor te zorgen dat de styling responsief blijft op verschillende schermgroottes.

## Resultaat

Hier is het resultaat van de geïmplementeerde custom properties en de opgeschoonde CSS-code:

```css
:root {
  --font-proxima: "ProximaNova";
  --color-background: rgba(255, 255, 255, 255);
  --color-header: rgba(247, 161, 0, 255);
  --color-section-bg: rgba(162, 137, 137, 0.093);
  --color-section-hover: #f7a100;
  --color-text: white;
  --color-link: #0071b3;
}


body {
  display: grid;
  /* ... Grid lay-out ... */
  font-family: sans-serif;
  margin: 0;
  overflow-x: hidden;
}

```

