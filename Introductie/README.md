# I. Introductie

Deze scriptie zal een beschrijving geven van het project, ontwikkeld tijdens een driemaandelijkse stage bij CTG Belgium NV/SA.

<div id="stagebedrijf"></div>

### 1.1 Stagebedrijf

CTG - Computer Task Group - is een IT service provider met kantoren in Belgi&euml;, Luxemburg, het Verenigd Koninkrijk en meerdere locaties in Noord-Amerika. Zij vieren dit jaar hun 50e verjaardag na hun oprichting in 1966.

CTG biedt in Belgi&euml; IT services aan in 6 hoofdzakelijke categorie&euml;n: Application Solutions (AS), IT Service Management (ITSM), Regulatory Compliance, Healthcare Services, Management Consultancy en Testing.
AS wordt verder onderverdeeld in enkele subcategorie&euml;n, waaronder Mobile Web Development. Het stageproject verliep binnen deze laatste categorie.

<div id="situering"></div>

### 1.2 Situering

Het stageproject zou een applicatie worden voor de CTG Experience Day (XPDay), dat zal doorgaan op 27 oktober in 'De Montil', te Affligem. Alvorens verder in te gaan op de applicatie is het handig om te weten wat deze Experience Day inhoudt.

> De **[Excperience Day](https://experienceday.ctg.com/home)** is een jaarlijkse conferentie, georganiseerd door CTG, waarbij het bedrijf zijn ervaringen en *best practices* deelt met zijn klanten, interne specialisten en partners. Hiervoor zullen meer dan 40 presentaties en workshops voorzien worden, ook samengesteld door de klanten, interne specialisten en partners. Deze presentaties en workshops delen een kern van vier grote thema's: Data, Apps, Security en Methodologie&euml;n.




<div id="opgave"></div>

## 1.3 Opgave

Bij aanvang van de stage was de organisatie van de Experience Day nog niet op gang gezet. Tijdens het verloop van de stage en voornamelijk in het begin, waren dus nog niet alle factoren bekend. Hierdoor zijn er enkele vereisten opgesteld die passen binnen een standaard conferentie applicatie. In de loop van het project zijn er prioriteiten gesteld en veranderd. Er zijn echter ook enkele kernelementen die onveranderd blijven doorheen het project zoals het type applicatie en de gebruikte technologie.

#### 1.3.1 Mobiele applicatie
Bij een conferentie met meer dan 40 presentaties en workshops is een effici&euml;nt overzicht meer dan welkom. Informatie hieromtrent en omtrent andere praktische zaken zoals locatie en presentatoren, moet gemakkelijk toegankelijk zijn voor de genodigden. Deze informatie zal in de eerste plaats beschikbaar zijn op de Experience Day website. Om de informatie sneller raadpleegbaar te maken en ook offline aan te bieden, is een mobiele applicatie passend. 

Voor de Experience Day app is het niet nodig om en speciaal design voor tablets te voorzien. Het design voor smartphones volstaat, echter wel rekening houdend met verschillende resoluties.

#### 1.3.2 Hybride applicatie
Op een conferentie heeft natuurlijk niet iedereen dezelfde smartphone. Wanneer we kijken naar het marktaandeel van de verschillende operating systems (OS), zien we dat Android ongeveer 63% van de markt bezet en iOS ongeveer 30%. Windows Phone staat op een kleine 3%. We kunnen dus veronderstellen dat voornamelijk mensen met Android en iOS smartphones aanwezig zullen zijn op de conferentie. Het zal dus een voordeel zijn om een mobiele applicatie te maken die voor beide platformen beschikbaar is. Het zou dubbel werk zijn als we voor beide platformen een aparte applicatie zouden schrijven: eenmaal in Swift of Objective C voor iOS en eenmaal in Java voor Android. Voor dit project is er 
dus gekozen voor een hybride applicatie.

Een hybride applicatie worden gemaakt met dezelfde bouwstenen als bij een website: HTML, CSS en JavaScript. Dit zorgt er voor dat men met &eacute;&eacute;n eenvoudige taalset kan werken. De leercurve hiervoor ligt aanzienlijk lager dan die voor bijvoorbeeld Swift en Java tezamen. Bovendien kan er gebruik worden gemaakt van een gigantisch aanbod aan plugins, frameworks, packages et cetera. 

Verder laten hybride applicaties het ook toe om gebruik te maken van native functionaliteiten. Native functionaliteiten zijn zaken zoals de microfoon, camera, qr-scanners, native pop-ups enzovoorts.

#### 1.3.3 Versie 2
In 2015 werd er een mobile/web klas georganiseerd. Hierbij worden er presentaties en opleidingen gegeven over allerhande nieuwe technologieën en algemene kennis. Op het einde van deze opleiding werd er tijd voorzien om een project te ontwikkelen waarbij de nieuwe kennis gebruikt kon worden. Hierbij hebben enkele mensen samengewerkt om een applicatie te maken voor de Experience Day editie van 2015. Deze editie heeft niet kunnen plaats vinden wegens omstandigheden en deze applicatie is dus nooit in gebruik genomen.

Dit project zal gebruik maken van nieuwere technologie. De bestaande applicatie kan echter wel als referentie gebruikt worden voor enkele vereisten. 

#### 1.3.4 Technologie
Zowel voor onderzoeksdoeleinden in verband met de stage als voor CTG is het interessant om nieuwe technologie te gebruiken voor de applicatie. Door gebruik te maken van nieuwe *frameworks* laat CTG zien aan zijn klanten dat men gebruik maakt van de nieuwste beschikbare elementen op de markt. Verder is het tijdens de stage een buitenkans om *hands-on* ervaring op te doen met deze nieuwigheden en er veel over te leren. 

De nieuwe technologie&euml;n waarvoor gekozen is, zijn Ionic 2, gecombineerd met Angular 2 en Typescript. In het hoofdstuk [2.1.1 Technologie](../Technisch/README.md#technologie) hierover meer.

#### 1.3.5 Evaluatie
Een belangrijk element van de applicatie zal een evaluatieformulier zijn. Dit formulier is erop gericht informatie te verzamelen over het verloop van de sessies en hoe de bezoekers deze ervaren hebben. Deze evaluaties zullen gebruikt worden om feedback te verzamelen en zo de toekomstige Experience Days mogelijk te verbeteren.

In vorige edities van de Experience Day werden deze formulieren nog op papier afgedrukt, uitgedeeld en verzameld in een brievenbus. In een IT Service bedrijf zijn de middelen - indien beschikbaar - aanwezig om dit te voorzien in een digitale vorm. Het is positief om aan klanten en partners aan te tonen dat zij dit kunnen verwezenlijken op een dergelijke wijze.

<div id="vereisten-in-scope"></div>

#### 1.3.6 Vereisten in scope
Om een richtlijn te hebben zijn er toch enkele *requirements* opgesteld en vastgelegd. Hieronder de vereisten die vallen binnen de scope van de stageperiode:

* Het gaat hier om een mobile app. Er moet geen speciale aandacht worden besteed aan tablets.
* Deze moet uiteindelijk beschikbaar zijn in de Google Play Store en de Apple App Store. Dit wil dus zeggen dat de applicatie zowel voor Android als iOS beschikbaar moet zijn.
* Belangrijke informatie moet offline beschikbaar zijn. Dit gaat over volgende info: thema's, sessies, tijdstippen, sprekers, algemeen CTG, deelnemers, sponsors en de locatie (floorplan, parking en route).
* Men moet de agenda kunnen bekijken van de Experience Day. Hierbij horen begin- en einduren van sessies.
* Men moet een persoonlijke agenda kunnen opstellen voor sessies die zij wensen bij te wonen.
* Hiervoor moet men ook kunnen inloggen met een persoonlijke account.
* Er moet een evaluatieformulier per sessie ingevuld kunnen worden.
* *Branding*: Het moet duidelijk zijn dat de app van CTG komt. Dit impliceert dus duidelijk gebruik van het Experience Day logo en gebruik van het *CTG-groen*.
* De applicatie zal gemaakt worden aan de hand van nieuwe technologie.


#### 1.3.7 Vereisten buiten scope
Omdat de stage beperkt is in tijd en de deadlines van de Experience Day ergens in Augustus 2016 liggen, zijn er een aantal variabele factoren die buiten het domein van de stage vallen. De ontwikkeling van de Experience Day website staat los van het stageproject. Op deze website zullen enkele belangrijke zaken worden afgehandeld die veelbepalend zijn. Naast de website zullen veel gegevens in verband met de Experience Day zullen op een server in de Verenigde Staten terecht komen. Dit zal dezelfde server zijn waar de website en gegevens van de vorige Experience Day op stonden.

De Experience Day is enkel voor mensen die uitgenodigd zijn. Elke genodigde zal 20 dagen voor de XPDay een uitnodiging ontvangen, waarschijnlijk via email, met een username en eventueel een toegewezen wachtwoord. Deze login gegevens zullen de genodigden kunnen gebruiken om zich aan te melden op de website en de mobiele applicatie. De login gegevens en persoonlijke agenda's die de gebruikers samenstellen op de website of in de applicatie zullen worden opgeslagen op deze server. Verder zullen ook de evaluatieformulieren op dezelfde server terecht komen.

