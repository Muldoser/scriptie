# III. Conclusie

<div id="resultaten"></div>

## 3.1 Resultaten

<div id="Project"></div>

#### 3.1.1 Project

Het doel van dit project was een hybride, mobiele applicatie voor de CTG Experience Day. Dit met behulp van Ionic 2, Angular 2 en TypeScript. Belangrijke punten waren de offline beschikbaarheid van informatie en de evaluatieformulieren voor de verschillende sessies en workshops die gegeven zullen worden.

Verdere vereisten, beschreven in [1.3.6 Vereisten in scope](../Introductie/README.md#vereisten-in-scope) waren:

* Het gaat hier om een mobile app. Er moet geen speciale aandacht worden besteed aan tablets.
* Deze moet uiteindelijk beschikbaar zijn in de Google Play Store en de Apple App Store. Dit wil dus zeggen dat de applicatie zowel voor Android als iOS beschikbaar moet zijn.
* Belangrijke informatie moet offline beschikbaar zijn. Dit gaat over volgende info: thema's, sessies, tijdstippen, sprekers, algemeen CTG, deelnemers, sponsors en de locatie (floorplan, parking en route).
* Men moet de agenda kunnen bekijken van de Experience Day. Hierbij horen begin- en einduren van sessies.
* Men moet een persoonlijke agenda kunnen opstellen voor sessies die zij wensen bij te wonen.
* Hiervoor moet men ook kunnen inloggen met een persoonlijke account.
* Er moet een evaluatieformulier per sessie ingevuld kunnen worden.
* *Branding*: Het moet duidelijk zijn dat de app van CTG komt. Dit impliceert dus duidelijk gebruik van het Experience Day logo en gebruik van het *CTG-groen*.
* De applicatie zal gemaakt worden aan de hand van nieuwe technologie.


Deze elementen zijn allemaal verwezenlijkt. De Experience Day App is mobile en is beschikbaar voor zowel Android, als iOS. De nodige informatie wordt offline aangeboden. Men kan de planning van de Experience Day raadplegen en hierbij een persoonlijke agenda opstellen. Het is mogelijk om in te loggen, echter wel zonder bestaande login gegevens. De belangrijke formulieren voor de evaluatie van de sessies zijn aanwezig en functioneel. De logo's en vooral de kleuren van CTG zijn rijkelijk aanwezig in het algemene thema. Dit alles is ontworpen met de voorafbepaalde technologie.


<div id="opmerkingen"></div>

#### 3.1.2 Opmerkingen

In de loop van het project was het grootste struikelblok het alpha/beta-gedeelte in het Ionic verhaal. Ionic 2 was bij aanvang van het project in alpha. De veranderingen die soms doorgevoerd werden konden er soms voor zorgen dat bepaalde zaken niet meer werkten zoals voordien. De aanpassingen van de ionic releases doortrekken naar het XPDay project nam soms veel tijd in beslag.

Langs de andere kant van het verhaal, is het een voordeel om de groei van het framework van dichtbij te volgen. Zo kan er opgemerkt worden dat de documentatie aanzienlijk verbeterd is en veel uitgebreider is gemaakt.

Een laatste opmerking draait rond de mobile web klas. De lessen namen redelijk wat tijd van het project in beslag. De voorbereiding van de lessen en het volgen van de andere cursussen liet weinig ruimte voor werk aan de XPDay App. Los daarvan blijft het een bonus om deze lessen te hebben mogen volgen. De klas nam veel tijd in beslag, maar de applicatie heeft de voornaamste features bereikt. Ook de kans om les te geven en de *presentation skills* bij te schaven compenseert voor de tijd die in de opleiding is gekropen.


<div id="feedback"></div>

#### 3.1.3 Feedback Mobile Web klas

Voor de mobile web klas was er een les voortgekomen uit dit project. Hiervoor zijn resultaten via mail teruggekomen van zij die de lessen hebben bijgewoond.

* **Angular 2 & Ionic 2 introductie**
    - *Trainer*: Michiel Mulder
    - *Score content*: 8/10
    - *Feedback content*:

    > Presentatie over Ionic(2), praktische demo en dan verder een oefenproject in verband met Angular 2 (die gebruikt word in Ionic 2).  Presentatie & praktische demo was duidelijk.  Oefenproject was zeer leerrijk maar zelfstudie is in onze mening niet de meest ideale manier om bij te leren (dit kunnen we ook in de bench).  De kwaliteit van de oefening (Heroes) was zeker hoog genoeg maar we hadden sommige dingen toch liever klassikaal gedaan. Van nul af samen alles opgebouwd.
    > De oefening die we kregen was ook onmogelijk af te maken op de tijd die we kregen zonder voorkennis.

    - *Score trainer*: 8/10
    - *Feedback trainer*:
    > Hij was vlot en duidelijk.  Kon vlot helpen met vragen die gesteld werden.  

* **Ionic 2** 
    - *Trainer*: Michiel Mulder
    - *Score content*: 8/10
    - *Feedback content*:
    > In navolging van woensdag, meer les over Ionic en oefenproject.  Gaf ons goed overzicht van het gebruik van Ionic 2, een goeie en duidelijke demo van hoe een project op te zetten.  Hoe de structuur in elkaar zit.  Design & thema’s aanpassen.  Zeer compleet maar we hebben hier zeker nog meer oefening op nodig om dit praktische te kunnen gebruiken.

    - Score trainer: 8.5/10
    - Feedback trainer:
    > Hij was vlot en duidelijk.  Kon vlot helpen met vragen die gesteld werden.  Het was duidelijk dat hij al heel wat praktische kennis van Ionic2 en kon dit ook makkelijk demonstreren. 

<div id="uitbreiding-en-toekomst"></div>

## 3.2 Uitbreidingen en toekomst

#### 3.2.1 Overname

De applicatie is bij het be&euml;indigen van de stage overgedragen aan Younes Kichouh en Karim Dehbi. Zij zullen de applicatie verder afwerken opdat deze gebruiksklaar zal zijn op 27 oktober en de weken daarvoor. Zij zullen nog moeten samenzitten met de ontwikkelaar van de website en backend om samen de data te kunnen gebruiken vanop de server. De persoonlijke agenda's zullen extern worden opgeslagen, zodat de gebruikers deze zowel op de website als in de applicatie kunnen bekijken en bewerken. De gegevens van de evaluaties zullen ook naar de server gecommuniceerd moeten worden. Hierbij moet nog beslist worden wat er verder met deze evaluaties gaat gebeuren.


<div id="twitter"></div>

#### 3.2.2 Twitterfeed

De twitterfeed is een leuke feature omdat mensen zo live in de Experience Day app kunnen volgen wat er over de Experience Day (#XPDay) wordt getweet. Hiervoor is er in de laatste week van de stageperiode de API boven komen drijven die vorig jaar werd gebruikt. Deze is in samenwerking met Wout De Rooms aangepast geweest en dus klaar om voor de editie van 2016 te gebruiken.
De API gaf correcte JSON data terug, dus de volgende en enige stap die (normaal gezien) nu nog genomen zou moeten worden is een view die deze JSON data juist weergeeft.

#### 3.2.3 Puntensysteem

Om de bezoekers te motiveren bestaat het idee om punten te geven per ingevuld formulier. Wanneer de gebruiker genoeg punten verzameld heeft zou deze een goodybag kunnen afhalen bij de balie. Hiervoor zou ook de QR-code scanner goed van pas komen, om bijvoorbeeld op het einde van de presentatie te scannen en zo de evaluatie te valideren. Dit laatste is om te voorkomen dat mensen snel enkele willekeurige evaluaties invullen om zo hun goodybag te winnen.