# OmroepflevoS6G2
Welkom bij de ReadMe van Groep 2 Semmester 6. We lichten hieronder de functies van de code toe. Het project is gebaseerd op het Vue-framework.

## index.js
Dit is het document voor de Vue-router. Deze handelt navigatie in de website af en zorgt ervoor dat hier geen reloads nodig zijn.

## Views
Vue werkt met Views waar de router naartoe linkt. 

## SubContentViews
We maken gebruik van sub-navigatie: een navigatiebalk binnen een View. De Views hiervoor tref je in deze map.

## StoryView
Dit is de View waar alles betreffende story's zich huisvest. Hier tref je een navigatiebalk en een routerview waar de verschillende pagina's binnen deze view worden weergegeven.

## NewStoryView
Dit is de View waar je een nieuwe story aan kunt maken. Hier tref je in de HTML de invoervelden, die we afvangen met de consoleLog-methode. Deze data wordt verzonden naar de Firebase-database, waarna de velden geleegd worden. De gebruiker krijgt na het verzenden een melding in beeld.

## StoriesView
Dit is de View waar de gebruiker de aangemaakte story's treft. Dit gebeurt real time. In de Created-hook van Vue wordt de data uit de database op het moment dat de website aangemaakt is, opgehaald en in een lokale array weggeschreven. De functies die de Created()-functie aanroept, zijn Firebase-functies, verversen wanneer de database wordt aangepast. In deze zelfde functie wordt de timestamp geïntialiseerd.

De zoekbalk werkt door de uitVoerZoekOpdracht-functie, die aan de Computed-hook vastzit. Deze luistert naar wijzigingen van de DOM, en wordt dan uitgevoerd.
