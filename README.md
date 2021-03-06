# Procesverslag
Markdown is een simpele manier om HTML te schrijven.  
Markdown cheat cheet: [Hulp bij het schrijven van Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

Nb. De standaardstructuur en de spartaanse opmaak van de README.md zijn helemaal prima. Het gaat om de inhoud van je procesverslag. Besteedt de tijd voor pracht en praal aan je website.

Nb. Door *open* toe te voegen aan een *details* element kun je deze standaard open zetten. Fijn om dat steeds voor de relevante stuk(ken) te doen.

## Jij

<details>
<summary>uitwerken voor kick-off werkgroep</summary>

### Auteur:
Bram Tersteeg.

#### Je startniveau:
Rood, ken wel een beetje maar ben nog niet mega goed.

#### Je focus:
Surface plane en responsive
 
</details>


## Je website

<details>
<summary>uitwerken voor kick-off werkgroep</summary>

### Je opdracht:
https://www.orsm.jp/#top

#### Screenshot(s) van de eerste pagina (small screen): 
Landing section
<img src="images/screenshots/screenshot_1.png" width="375px" alt="Op de landing section is een achtergrond, menu en een afbeelding te zien. Ook is er een button te zien die aangeeft dat je naar beneden moet scrollen.">

#### Screenshot(s) van de tweede pagina (small screen):
Begin animatie
<img src="images/screenshots/screenshot_2.png" width="375px" alt="De section begint met een animatie die het scherm uit beweegt. Hierna is het nieuws zichtbaar">
News section
<img src="images/screenshots/screenshot_3.png" width="375px" alt="Na de animatie is er nieuws te zien met een paar categorieën. Ook bevinden zich er een aantal afbeeldingen omheen en een verticaal scroll menu.">
 
</details>



## Breakdownschets (week 1)

<details>
<summary>uitwerken na afloop 2e werkgroep</summary>

### de hele pagina: 
<img src="images/breakdown_schetsen/breakdown_hele_pagina.jpg" width="375px" alt="breakdown van de hele pagina">

### dynamisch deel 1 (scrollanimatie): 
<img src="images/breakdown_schetsen/breakdown_dynamisch_deel1.jpg" width="375px" alt="breakdown van het begin van de scrollanimatie">
<img src="images/breakdown_schetsen/breakdown_dynamisch_deel2.jpg" width="375px" alt="breakdown van de scrollanimatie halverwege">

### dynamisch deel 2 (hamburgermenu mobiel): 
<img src="images/breakdown_schetsen/breakdown_dynamisch2_deel1.jpg" width="375px" alt="breakdown van het menu dat openklapt">

</details>





## Voortgang 1 (week 2)

<details open>
<summary>uitwerken voor 1e voortgang</summary>

### Stand van zaken
Ik heb een start gemaakt aan mijn HTML. Ik was soms nog wel even aan het twijfelen of ik dingen soms semantischer neer kon zetten, maar verder ging het goed. Ik heb gekeken naar het maken van een hamburgermenu met javascript om mijn kennis weer even op te frissen, en ik heb gekeken naar de Intersection Observer.  


### Agenda voor meeting
samen met je groepje opstellen

| Bram     | Xiao Nan         | Kevin    | Tijn        |
| ---      | ---              | ---      | ---         |
|  | aria-label | figure/figcaption |  |
|          | feedback op haar html | achtergrondimg |   |
|          |                  |          |             |
| ...      | ...              | ...      | ...         |


### Verslag van meeting
hier na afloop snel de uitkomsten van de meeting vastleggen

- Door het kijken naar Xiao Nan haar HTML zijn we allemaal iets meer te weten gekomen over semantische HTML.
- Geleerd hoe we een aria-label moeten gebruiken.
- .Visually-hidden class gebruiken als je een heading element in een element niet wil gebruiken maar er wel in stopt voor semantiek. https://www.a11yproject.com/posts/2013-01-11-how-to-hide-content/ 
- Opgefrist wanneer je nou een button of a element gebruikt.

</details>


## Voortgang 2 (week 3)

<details>
<summary>uitwerken voor 2e voortgang</summary>

### Stand van zaken
Ik ben verder gegaan aan mijn HTML en heb hierbij wat content toegevoegd aan mijn website. De sections staan en zijn nu scrollbaar met de intersection observer (hoewel deze het nu even niet goed doet.) Ik ben van plan alle content eerst in de website te zetten en daarna aan de animaties te beginnen.


### Agenda voor meeting
samen met je groepje opstellen

| Bram     | Xiao Nan          | Kevin    | Tijn       |
| ---            | ---                | ---          | ---              |
| toevoegen van een slider | witruimte tussen afbeelding en section weghalen | hamburgermenu |    |
|                |                    |              |                  |
| ...            | ...                | ...          | ...              |

Bonus tip van Yunus: Schrijf zo helder mogelijke css, toepassen van bepaalde structuur kan helpen.

### Verslag van meeting
hier na afloop snel de uitkomsten van de meeting vastleggen

- Door de link naar Sanne zijn voorbeelden over sliders, wist ik beter hoe ik mijn eigen sliders aan moest pakken.
- Ik ben iets meer te weten gekomen over debuggen, omdat Xiao Nan een probleem had waar de studentassistenten ook niet zo snel een antwoord op wisten.

</details>


## Toegankelijkheidstest (week 4)

<details>
<summary>uitwerken na test in 8e voortgang</summary>

### Bevindingen
1. Button voor het hamburgermenu word overgeslagen aan het begin.
2. Als het menu openstaat is andere content op de pagina nog gewoon toegankelijk wat niet hoort.
3. Met de screenreader was er een goede scheiding tussen Engelse en Japanese content en veranderde hij goed van stem. Alleen konder sommige aria-labels nog duidelijker.
4. Met de wazige bril was sommige tekst soms slecht leesbaar, dit gelde vooral voor de content van de slider.

#### Overgeslagen hamburgericoon (Toetsenbord)
Bij het tabben door de website werd op mobiel elke keer het hamburgermenu overgeslagen en ging je meteen naar de live section toe. 

Ik had hiernaar gekeken en wat het had opgelost was om de tabIndex van 0 naar 1 te veranderen.

<img src="images/tabindex0.png" width="375px" alt="Image waar de tabindex 0 is">
<img src="images/tabindex1.png" width="375px" alt="Image waar de tabindex 1 is">


#### Alle content toegankelijk als menu openstaat (Toetsenbord)
Bij het tabben kwam ik er achter dat als het menu openstaat hij gewoon naar de volgende section toe tabbed als je bij het laatste menu item bent.

Michiel en ik hadden dit nagevraagd aan Sanne en hij gaf ons een paar links waarmee we dit probleem aan konden pakken.

1. https://developer.mozilla.org/en-US/docs/Web/API/Document/keydown_event
2. https://developer.mozilla.org/en-US/docs/Web/CSS/:focus-within
3. https://keycode.info/

Ik heb besloten hiernaar te gaan kijken als ik tijd over heb.

#### Zowel Japans als Engels (screenreader)
Voor mijn website was het een uitdaging om zowel Japans en Engels leesbaar te kunnen maken met de screenreader. Gelukkig ging dit goed omdat ik al vrij vroeg op Japanse elementen de lang had verandert naar "ja". Het enige wat soms nog een beetje moeizaam ging was dat ik een element slecht had uitgelegd of dat twee elementen die gewrapped waren niet goed voor werder gelezen.

<img src="images/back_to_top_button_before.png" width="375px" alt="back to top button voor veranderingen">

Na een gesprekje te hebben gehad met Sanne vertelde hij over aria-hidden="true". Ik heb dit opgezocht en toen zelf proberen te gebruiken.
https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/ARIA_Techniques/Using_the_aria-hidden_attribute

<img src="images/back_to_top_button_after.png" width="375px" alt="back to top button na veranderingen">


#### Sommige content onleesbaar voor slechtzienden
Door een wazige bril op te hebben gezet kwam ik erachter dat kleine dingen in de slider bijvoorbeeld slecht leesbaar waren. Daarom heb ik besloten de mobiele versie van de website ook mee te maken. De titels waren wel groot genoeg om te lezen met de bril op. Ik zou dit op kunnen lossen door op mobiel specifiek, de kleine content uit de slider bijvoorbeeld grotere blokken te kunnen geven.

<img src="images/slider_voor.png" width="375px" alt="de slider voor de veranderingen">
<img src="images/slider_na.png" width="375px" alt="de slider na de veranderingen">


</details>





## Voortgang 3 (week 4)

<details>
<summary>uitwerken voor 3e voortgang</summary>

### Stand van zaken

Ik heb een tijd zitten twijfelen om mobiel anders te maken dan desktop. In de echte site is er een aparte versie voor mobiel en desktop, hij stemt dit automatisch af op het device dat gebruikt word. Hierom leek mij dit leuk om dit ook te proberen, ik heb hierom nu images toegevoegd die tussen de section geplaatst worden als mobiele banners. Deze banners krijgen op groot scherm een display: none; zodat ze zichzelf verbergen. Ook werken de sliders anders op mobiel omdat ze zo beter leesbaar zijn.

Na het toevoegen van de banners op mobiel kwam hier helaas witruimte onder te zitten die ik niet weg kon krijgen. Na met Yunus gepraat te hebben vonden wij dit artikel:
https://stackhowto.com/how-to-remove-white-space-under-an-image-using-css/

In dit artikel stond dat je een display: block; op de image moest zetten. Dit heb ik ook gedaan en toen ging gelukkig de witruimte weg.

<img src="images/display_block.png" width="375px" alt="display block op image">


### Agenda voor meeting
samen met je groepje opstellen

| Bram      | Kevin         | Xiao Nan   |       
| ---            | ---                | ---          | 
| Animation voor section  | Niet meeschalende foto + tekst | rare witruimte boven foto   | 
| Mediaqueries | Overscroll-behavior | Javascript | 
| ...            | ...                | ...          | 


### Verslag van meeting
hier na afloop snel de uitkomsten van de meeting vastleggen

- Ik heb verduidelijking gekregen over hoe ik de animaties precies aan kan pakken.
- Kevin en Xiao Nan weten nu hoe ze de rare witruimte bij een foto weg kunnen krijgen als het ooit bij ze gebeurd.

</details>





## Eindgesprek (week 5)

<details>
<summary>uitwerken voor eindgesprek</summary>

### Stand van zaken
De laatste week was voor mij nog wel een beetje aanpoten. Ik wilde nog best veel dingen van mijn website uitwerken. Ik heb bijvoorbeeld kleine animaties uitgewerkt voor de pijltjes van de sliders, en voor de button in de video section waarmee je weer omhoog kon scrollen. Ik heb er ook voor gekozen om mijn code te verspreiden over meerdere css bestanden. Ik heb css bestanden gemaakt voor de meerdere formaten schermen en voor de section animaties.

Links zijn de keyframes van de arrow animatie te zien, en rechts die van de section animaties.

<img src="images/keyframes_van_de_arrow_animaties.png" width="375px" alt="keyframes van de arrow animaties">
<img src="images/keyframes_van_de_section_animaties.png" width="375px" alt="keyframes van de section animaties">

Ook heb ik geprobeerd om meerdere sliders in de website te zetten. Dit ging een beetje moeizaam omdat ik het moeilijk vond om de code van Sanne aan te passen. Dit was niet omdat Sanne warrige code schreef, maar omdat ik zelf nog niet heel goed ben in JavaScript :)

<img src="images/foutmelding.png" width="375px" alt="foutmelding">

Ik heb uiteindelijk Deanna om hulp gevraagd omdat ik er zelf niet uitkwam. Nadat ik haar om hulp had gevraagd kwam ik pas achter de fout. Toen ik aan het begin van de dag de sliders in de website ging zetten had ik ze allemaal dezelfde IDs gegeven, element1, element2 enz. Dit mag natuurlijk niet dus had ik ze aangepast, maar ik had de bolletjes hun href niet mee verandert waardoor ze stuk gingen. Dit realiseerde ik me natuurlijk pas nadat ik Deanna een berichtje had gestuurd. 

<img src="images/nav_voor.png" width="375px" alt="nav voor mijn aanpassing">
<img src="images/nav_na.png" width="375px" alt="na na mijn aanpassing">

Ik heb ook mijn intersection observer bijgewerkt zodat hij het weer zou doen. De code die ik al gebruikte was nog niet goed geoptimaliseerd voor het gebruik van scroll-snap daarom ben ik gaan zoeken naar een ander voorbeeld die wel werkte.

https://codepen.io/michellebarker/pen/XwQXGv

Ik vond het fijne aan dit voorbeeld dat hij aparte functies had gemaakt voor het toevoegen en verwijderen van de class.

<img src="images/IO_oud.png" width="375px" alt="oude code van de intersection observer">
<img src="images/IO_nieuw.png" width="375px" alt="nieuwe code van de intersection observer">

Ik heb me de laatste dag bezig gehouden met alles netjes maken. Ik heb bijvoorbeeld de section animaties toegevoegd. Dit had ik de dag ervoor ook geprobeerd met een ::before en ::after maar dat lukte mij helaas niet. Daarom had ik op de laatste dag ervoor gekozen om dit toch te doen met een aparte div waar alle images in stonden. 

<img src="images/section_animatie_div.png" width="375px" alt="div waar de images van de section animatie in staan">

Er zijn een hele boel dingen die ik helaas nog niet uit heb kunnen werken omdat ik hier niet genoeg tijd voor over had. 

- De modal popup die opkomt als je op de detail button drukt in de profile section.
- Op mobiel zorgen dat je in het hamburger menu blijft als je hem opent doormiddel van tabben.
- Nav menu met dots aan de zijkant dat verandert op basis van welke section je zit. 
- Sticky menu dat met je mee scrollt.

### Screenshot(s)

Hieronder zijn de eindresultaten van mijn website te zien. Door de scroll-snap kan ik helaas mijn medium en large screen niet screenshotten, maar deze zijn gelukkig in mijn testomgeving te vinden. 

<img src="images/website_mobile.jpg" width="375px" alt="mijn website op mobiel">

</details>

## Bronnenlijst

<details open>
<summary>continu bijhouden terwijl je werkt</summary>

Nb. Wees specifiek ('css-tricks' als bron is bijv. niet specifiek genoeg).

1. https://developer.mozilla.org/en-US/docs/Web/API/Intersection_Observer_API
2. https://medium.com/elegant-seagulls/parallax-and-scroll-triggered-animations-with-the-intersection-observer-api-and-gsap3-53b58c80b2fa
3. https://stackhowto.com/how-to-remove-white-space-under-an-image-using-css/
4. https://developer.mozilla.org/en-US/docs/Web/CSS/:focus-within
5. https://developer.mozilla.org/en-US/docs/Web/API/Document/keydown_event
6. https://keycode.info/
7. https://www.sinds1971.nl/fed/bolletjes/index.html

</details>