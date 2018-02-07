# Portfolio_kb-74
Welkom op mijn Portfolio. Deze portfolio heb ik gemaakt gedurende het blok KB-74. In de portfolio heb ik mijn uitgevoerde taken opgenomen.

De initiële afspraak die is gemaakt met docenten was dat iedere portfolio om de 4 weken feedback zou ontvangen. Echter is in week 15/16 feedback gegeven die niet diepgaant was en geen extra toevoeging gaf op wat er in de portfolio dient te worden toegevoegd naast de minimalistische beoordelingslijst.

--------------------------------------------------------------------------------
## KB-74
De minor kb-74 gaat over "Applied Data Science". In deze minor is de nadruk gelegt op het onderwerp "Machine learning". In deze minor hadden we keuze uit 4 projecten. Aan de start van de minor heb ik gewerkt in de groep EM-Fields waarin ik onderzoek heb uitgevoerd over elektromagnetische straling. Echter werdt deze groep opgeheven aan het eind van week 3 vanwege een te grote druk bij de begeleidend docent. Ik heb in week 4 een nieuw projectgroep moeten kiezen om mijn minor voort te zetten. In die tijd heb ik gekozen voor het project Urbinn.

Het project Urbinn focust zich op het onderdeel "Autonoom rijden" met nadruk op het maken van een "Semantische kaart". Om nog specifieker te zijn moest er een semantische kaart worden gemaakt van de omgeving Delft. Deze kaart dient om de omgeving van de route vast te leggen. Deze kaart van de omgeving zal dan later weer gebruikt worden door het voertuig van Urbinn om te navigeren door het stedelijke gebied.

## Mijn portfolio
In mijn portfolio zijn de volgende onderdelen te vinden:

 - De door mij gegeven presentaties
 - Codes die ik geschreven en/of aangepast heb
 - Screenshots van Datacamp en Coursera
 - Scrum tickets waar ik aan gewerkt heb
 - Uitgelichte onderwerpen
 - Workshop opdrachten
 
In week vier van het blok heb ik mij samengevoegt in de groep Urbinn. In die tijd was er al vooronderzoek uitgevoerd over de basis van het project en welke richitng het project op ging. Ik heb het vooronderzoek doorgelezen zodat ik de stof begreep en met de rest verder kon werken.

Het werdt duidelijk voor me dat het maken van een semantische map meerdere onderdelen nodig zijn. een paar van deze onderdelen zijn:
 - Beeldmateriaal
 - Geclassificeerde objecten
 - Ruimtelijke kaart

Naar aanleiding van mijn achtergrond hebik mij meer gericht op het maken van plannen voor het vergaren van informatie en het uitvoeren van evaluaties.

Voor het genereren van beeldmateriaal was stereo beeld benodigd. Door het gebruik van stereobeelden was het mogelijk om niet alleen beter putnen te herkennen maar ook om beter diepte te bepalen. De informatie die opgehaald moest worden was ook deels de "Ground-truth". De ground truth is erg belangrijk voor het project om de progressie te evalueren en te kijken hoe goed het product (semantische map) is tegenover de ground-truth.

In samenwerking met groepsgenoten heb ik onderzoek uitgevoerd voor manieren om ons product te evalueren. Hier hebben we wat methodes gevonden, waarvan wij dachten, toepasbaar zijn.

Een van deze methodes is het vergelijken van pointclouds. Een pointcloud is een map gemaakt uit punten die zijn geïdentificeerd en gevisualiseerd door een programma zoals ORB-Slam2. Deze pointcloud plaats je over de pointcloud dat de ground-truth dient te zijn en hier kijkt of er verschillen aanwezig zijn om de accuraatheid te meten. Dit heb ik samen met Isa uitgevoerd.
![ORB-Slam2](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Plaatjes/ORBSlam2.png)

Tussentijds heb ik de groep geholpen met kleine taken zoals het controleren van papers, documenten, het meedenken over oplossingen voor code.

Samen met Viradj heb ik geholpen met het maken van beeldmateriaal voor de groep. Voor het maken van dit beeldmateriaal hebben we een trolly gebruikt met mij erop terwijl ik een laptop en camera vathield. Hierdoor hebben we camera opnames gemaakt van twee kleine routes vlak bij de Haagse Hogeschool.
[Klik hier voor een afbeelding hoe de opnames HHS werden uitgevoerd](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Plaatjes/opnameshhs.jpg)

Samen met Nektarios, Kevin en Viradj heb ik meer dan 500 foto's gelabeld. Iedere foto bevatte gemiddeld meer dan 15 verschillende objecten die gelabeld moesten worden zodat we het programma YOLO verder konden trainen om overfitting te voorkomen. Chris heeft hier later een testrun overheen laten lopen.
![Testrun KITTI](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Plaatjes/KITTIYolo.png)



---------------------------------------------------------------------------------
## Algemene onderdelen
### [Datacamp](https://github.com/BobvanElburg/Portfolio_kb-47/tree/master/Datacamp)
Voor de minor is de vraag naar kennis over de codetaal Python. Het is lastig om hiervan de voortgang vast te leggen. Ik probeer zoveel mogelijk informatie vast te leggen om mijn voortgang te laten zien.

Voor datacamp heb ik de volgende courses gemaakt en afgerond.

* Intro to Python for Data Science
* Intermediate Python for Data Science
* Python Data Science Toolbox (Part 1)
* Pandas foundation
* Python Data Science Toolbox (Part 2)
* Introduction to data visualization with Python
* Cleaning Data
* Statistical Thinking in Python (part 1)
* Supervised Learning with scikit-learn

Ik vond de Python courses erg leuk maar wel tijdrovend. Vooral omdat het project zoveel tijd vereist blijft er weinig tijd over om zelf opdrachten uit te voeren.

### [Coursera](https://github.com/BobvanElburg/Portfolio_kb-47/tree/master/Coursera)
Tijdens de minor is geavanceerde wiskundige kennis nodig om machine learning te begrijpen. Ik zal mijn voortgang hiervan vastleggen.

Voor coursera heb ik de volgende hoofdstukken afgerond.

* 1 Linear Regression with One variable
* 2 Linear Regression with Multiple Variables
* 3 Logistic Regression & Regularization
* 6 Advice for Applying Machine Learning

Voor het project vond ik Coursera wel een zware pil. Voor het Urbinn project is het wel leuk als je een beetje begrijpt van machine learning. Echter vond ik de hele coursera course erg zwaar voor het blok en heel erg tijdrovent.

### [Code opdrachten](https://github.com/BobvanElburg/Portfolio_kb-47/tree/master/notebook%20tutorials)
Gedurende de minor heb ik verschillende code opdrachten uitgevoerd waaronder de spark tutorial. Deze heb ik opgenomen in mijn portfolio.

### [Issues](https://github.com/BobvanElburg/Portfolio_kb-47/tree/master/issues)
In mijn portfolio heb ik de issues waar ik aan heb gewerkt opgenomen. Over deze issues heb ik een uitleg gegeven wat ik heb uitgevoerd.

|issue|uitleg|resultaten|
|-----|------|----------|
|43|Voor het project Urbinn was het doel gesteld om de software en hardware te evalueren. Hiervoor was het benodigt om een template te maken voor het maken van een evaluatieplan. Ik heb de template gemaakt voor evaluatiedocumenten. Hierop heb ik een evaluatieplan geschreven.|Document: Evaluatieplan|
|52|In deze issue is de nadruk gelegd om naar evaluatiemethode te kijken die relevant zijn voor ons project. Ik heb gekeken naar verschillende papers die bbetrekking hebben tot ons project. Ik heb de paper van TUM gebruikt voor informatie over de uitvoer van de evaluatie over Object Detection en Semantic mapping en hoe wij dit zelf kunnen toepassen.|Papers: ECMR_2015_Razlaw, measuring the accuracy of slam algorythms, sturm12iros_ws, Document: Evaluatie TUM & ORB SLAM2|
|55|In deze issue is het doel om papers, die gerelateerd zijn aan object detection, kritisch te lezen. Ik heb een paper eruitgehaald omdat deze niet de juiste methode hanteren om objecten te herkennen die bruikbaar is voor ons project.|Papers|
|63|In deze Issue moest ik de pointcloud tegenover een andere pointcloud zetten. Samen met Isa heb ik gewerkt om een pointcloud van de KITTI-dataset(ground truth) over de eigen pointcloud die wij met ORB-Slam2 hebben gemaakt.|Document: Issue 63 - Evaluatieplan point cloud|
|68| In issue 68 was het doel om onderzoek te doen naar de manier waarop "Tiny Yolo" getraind wordt en hoe het trainingsproces werkt. In deze Issue heb ik gekeken hoe het programma "Tiny Yolo" getraind kon worden. Hierbij keek ik naar de informatie dat het programma nodig had en hoe het trainingsproces in elkaar zat. Dit heeft mij duidelijkheid gegeven over de werking van Yolo en hoe deze leert aan de hand van eerder gelabelde plaatjes. Het deel over het convolutional netwerk vond ik erg interessant. Dat door een afbeelding in kleinere delen te splitsen en verschillende kanalen en hier met een bepaalde zekerheid kan worden aangetoond dat het een object is, is erg fascinerend.|Hoe Yolo te trainen|
|77|Voor deze issue heb ik een presentatie gemaakt en de blog bijgewerkt.|Blog|
|86|Ik heb samen met groepsleden de trainingsdata van Kitti opnieuw gelabeld om zo nieuwe trainingsdata voor Yolo te maken. Hiermee hopen er het probleem op te lossen dat ons objectherkenningssysteem niet overfit door meer trainingsdata toe te voegen.|B-Box Labeling Tool|
|87|Papers gezocht voor close reading sessie.|Papers|
|104|Samen met Viradj opnamens gemaakt met de stereo camera voor trainingsdoeleinden.|Foto's|
|114|Samen met Viradj plannen gemaakt voor de opnamens van Delft. Hierbij hebben we routes gemaakt en later is dit uitgevoerd.|Evaluatie Delft|
|120|Met het RGB naar HSV hue experiment heb ik zelf code geschreven voor het omzetten van RGB afbeeldingen naar HSV hue. Deze afbeeldingen worden dan ook opgeslagen op de jupyter server. Ik vond dit lastig maar het lukte uiteindelijk wel.|Code|
|130|Voor deze issue is aan mij opgedragen een stuk code opnieuw te scrijven om een pointcloud te maken.|Code pointcloud|
|152|Ik heb in samenwerking de introductie gemaakt voor de paper.|Paper|
|153|In de paper heb ik in samenwerking het hoofdstuk "related work" geschreven.|Paper|
|154|Gewerkt aan het opzetten van het hoofdstuk "design" voor de paper.|Paper|
|155|Bezig geweest met het hoofdstuk "experiment" te ontwikkelen in de paper.|Paper|
|156|Meegeholpen met het hoofdstuk "Evaluatie" van de paper.|Paper|
|157|Het hoofdstuk "Results" van de paper geschreven en gecontroleerd.|Paper|
|158|Mede vorm gegeven aan de discussie van de paper.|Paper|
|159|In samenspraak conclusies gevormd voor de paper.|Paper|

### [Bullshit opdracht](https://github.com/BobvanElburg/Portfolio_kb-47/tree/master/bullshit%20opdracht)
Ik heb de opdrachten en illustraties, die ik heb gebruikt voor de bullshitopdrachten, opgenomen in mijn portfolio.

## Unieke bijdrage
### [Documenten](https://github.com/BobvanElburg/Portfolio_kb-47/tree/master/Documenten)
Tijdens de minor KB-47 heb ik verschillende documenten opgesteld. Deze zal ik in een aparte map plaatsen om mijn contributie aan de groep vast te leggen.

### [Presentaties](https://github.com/BobvanElburg/Portfolio_kb-47/tree/master/Presentaties)
Iedere week worden er presentaties gehouden om de voortgang van het project te bespreken. De presentaties waar ik aan mee heb geholpen zal ik in een aparte map plaatsen ter vastlegging van mijn contributie. Tijdens de minor heb ik voor een paar mensen ingevallen. Verder heb ik in de volgende weken gepresenteerd.

* Week 1 EM-Fields
* Week 2 EM-Fields
* Week 8 Urbinn
* Week 9 Urbinn
* Week 10 Urbinn
* Calling Bullshit - John Deere & Big Data (naamloze presentatie.pptx)
![alt text](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/bullshit%20opdracht/gold%20and%20wealth.png "Logo Title Text 1")

### [Eigen code/notebooks](https://github.com/BobvanElburg/Portfolio_kb-47/tree/master/bullshit%20opdracht)
Zelf heb ik niet veel code uitgevoerd omdat dit niet mijn expertise is. Wel heb ik de notebooks met code opgenomen in mijn portfolio.

### Reflectie
De minor kb-47 vond ik een erg interessante minorkeuze. De minor trok mijn aandacht op het gebied van onderzoek en samenwerking met anderen op verschillende expertisegebieden. 


Al snel had onze groep een solide structuur gebouwd op het gebied van afspraken, communicatie en planning. Binnen de groep was er wel de drang om verder te gaan met het project. Echter was er geen informatie beschikbaar die welbenodigd was om het project te bevorderen. Om deze reden hebben we de eerste 4 weken ons bezig gehouden met de Python courses en het lezen van papers. Helaas werd de groep 4 weken later opgeheven door persoonlijke problemen van de meelopende docent. 


Na de opheving van EM-Fields werd ik geplaatst in een nieuwe groep die zich bezig hield met het project Urbinn. Dit project focust zich op het maken van een semantische kaart die gebruikt zal worden om een zelfrijdende auto te helpen in het herkennen van de huidige locatie en objecten.

In de nieuwe groep merkte ik samen Viradj (groepslid die ook een business mindset heeft) dat de groepsstructuur niet soepel en stroef verliep. Aan de hand hiervan hebben Viradj en ik aangegeven de structuur van de groep aan te willen pakken. Door elk groepslid te vragen over de huidige situatie van de groepsstructuur en functionering zijn punten genoteerd en meegenomen in een mogelijke oplossing.
Deze oplossing hebben we erg dynamisch gehouden en was vrij kneedbaar voor implementatie. Viradj en ik hebben gedurende de tijd de oplossingen uitgelegd aan Jeroen (onze meelopende docent) met achterliggende gedachten dat niet alles geïmplementeerd moest worden maar dat ieder punt de groepsstructuur kan verbeteren. Dit gesprek met Jeroen ging redelijk, hij leek op sommige punten niet erg vrolijk en we hadden het gevoel alsof het soms een beetje veel om te bevatten was. Hiervoor hebben we tijdens het gesprek dit rustiger en simpeler uit te leggen voor hem. Dit was voor Jeroen wel duidelijker om te begrijpen.

Na deze uitleg zijn bepaalde punten van onze oplossingen toegepast op de groep. Een paar voorbeelden hiervan zijn het labelen van de scrum issues en het toewijzen van een scrum master. Het toewijzen van de scrum master functie vond ik niet erg fijn. Deze functietoewijzing was niet besproken in de groep en was gelijk vastgesteld. Zelf zou ik het fijner vinden als de groep meer de keuzevrijheid kreeg om zelf een scrum master toe te wijzen. 

Binnen de groep heb ik mij volledig ingezet om zo snel mogelijk de draad op te kunnen pakken en mee te draaien met het door de groep gemaakte schema. In de groep is er veel vraag naar het gebruik van code om veel scrum issues af te handelen. Mijn kennis op het gebied van Python is nog vrij nieuw en ben nog momenteel nog niet in staat om zelf complexe codes te schrijven. Mijn expertise licht op het gebied van informatie beveiliging en het zien van problemen vanuit verschillende oogpunten.

Voor het scrum proces binnen de groep is een document opgesteld om de definitie vast te stellen van wanneer taken "Done" zijn. Dit document heb ik bekeken en was hier niet tevreden mee. Het document bevatte 16 regels die waren opgedeeld in twee categorieën wat zou betekenen dat er twee definities waren van "Done". Aan de hand van het document heb ik zelf een document opgesteld over het definieëren van alle scrum proces statussen.

In week 5 heb ik mij bezig gehouden met het maken van een evaluatieplan die de accuraatheid van het programma ORB SLAM2 te meten. Mijn kennis over ORB SLAM2 was in die tijd erg gelimiteerd en moest ik veel documenten lezen voor meer informatie over het programma. Tijdens week 5 kreeg ik door dat ik mijn deadline voor het opleveren van een evaluatieplan in die week niet kon halen. Hiervoor heb ik gevraagd aan de groep om hulp. 

In week 6 is de taak aangepast om specifieker hhet probleem aan te pakken. Deze taak heb ik samen met Isa Isaku(groepslid) opgepakt. Samen met Isa heb ik aan tafel gezeten om te kijken wat precies geëvalueerd moest worden. Dit gesprek was erg zinvol en hebben we samen veel bereikt op het vaststellen wat precies geëvalueerd moet worden. Dit hebben we later gedocumenteerd.

Aan het einde van week 6 hebben Isa en ik de voortgang van de sprint gepresenteerd aan de andere groepen/projecten. Deze presentatie hebben we opgedeeld in twee stukken. Isa heeft de eerste helft gepresenteerd en ik de tweede helft. In de tweede helft van de presentatie heb ik de nieuwe planning van het project uitgelegd. Hiernaast heb ik ook uitleg gegeven over de aankomende focus van de groep waar de projectgroep verder mee zal gaan. Ik vond het erg belangrijk om te presenteren voor mijn eigen ontwikkeling. Een van mijn mindere punten is het presenteren voor grotere groepen en vind dit een goed leerpunt voor mijzelf. 

------------------------------------------
