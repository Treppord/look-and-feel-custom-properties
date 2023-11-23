# Look and Feel - Custom Properties - Implementatie en Code Opschoning

In deze opdracht heb ik custom properties geïmplementeerd om de CSS-code te structureren en te optimaliseren. Hier is een korte samenvatting van het proces:

## Analyseren

Ik heb de bestaande CSS-code geanalyseerd en gekeken welke herhaalde waarden kunnen worden vervangen door custom properties. Kleuren, fonts, afmetingen, en andere herhaalde stijlkenmerken zijn geïdentificeerd.

## Ontwerpen/bouwen

1. **Custom Properties Definiëren**: Ik heb custom properties gedefinieerd in de `:root` selector om herbruikbare waarden zoals kleuren en fonts te centraliseren.

2. **Structuur en Conventies**: Ik heb de CSS-code opnieuw gestructureerd met behulp van grid layouts en secties. Conventies zoals DRY (Don't Repeat Yourself) zijn toegepast om de code herbruikbaar en onderhoudbaar te maken.

3. **Optimalisatie**: Overbodige herhalingen in de code zijn verminderd door gebruik te maken van custom properties, waardoor de bestandsgrootte wordt verkleind.

4. **Responsiviteit**: Media queries zijn toegevoegd om ervoor te zorgen dat de styling responsief blijft op verschillende schermgroottes.


## Structuur

Zoals bij Resultaat te zien is, heb ik nu een aantal custom properties gemaakt.
De color-background, -header etc zijn geimplementeerd om de kleuren van de website simpel bij te houden en evt toekomstig een darkmode toe te voegen.

Ik heb de kebab-case methode gebruikt omdat ik daar simpelweg het meeste aan gewend ben. En daardor dus universeel al toe pas.

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

@font-face {
  font-family: var(--font-proxima);
  src: url(../assets/Fonts/ProximaNova-Regular_2607783814[2260].otf);
}



@media (min-width: 1125px) {
  body {
    background-color: var(--color-background);
    display: grid;
    grid-template-columns: 2fr 3fr 0.5fr 3fr 2fr;
    grid-template-rows: 0.5fr 0.25fr 0.25fr 0.25fr 0fr 0.25fr 1fr 1fr;
    grid-gap: 0.5rem;
    grid-template-areas:
      "header header header header header"
      ". h1 h1 h1 ."
      ". sec1 . sec2 ."
      ". sec3 . sec4 ."
      ". div div div ."
      ". h2 h2 h2 ."
      ". sec5 . sec7 ."
      ". sec6 . sec8 .";
    font-family: sans-serif;
    margin: 0;
  }

```

