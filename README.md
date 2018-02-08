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
<br>[Klik hier voor een afbeelding hoe de opnames HHS werden uitgevoerd](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Plaatjes/opnameshhs.jpg)

Samen met Nektarios, Kevin en Viradj heb ik meer dan 500 foto's gelabeld. Iedere foto bevatte gemiddeld meer dan 15 verschillende objecten die gelabeld moesten worden zodat we het programma YOLO verder konden trainen om overfitting te voorkomen. Chris heeft hier later een testrun overheen laten lopen.
![Testrun KITTI](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Plaatjes/KITTIYolo.png)



---------------------------------------------------------------------------------
## Unieke bijdrage/Uitgelichte onderwerpen
### Evalueren van de Pointcloud
Ik ben vooral bezig geweest met het maken van en helpen bij de evaluaties van soft- en hardware. Ik heb zelf een grote bijdrage geleverd aan het zoeken naar evaluatiemethodes die toepasbaar zijn op het project Urbinn. Voor het evalueren van de Pointcloud die is gemaakt door ORB-Slam2 hebben we gekeken naar verschillende mogelijkheden. Hiervoor heb ik een reeks aan verschiillende wetenschappelijke papers kritisch doorgelezen en opgenomen in documentatie.

Uit deze methodes heb ik de keuze gemaakt om de pointcloud met de ground-thruth pointcloud te vergelijken. Door de punten uit de pointcloud met elkaar te vergelijken kan gekeken worden hoeveel afwijking aanwezig is. Ik heb nagedacht dat het lastig is voor het ORB-Slam2 algoritme om alle exacte punten te vinden. Daarom wordt er gebruik gemaakt van de Nearest Neighbours techniek om punten met de kortste afstand uit beide mappen met elkaar te vergelijken.

Voor het vergelijken van de Pointsclouds maak ik gebruik van het programma Cloudcompare. Cloudcompare geeft de mogelijkheid om pointclouds in te laden en te vergelijken. ![cloudcompare](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Plaatjes/Cloudcompare.jpg)

## Hoe YOLO te trainen en Labelen van informatie
Voor het detecteren van objecten maakt de groep gebruik van het programma YOLO. De YOLO software wordt gebruikt voor real-time object detection en classification. De ontwikkeling van Yolo is erg slecht gedocumenteerd en hierdoor was het lastig om de manier te vinden waarop traint. Hiervoor heb ik onderzoek moeten uitvoeren over de werking van YOLO. YOLO maakt gebruik van een convolutional network wat gebruikt wordt voor class/deep learning. 
![YOLO2](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Plaatjes/YOLO2.png)
De convolutional network wordt de afbeelding opgesplitst in behapbare delen. Hierbij wordt aan ieder vlak een gewicht gehangen dat meegenomen wordt in het pooling proces. Het pooling proces die de uitkomsten clustert en meegeeft aan een nieuwe convolutional layer. In deze processen word gekeken naar naastliggende vlakken die mogelijke relevantie hebben met elkaar. Dit proces van convolutional layer en pooling herhaald zich een vastgesteld aantal keer en komt met een resultaat waarin een zekerheid wordt gegeven over de herkenning van een object en welk object.

Het trainen van YOLO was erg interessant om te zien en mee te maken. Echter kwamen we tot een probleem dat YOLO Om YOLO verder te trainen was meer traingingsdata benodigt. Meer trainingsdata helpt tevens ook tegen overfitten, door meer trainingsdata te hebben dan features.

Het maken van nieuwe trainingsdata heeft twee weken geduurd om alle objecten in meer dan 500 foto's te labellen. Dit heeft later wel geholpen met het beter kunnen herkennen van verkeersborden, ramen, lantaarnpalen, paaltjes, auto's, voetgangers, etc.
![bboxlabelingtool](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Plaatjes/bboxlabelingtool.jpg)


## Algemene onderdelen
### [Datacamp](https://github.com/BobvanElburg/Portfolio_kb-47/tree/master/Datacamp)
Voor de minor is de vraag naar kennis over de codetaal Python. Het is lastig om hiervan de voortgang vast te leggen. Ik probeer zoveel mogelijk informatie vast te leggen om mijn voortgang te laten zien.

Voor datacamp heb ik de volgende courses gemaakt en afgerond.

* [Intro to Python for Data Science](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Datacamp/Intro%20to%20python%20for%20Data%20Science.png)
* [Intermediate Python for Data Science](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Datacamp/Intermediate%20Python%20for%20Data%20Science.png)
* [Python Data Science Toolbox (Part 1)](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Datacamp/Pyhon%20Data%20Science%20Toolbox%20(Part1).png)
* [Pandas foundation](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Datacamp/Pandas%20Foundation.png)
* [Python Data Science Toolbox (Part 2)](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Datacamp/Python%20Data%20Science%20Toolbox%20(Part2).png)
* [Introduction to data visualization with Python](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Datacamp/Introdcution%20to%20Data%20Visualization%20with%20Python.png)
* [Cleaning Data](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Datacamp/Cleaning%20Data%20in%20Python.png)
* [Statistical Thinking in Python (part 1)](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Datacamp/Statistical%20thinking%20in%20Python(Part1).png)
* [Supervised Learning with scikit-learn](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Datacamp/Supervised%20learning%20with%20scikit-learn.png)

Ik vond de Python courses erg leuk maar wel tijdrovend. Vooral omdat het project zoveel tijd vereist blijft er weinig tijd over om zelf opdrachten uit te voeren.

### [Coursera](https://github.com/BobvanElburg/Portfolio_kb-47/tree/master/Coursera)
Tijdens de minor is geavanceerde wiskundige kennis nodig om machine learning te begrijpen. Ik zal mijn voortgang hiervan vastleggen.

Voor coursera heb ik de volgende hoofdstukken afgerond.

* Week 1 Linear Regression with One variable
* Week 2 Linear Regression with Multiple Variables
* Week 3 Logistic Regression & Regularization
* Week 6 Advice for Applying Machine Learning

Coursera afbeeldingen.
* [Afbeelding van overzicht 1](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Coursera/coursera%20progress%201.PNG)
* [Afbeelding van overzicht 2](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Coursera/coursera%20progress%202.PNG)
* [Afbeelding van overzicht 3](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Coursera/extra%20coursera%20foto.PNG)

Voor het project vond ik Coursera wel een zware pil. Voor het Urbinn project is het wel leuk als je een beetje begrijpt van machine learning. Echter vond ik de hele coursera course erg zwaar voor het blok en heel erg tijdrovent.

### [Code opdrachten](https://github.com/BobvanElburg/Portfolio_kb-47/tree/master/notebook%20tutorials)
Gedurende de minor heb ik verschillende code opdrachten uitgevoerd waaronder de spark tutorial. Deze heb ik opgenomen in mijn portfolio.
* [Spark deel 1](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Spark/assignment1.md)
* [Spark deel 2](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Spark/assignment2.md)
* [Exploratory_data_analysis plaatjes](https://github.com/BobvanElburg/Portfolio_kb-47/tree/master/Exploratory_data_analysis)


### [Issues](https://github.com/BobvanElburg/Portfolio_kb-47/tree/master/issues)
In mijn portfolio heb ik de issues waar ik aan heb gewerkt opgenomen. Over deze issues heb ik een uitleg gegeven wat ik heb uitgevoerd.

|issue|uitleg|resultaten|
|-----|------|----------|
|43|Voor het project Urbinn was het doel gesteld om de software en hardware te evalueren. Hiervoor was het benodigt om een template te maken voor het maken van een evaluatieplan. Ik heb de template gemaakt voor evaluatiedocumenten. Hierop heb ik een evaluatieplan geschreven.|Document: [Evaluatieplan aanpak](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Documenten/evaluatie%20aanpak.docx), [Evaluatieplan](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Documenten/evaluatieplan.docx)|
|52|In deze issue is de nadruk gelegd om naar evaluatiemethode te kijken die relevant zijn voor ons project. Ik heb gekeken naar verschillende papers die bbetrekking hebben tot ons project. Ik heb de paper van TUM gebruikt voor informatie over de uitvoer van de evaluatie over Object Detection en Semantic mapping en hoe wij dit zelf kunnen toepassen.|[Wetenschappelijke Papers](https://github.com/BobvanElburg/Portfolio_kb-47/tree/master/Wetenschappelijke%20papers): ECMR_2015_Razlaw, measuring the accuracy of slam algorythms, sturm12iros_ws, Document: Evaluatie TUM & ORB SLAM2|
|55|In deze issue is het doel om papers, die gerelateerd zijn aan object detection, kritisch te lezen. Ik heb een paper eruitgehaald omdat deze niet de juiste methode hanteren om objecten te herkennen die bruikbaar is voor ons project.|[Wetenschappelijke Papers](https://github.com/BobvanElburg/Portfolio_kb-47/tree/master/Wetenschappelijke%20papers)|
|63|In deze Issue moest ik de pointcloud tegenover een andere pointcloud zetten. Samen met Isa heb ik gewerkt om een pointcloud van de KITTI-dataset(ground truth) over de eigen pointcloud die wij met ORB-Slam2 hebben gemaakt.|[Document: Issue 63 - Evaluatieplan point cloud](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Documenten/Issue%2063%20-%20Evaluatieplan%20point%20cloud.docx)|
|68| In issue 68 was het doel om onderzoek te doen naar de manier waarop "Tiny Yolo" getraind wordt en hoe het trainingsproces werkt. In deze Issue heb ik gekeken hoe het programma "Tiny Yolo" getraind kon worden. Hierbij keek ik naar de informatie dat het programma nodig had en hoe het trainingsproces in elkaar zat. Dit heeft mij duidelijkheid gegeven over de werking van Yolo en hoe deze leert aan de hand van eerder gelabelde plaatjes. Het deel over het convolutional netwerk vond ik erg interessant. Dat door een afbeelding in kleinere delen te splitsen en verschillende kanalen en hier met een bepaalde zekerheid kan worden aangetoond dat het een object is, is erg fascinerend.|[Hoe Yolo te trainen](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Documenten/ISSUE%2068%20-%20Hoe%20tiny%20yolo%20te%20trainen.docx)|
|77|Voor deze issue heb ik een presentatie gemaakt en de blog bijgewerkt.|[Blog week 10](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Presentaties/Blog%20week%2010.docx)|
|86|Ik heb samen met groepsleden de trainingsdata van Kitti opnieuw gelabeld om zo nieuwe trainingsdata voor Yolo te maken. Hiermee hopen er het probleem op te lossen dat ons objectherkenningssysteem niet overfit door meer trainingsdata toe te voegen.|[B-Box Labeling Tool](https://github.com/urbinn/BBox-Label-Tool)|
|87|Papers gezocht voor close reading sessie.|[Wetenschappelijke Papers](https://github.com/BobvanElburg/Portfolio_kb-47/tree/master/Wetenschappelijke%20papers)|
|104|Samen met Viradj opnamens gemaakt met de stereo camera voor trainingsdoeleinden. Deze zijn gemaakt met de B-Box Labeling Tool.|[B-Box Labeling Tool](https://github.com/urbinn/BBox-Label-Tool)|
|114|Samen met Viradj plannen gemaakt voor de opnamens van Delft. Hierbij hebben we routes gemaakt en later is dit uitgevoerd.|[Evaluatie Delft](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Documenten/Issue%20114_%20Plan%20maken%20openames%20Delft.docx)|
|120|Met het RGB naar HSV hue experiment heb ik zelf code geschreven voor het omzetten van RGB afbeeldingen naar HSV hue. Deze afbeeldingen worden dan ook opgeslagen op de jupyter server. Ik vond dit lastig maar het lukte uiteindelijk wel.|[HSV Experiment](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Eigen%20notebooks/HSV%2Bexperiment.ipynb)|
|130|Voor deze issue is aan mij opgedragen een stuk code opnieuw te scrijven om een pointcloud te maken.|[Code Plot_Trajectory](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Eigen%20notebooks/plot_trajectory.ipynb)|
|152|Ik heb in samenwerking de introductie gemaakt voor de paper.|[Paper](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Documenten/Kopie%20van%20landmark-filtering-techniques-for-semantic-mapping.docx)|
|153|In de paper heb ik in samenwerking het hoofdstuk "related work" geschreven.|[Paper](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Documenten/Kopie%20van%20landmark-filtering-techniques-for-semantic-mapping.docx)|
|154|Gewerkt aan het opzetten van het hoofdstuk "design" voor de paper.|[Paper](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Documenten/Kopie%20van%20landmark-filtering-techniques-for-semantic-mapping.docx)|
|155|Bezig geweest met het hoofdstuk "experiment" te ontwikkelen in de paper.|[Paper](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Documenten/Kopie%20van%20landmark-filtering-techniques-for-semantic-mapping.docx)|
|156|Meegeholpen met het hoofdstuk "Evaluatie" van de paper.|[Paper](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Documenten/Kopie%20van%20landmark-filtering-techniques-for-semantic-mapping.docx)|
|157|Het hoofdstuk "Results" van de paper geschreven en gecontroleerd.|[Paper](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Documenten/Kopie%20van%20landmark-filtering-techniques-for-semantic-mapping.docx)|
|158|Mede vorm gegeven aan de discussie van de paper.|[Paper](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Documenten/Kopie%20van%20landmark-filtering-techniques-for-semantic-mapping.docx)|
|159|In samenspraak conclusies gevormd voor de paper.|[Paper](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Documenten/Kopie%20van%20landmark-filtering-techniques-for-semantic-mapping.docx)|

### [Bullshit opdracht](https://github.com/BobvanElburg/Portfolio_kb-47/tree/master/bullshit%20opdracht)
Ik heb de opdrachten en illustraties, die ik heb gebruikt voor de bullshitopdrachten, opgenomen in mijn portfolio.
* [Powerpoint: Zijn katten vloeibaar](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/bullshit%20opdracht/Bullshit%20extra%20presentatie%20-%20zijn%20katten%20vloeibaar.pptx)
* [Hoofdopdracht Calling Bullshit](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/bullshit%20opdracht/bullshit%20opdracht%20Bob%20van%20Elburg.docx)
* [Calling Bullshit - John Deere & Big Data](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Presentaties/Naamloze%20presentatie.pptx)

### [Documenten](https://github.com/BobvanElburg/Portfolio_kb-47/tree/master/Documenten)
Tijdens de minor KB-47 heb ik verschillende documenten opgesteld. Deze zal ik in een aparte map plaatsen om mijn contributie aan de groep vast te leggen.
* [Map met alle documenten](https://github.com/BobvanElburg/Portfolio_kb-47/tree/master/Documenten)

### [Presentaties](https://github.com/BobvanElburg/Portfolio_kb-47/tree/master/Presentaties)
Iedere week worden er presentaties gehouden om de voortgang van het project te bespreken. De presentaties waar ik aan mee heb geholpen zal ik in een aparte map plaatsen ter vastlegging van mijn contributie. Tijdens de minor heb ik voor een paar mensen ingevallen. Verder heb ik in de volgende weken gepresenteerd.

* [Week 1 EM-Fields](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Presentaties/Sprint%201%20%5Bweek%201%5D%20(powerpoint%201).pptx)
* [Week 2 EM-Fields](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Presentaties/Sprint%201%20%5Bweek%202%5D%20(powerpoint%202).pptx)
* [Week 8 Urbinn](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Presentaties/Kopie%20van%20Week%208%20-%20Presentatie.pptx)
* [Week 9 Urbinn](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Presentaties/Week%209%20-%20Presentatie.pptx)
* [Week 10 Urbinn](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Presentaties/Week%2010%20-%20Presentatie.pptx)
* [Calling Bullshit - John Deere & Big Data](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Presentaties/Naamloze%20presentatie.pptx)
* [Blog week 10](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Presentaties/Blog%20week%2010.docx)

### [Eigen code/notebooks](https://github.com/BobvanElburg/Portfolio_kb-47/tree/master/bullshit%20opdracht)
Zelf heb ik niet veel code uitgevoerd omdat dit niet mijn expertise is. Wel heb ik de notebooks met code opgenomen in mijn portfolio.
* [HSV Experiment](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Eigen%20notebooks/HSV%2Bexperiment.ipynb)
* [Plot Trajectory](https://github.com/BobvanElburg/Portfolio_kb-47/blob/master/Eigen%20notebooks/plot_trajectory.ipynb)

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
