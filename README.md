# AI Persona Quiz

Dit project is een eenvoudige webapplicatie die een quiz aanbiedt om inzicht te krijgen in uw persoonlijke AI-profiel. De quiz is gebaseerd op onderzoek van Slack’s Workforce Lab en maakt onderscheid tussen vijf AI-persona’s. Door het invullen van de quiz en het vergelijken van resultaten met collega’s, kunt u beter inzicht krijgen in de diverse behoeften, verwachtingen en motivaties rondom AI-gebruik op de werkvloer.

## Overzicht

- **Vijf AI-persona’s**
  De quiz maakt gebruik van vijf persona’s: **Maximalist**, **Underground**, **Rebel**, **Superfan** en **Observer**. Elk van deze persona’s weerspiegelt een specifieke houding ten opzichte van het gebruik van AI in een professionele omgeving.

  - 🥰 **The Maximalist** - All-in op AI en al profiteren van de voordelen.
  - 🤫 **The Underground** - Gebruikt AI discreet en is terughoudend om het met collega's te delen.
  - 😎 **The Rebel** - Ziet AI als een bedreiging en rebelleert tegen de AI-hype.
  - 🤩 **The Superfan** - Enthousiast over AI maar juicht vanaf de zijlijn.
  - 🧐 **The Observer** - Onverschillig tegenover AI, maar volgt de ontwikkelingen met interesse en voorzichtigheid.

- **Onderbouwing**
  Het idee is geïnspireerd door een onderzoek van Slack’s Workforce Lab, dat zich richtte op het in kaart brengen van werkmotivaties, AI-vaardigheden en AI-enthousiasme onder kantoormedewerkers.

- **Doel van de quiz**
  Het resultaat van de quiz laat zien welke AI-persona u het meest waarschijnlijk vertegenwoordigt. Door deze inzichten te delen met uw team of afdeling kunnen organisaties beter inspelen op diverse AI-behoeften en -kansen.

## Functies en Kenmerken

- **Likert Scale- en meerkeuzevragen**
  Sommige vragen bevatten een 5-punts Likert-schaal (1 = Helemaal oneens, 5 = Helemaal eens), terwijl andere vragen meerkeuze of meerdere-selectievragen gebruiken.

- **Automatische scoreberekening**
  Aan elk antwoord zijn punten voor specifieke persona’s gekoppeld. Wanneer de quiz wordt ingeleverd, worden de punten opgeteld om de dominante persona(’s) te bepalen.

- **Resultaatweergave en persona-omschrijving**
  De resultaten worden direct op de pagina getoond, inclusief een korte beschrijving van uw (top)persona(’s) en een horizontale staafdiagram met de puntenscore voor elke persona.

- **PDF-generator**
  U kunt een persoonlijke rapportage downloaden in PDF-formaat. De rapportage bevat de volgende informatie:
  - Uw voornaam (privacyvriendelijk)
  - Uw persona-resultaten en totale scores
  - Een korte achtergrond van het onderzoek en de gebruikte persona’s
  - Uw antwoord op de vraag hoe uw organisatie AI ondersteunt

## Installatie en Gebruik

1. **Download of clone deze repository**

2. **Open de quiz**
   - Open het bestand `index.html` (of de HTML-bestandsnaam in de repo) in uw webbrowser.
   - Alle nodige scripts en CSS worden via CDN geladen, dus er is geen extra installatie vereist.

3. **Vul de quiz in**
   - Vul alleen uw voornaam in (privacy) en beantwoord alle vragen.
   - Klik op **Resultaten Berekenen** om uw score en persona-resultaat te bekijken.

4. **Download rapport**
   - Na het bekijken van uw resultaten kunt u de rapportage genereren door te klikken op **Download PDF rapport**.

5. **Opnieuw beginnen**
   - Klik op **Opnieuw beginnen** om het formulier te resetten en de quiz opnieuw in te vullen.

## Structuur van de Code

- **HTML**
  De quiz, vragen, en UI-elementen staan in één bestand (`index.html`), waardoor de applicatie direct in de browser te gebruiken is.

- **JavaScript-modules**
  - **QuizData**: Bevat de quizvragen en de persona-logica.
  - **PersonaDescriptions**: Beschrijvingen van de vijf AI-persona’s.
  - **QuizRenderer**: Genereert dynamisch de vragen en het formulier in de DOM.
  - **QuizValidator**: Controleert of alle vragen zijn beantwoord en valideert de invoer.
  - **QuizCalculator**: Berekent de scores per persona en bepaalt de dominante persona(’s).
  - **ResultRenderer**: Toont de eindresultaten op het scherm en maakt de staafdiagram.
  - **PDFGenerator**: Maakt een rapport in PDF-formaat, met behulp van de bibliotheek `html2pdf.js`.
  - **QuizController**: Coördineert de quizlogica en initieert het renderen en valideren.

## Bron en Referentie

- Slack. (n.d.). [*AI team-building with the AI persona quiz*](https://slack.com/blog/transformation/ai-team-building-with-the-ai-personas-quiz). Slack. Geraadpleegd op 4 februari 2025.

## Contributies

- Pull requests, bugmeldingen en suggesties zijn van harte welkom.
- Voel u vrij om deze code te forken of te klonen en aan te passen voor eigen gebruik.

## Licentie

Dit project is vrij te gebruiken en aan te passen. Het kan echter verwijzingen of content bevatten die onderhevig zijn aan rechten van derden (zoals Slack). Controleer altijd zelf de licentievoorwaarden van externe bronnen of voorbeelden.
