-----------------------------------------------
| PONG 2021 (Javascript / Pong game / 1WDV)   |
-----------------------------------------------


--------------------------------------------------------------------------
Stap 0: BOILERPLATE & SETUP & GIT
--------------------------------------------------------------------------  
   - VScode extention toevoegen: Live Server
   
   - Boilerplate clonen vanaf mijn github:
     git clone https://github.com/Stroomer/webdev-pong2021.git

   - GIT-repo aanmaken op jouw github:
     https://github.com/Romano2003/webdev-pong2021.git

   - GIT lokaal klaarmaken voor de eerste commit:  
             
        git init
        git add .
        git commit -m "Initial Commit"
        git remote add origin https://github.com/Romano2003/webdev-pong-2021.git
        git branch -M Master
        git push -u origin Master

   - Teams:  Jouw GIT-repo toevoegen in exceldocument bij Javascript/bestanden/pong

   - Toelichting op de aangeleverde bestanden en polyfill.js
   

--------------------------------------------------------------------------   
Stap1:  GAME CLASS
--------------------------------------------------------------------------

   - Game Class aanmaken (game.js)
   - Game constructor aanmaken
   - Game update & draw aanmaken
   - Game instance aanmaken
   - Testen

--------------------------------------------------------------------------
Stap2:  GAMELOOP
--------------------------------------------------------------------------

   - Uitleg: Class
   - Polyfill voor requestAnimationFrame aanmaken (polyfill.js)
   - Uitleg Gameloop (met setInterval en arrow-function)
   - Game update & draw aanroepen
   - Testen

--------------------------------------------------------------------------
Stap3: BALL & RECTANGLE CLASS
--------------------------------------------------------------------------
   
   - Ball Class aanmaken (ball.js)
   - Rectangle Class aanmaken (rectangle.js)
   - Vector Class aanmaken (vector.js)
   - Overerving en Extends
   - Ball instance
   - Ball tekenen
   - Testen

--------------------------------------------------------------------------
Stap4: 
--------------------------------------------------------------------------


--------------------------------------------------------------------------
Stap5: 
--------------------------------------------------------------------------


--------------------------------------------------------------------------
Stap6: 
--------------------------------------------------------------------------


--------------------------------------------------------------------------
Stap7: 
--------------------------------------------------------------------------


--------------------------------------------------------------------------
Stap8: 
--------------------------------------------------------------------------


--------------------------------------------------------------------------
Stap9: 
--------------------------------------------------------------------------


--------------------------------------------------------------------------
Stap10: 
--------------------------------------------------------------------------


--------------------------------------------------------------------------
Stap11: 
--------------------------------------------------------------------------


--------------------------------------------------------------------------
Stap12: 
--------------------------------------------------------------------------


--------------------------------------------------------------------------
Stap13: 
--------------------------------------------------------------------------


--------------------------------------------------------------------------
Stap14: 
--------------------------------------------------------------------------


--------------------------------------------------------------------------
Stap15: 
--------------------------------------------------------------------------


--------------------------------------------------------------------------
Stap16: 
--------------------------------------------------------------------------


--------------------------------------------------------------------------
Stap17: 
--------------------------------------------------------------------------


--------------------------------------------------------------------------
Stap18: 
--------------------------------------------------------------------------


--------------------------------------------------------------------------
Stap19: 
--------------------------------------------------------------------------


--------------------------------------------------------------------------
Stap20: 
--------------------------------------------------------------------------




TODO:

* Responsive maken
* Geluidjes inladen en afspelen 
* Intro maken
* Menu maken
* Betere gameloop maken (die nog strakker is en fps beter kan instellen)
* Betere AI schrijven
* Extra obstakels aanmaken
* Extra 'wapens' aanmaken die de speler voordeel geven (bijvoorbeeld multiball of extra ball-velocity)
* Extra technieken gebruiken voor compressie en/of minimalisatie van je code (bijvoorbeeld Webpack of SASS/SCSS)
* Vonken en/of particles toevoegen bij botsingen
* Jouw eigen aanvulling op de game


BEGRIPPENLIJST:

* class
Een class is een container waar variabelen en functies als een pakketje worden samengevoegd. 
De logica wordt afgescherm en de class is een blauwdruk voor de aanmaak van objecten.

* instance 
Een instance is een object die met behulp van het magische woord 'new' een nieuwe 'spawn' aanmaakt.
Het object is ontstaan uit de beschrijving die in de class staat. Het object stampt dus af van 
de class en wordt opgeslagen op een bepaalde geheugenlocatie. Aan het woord 'new' kan je zien dat 
er een instance wordt aangemaakt. Die instance noem je vanaf dat moment een 'object'. 

* constructor
Een constructor is een functie die wordt aangeroepen op het moment dat er een instance van een 
bepaalde class wordt aangemaakt. Je kan daar dus begininstelling mee instellen.

* function
Een function is een stukje code waarbij telkens dezelfde stappen worden doorlopen. Functions zijn 
erg handig op het moment dat je bepaalde code-fragementen schrijft die identiek zijn. Die identieke 
stappen in je code kan je dan in de functie zetten en op het moment dat je die stappen wilt uitvoeren, 
geef je het commando om de functie uit te voeren.

* parameters
Een function kan parameters hebben die bepaalde waarden doorgeven die intern in de functie kunnen 
worden gebruikt.

* arrow-function
Een arrow-function is een nieuwere manier van gebruik van een function, waarbij de scope van het 
woord 'this' behouden blijft. Soms, als je een function in een function zet bijvoorbeeld, heb je dat 
de toegang tot het woord 'this' verloren gaat. Dat kan je wel oplossen met work-arounds, maar met een 
arrow-function heb je dat probleem dus niet meer. Deze nieuwere manier van functions aanmaken is onderdeel 
van de Ecmascript6 standaard (ES6). 

* var
Variabelen van het type 'var' zijn ouderwetse (ES5) variabelen. Deze variabelen zijn ook na het aanmaken 
nog te veranderen in een andere waarde. Binnen een class ook te gebruiken, maar dan als locale variabele.

* const
Variabelen van het type 'const' zijn modernere (ES6) variabelen en zijn niet aan te passen nadat ze zijn 
ingesteld, vandaar de naam 'constant'. Binnen een class ook te gebruiken, maar dan als locale variabele.

* let
Variabelen van het type 'let' zijn modernere (ES6) variabelen en zijn wel aan te passen nadat ze zijn 
ingesteld. Kanttekening is wel dat deze variabelen in code-blokken een beperktere scope kunnen hebben.
Binnen een class ook te gebruiken, maar dan als locale variabele.

* this
Variabelen van het type 'this' worden gebruikt om aan te geven dat het om een variabele gaat die 
onderdeel is van een bepaalde class. De variabele is eigendom van de class.

* scope 
De scope gaat over het bereik van een variabele of function. Neem het voorbeeld van de arrow-function.
Als je een function in een function definieert, dan kan de scope naar 'this' verloren gaan. 
De scope wordt ook wel 'bereik' genoemd. 

* getters / setters
Naast variabelen en functies kunnen classes ook getters en setters hebben. Het zijn speciale functies die 
een variabele kunnen ophalen (get) of wegschrijven (set).

* rectangle
Een rectangle is een rechthoek. Een rechthoek heeft een x- en y-locatie, maar ook een breedte en hoogte.
De Pong game is eigenlijk voor 100% uit rechthoeken opgebouwd. Vandaar ook dat de class Rectangle erg 
belangrijk is en talloze malen wordt herbruikt. Zo wordt code efficient ingezet en vaak gebruikt.

* vector
Een vector geeft in feite alleen een richting aan. We gebruiken het in de Ponggame om een object aan te 
maken die een x- en y-waarde heeft, bijvoorbeeld zoals in:  {x:0, y:0}
In de class Rectangle gebruiken we Vector drie keer achter elkaar, omdat we een position, size en velocity 
nodig hebben die allemaal een x- en y-waarde nodig hebben. Weer een stukje efficientie dus!

* polyfill
Een polyfill is een verlengstukje in je code die ervoor zorgt dat browsers die functionaliteiten niet 
ondersteunen toch kunnen omgaan met deze wens. Stel bijvoorbeeld dat je function 'a' wilt gebruiken, maar 
die wordt niet ondersteund, dan kan je function 'a' zelf schrijven en zodat toch het gewenste gedrag 
kan worden weergegeven. De polyfill zorgt dat de tekortkoming in de browser toch kan worden opgelost.

* requestAnimationFrame
De function 'requestAnimationFrame' is een oplossing van Paul Irish voor het renderen van frames die 
toch niet zichtbaar kunnen worden gemaakt. Soms worden er bij animaties verzoeken gedaan om frames te 
tekenen, maar als de tijd om de frame te lang duurt ten opzichte van de framerate, dan zou het wijzer 
zijn als het script ervoor te kiezen om de frame niet te tekenen. Op die manier kan performance winst ontstaan.

* setInterval
De function setInterval kan net zoals requestAnimationFrame zorgen voor een gameloop of herhalend patroon 
waarbinnen iets kan worden uitgevoerd. De requestAnimationFrame en setInterval zijn eigenlijk vergelijkbaar, 
hoewel setInterval als de 'domme variant' wordt gezien. Deze functie ziet namelijk niet dat bepaalde frames 
uberhaupt niet getekend kunnen worden, maar leggen dus wel de rekening neer van niet-getekende frames.

* canvas
De canvas-tag is een dynamische bitmap en html5-tag die gebruikt kan worden om complete games en/of films 
op af te spelen. In de Ponggame gebruiken we er twee (zie index.html), een voor de game en een voor de hud.

* hud
Hud staat voor Headsup-display, het is een afkorting die gaat over de begeleidende onderdelen van een game. In de Ponggame hebben we die apart genomen op een canvas, omdat het onzin is om bijvoorbeeld de score iedere frame opnieuw te tekenen. De score verandert meestal niet iedere frame, alleen als er punten behaald zijn.

* context
De context is het raster van pixels van het canvas-element. Het zijn de feitelijke pixels die hierin liggen opgeslagen.

* getElementById()
De functie getElementById stelt je in staat om een HTML-element met een bepaald 'id' op te halen. 
In de Ponggame doen we dat bijvoorbeeld bij het ophalen van het canvas-element (zie class Game/constructor).
 
