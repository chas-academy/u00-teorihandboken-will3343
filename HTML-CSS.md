# Teorihandboken - HTML & CSS (HC)
Inlämningsdatum: 20231119   (Komplettering)

Studerande: 

### William Berhane 

### FWD-23 - Chas Academy

<br>

## Begrepp ord:

### CSS(stilmall) 
står för ***Cascading Style Sheet*** och ett programmering språk som stylar hur en hemsida ska se ut.

### Design
är ett metod där man i detalj fastställer hur ett system ska se ut innan man börjar realisera det.


### HTML
står för ***Hypertext Markup Language*** och ett språk man använder för att skriva och strukturera text, bilder och länkar på en hemsida. 

### Optimering 
är fastställande av det värde som ger det bästa utfallet för ett visst ändamål, till skillnad från det högsta värdet(maximering) eller det lägsta värdet (minimering).

### Responsiv
betyder att den anpassar sig med olika skärmstorlekar med hjälp av en flytande layout. 

### Tillgänglighet 
är det att en resurs i ett IT-system är möjligt att nå och att kommunicera med.

### Validering
kontroll av att något verkligenhar de egenskaper som det uppges eller förväntas ha. 

### Webb 
är där innehållet på hemsidorna till stor del skapas av användarna och är tillgängligt för alla.

>## HC 1.1 HTML <svg xmlns="http://www.w3.org/2000/svg" height="25" width="25" background-color="white" viewBox="0 0 384 512"><!--!Font Awesome Free 6.5.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2023 Fonticons, Inc.--><path d="M0 32l34.9 395.8L191.5 480l157.6-52.2L384 32H0zm308.2 127.9H124.4l4.1 49.4h175.6l-13.6 148.4-97.9 27v.3h-1.1l-98.7-27.3-6-75.8h47.7L138 320l53.5 14.5 53.7-14.5 6-62.2H84.3L71.5 112.2h241.1l-4.4 47.7z"/></svg>   & CSS    <svg xmlns="http://www.w3.org/2000/svg" height="25" width="25" viewBox="0 0 384 512"><!--!Font Awesome Free 6.5.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2023 Fonticons, Inc.--><path d="M0 32l34.9 395.8L192 480l157.1-52.2L384 32H0zm313.1 80l-4.8 47.3L193 208.6l-.3 .1h111.5l-12.8 146.6-98.2 28.7-98.8-29.2-6.4-73.9h48.9l3.2 38.3 52.6 13.3 54.7-15.4 3.7-61.6-166.3-.5v-.1l-.2 .1-3.6-46.3L193.1 162l6.5-2.7H76.7L70.9 112h242.2z"/></svg>

**HTML** står för "Hyper Text Markup Language" eller (extern stilmallar lagras i (.html)) och är det språk som alla webbsidor är byggda av. Det berättar hur en hemsida ska se ut och är alltså ett så kallat sidbeskrivningsspråk. Med hjälp av så kallade HTML-taggar kan du till exempel placera in bilder eller tabeller.

HTML5 är den senaste specifikationen för HTML-språket och representerade ett stort brott med tidigare uppmärkningsmetoder. Syftet med de djupgående förändringarna av språket var att standardisera de många nya sätt som utvecklare använde det på, samt att uppmuntra en enda uppsättning bästa praxis när det gäller webbutveckling.

De flesta av de individuella förändringarna är ett resultat av större mål i utformningen av språket. Dessa mål inkluderar främst:

- Uppmuntrande semantisk (meningsfull) uppmärkning
- Separera design från innehåll
- Främja tillgänglighet och designlyhördhet
- Minska överlappningen mellan HTML, CSS och JavaScript
- Stödja rika mediaupplevelser samtidigt som du eliminerar behovet av plugins som Flash eller Java
  
Att få grepp om HTML5 handlar inte bara om att lära sig vilka CSS-funktioner som ersätter gamla HTML-funktioner. Om du vill få en intuitiv känsla av HTML5 är det bäst att förstå hur dessa mål påverkade utvecklingen av språket.

#### Uppmuntrande semantisk uppmärkning (Encouraging Semantic Markup)

Semantisk markering betyder markering som har betydelse, snarare än markering som helt enkelt ser ut på ett visst sätt. Till exempel, `<h1>` - taggen antyder att innehållet i elementet är titeln eller rubriken för hela dokumentet. Den semantiska betydelsen skulle gå förlorad om vi bara gjorde texten fet och stor utan att använda lämplig tagg.

HTML har alltid haft lite semantisk markering tillgänglig för sig: `heading tags`, the `link rel attribute` och `document metadata`. Men det räckte inte.

I tidigare versioner av språket indikerades vanliga strukturella element som sidrubriker, navigeringsmenyer och huvudinnehållssektioner med samma HTML-element, taggen `<div>.` 
I HTML finns det en mängd nya semantiska element avsedda att indikera den grundläggande strukturen på en sida:



![Bild-1-HTML](/images/htmlT2.png)

HTML  har taggar,elements, attributes och där kan man skapa hemsida och redigera hemsida via olika sorts av TextEditor, Notepad, Notepad++ och andra framwork appar på windows, Mac och Linux.

Ett vanligt structurade HTML hemsida ser ut som: 

![Bild2-HTML-Structure](/images/HTML-structure.png)

Alla HTML- element har attribut:
   - href - attributet för `<a>` anger webbadressen till sidan som en länk går till. 
   - src - attributet för `<img>` anger sökvägen till bilden som ska visas. 
   - Bredd - och höjdattributen för `<img>` ger storleksinformation för bilder. 
   - Alt - attributet för `<img>` tillhandahåller en alternativ text för en bild. 
   - Style - attributet används för att lägga till stilar till ett element, som färg, teckensnitt, storlek med mera.
   - Lang - attributet för `<html>` - taggen deklarerar webbsidans språk. 
   - title - attributet definierar lite extra information om ett element. 

Nya element på textnivå (inline) har också introducerats, såsom `<adress>` och `<tid>`. Dessa hjälper sökmotorer och andra tjänster att enkelt hitta information på en sida, för visning i andra sammanhang. Samtidigt har befintliga inline-element som ger olika effekter som fetstil, kursiv och understruken förfinats eller omdefinierats för att antyda specifik semantisk betydelse.

#### Separera design från innehåll
Tillsammans med starkt uppmuntrande semantisk (meningsfull) uppmärkning, avråder HTML5-specifikationen starkt icke-meningsfull uppmärkning – uppmärkning som endast är avsedd att tala om för webbläsaren hur man visar saker. Detta inkluderar saker som:

- deklarerar teckensnitt och textfärger
- ställa in textjustering eller justering
- placera bårder på bord
- definiera hur text lindas runt bilder

De flesta HTML-funktioner som möjliggjorde den här typen av saker har blivit helt utfasade. De få som fortfarande stöds officiellt kommer med varningar om att de vanligtvis inte rekommenderas.

Det finns främst två skäl att föredra denna separation:

- Det är lättare att underhålla och designa om en webbplats om stildeklarationerna är begränsade till CSS
- Användare ser webbinnehåll i många olika sammanhang – stationära datorer, bärbara datorer, surfplattor, mobiltelefoner, RSS-läsare och många andra. Stilar och designbeslut som är vettiga i en miljö är inte alltid vettiga i en annan. Så det är mycket bättre att ge semantisk information och låta innehållet anpassas till sammanhanget.
  
Denna sista punkt är nära knuten till...

#### Främja tillgänglighet och designlyhördhet (Promoting Accessibility and Design Responsiveness)

Alla interagerar inte med webben på samma sätt som du gör.

"Konventionella" enheter – stationära datorer, bärbara datorer, surfplattor och telefoner – presenterar ett brett utbud av skärmstorlekar, bildformat, bildskärmsupplösningar och användarupplevelser. Enbart denna variation borde vara tillräckligt för att uppmuntra semantiska och responsiva designpraxis. Men inte alla använder en "konventionell" webbläsare.

Blinda och synskadade surfar också på nätet och de använder en mängd olika hjälpmedel för att göra det. Skärmläsare som översätter en webbplatss innehåll till tal, specialiserade webbläsare som tar bort stil och presenterar mycket förstorad eller högkontrasttext, punkttolkare och tangentbordsbaserad navigering tillåter alla med icke-standardiserad syn att interagera med webbplatser.

Och alla dessa tekniker hindras av uppmärkning som försöker "hårdkoda" design och styling i innehållet på en sida.

#### Minska överlappningen mellan HTML, CSS och JavaScript (Reducing the Overlap Between HTML, CSS, and Javascript)

Tre språk definierar front-end webbutveckling - `HTML`, `CSS` och `JavaScript`.

Ingen satte sig i början av internet och kom på vilka typer av saker som hör till respektive språk. De utvecklades var och en parallellt med varandra, ofta överlappande i funktionalitet och omfattning.

Förutom de praktiska överväganden som räknats upp ovan har det också funnits ett fokus på att definiera karaktären och syftet med dessa språk, och begränsa dem (eller utöka dem) så att de gör vad som ligger i deras natur att göra:

- HTML — Innehåll
- CSS — Design
- JS — Interaktivitet

> ### CSS

**CSS** står för "Cascading Style Sheets" (eller extern stilmallar lagras i .css) och används att beskriva hur HTML-element ska visas på skärmen, paper eller i andra media. Det viktigaste fördelen av CSS är att det sparar mycket arbete att styra layouten på fler webbsidor och app:ar. 

### Hur CSS fungerar

När man skriver CSS är det många gånger som regler skrivs som står i konflikt med varandra. Till exempel, när du formaterar rubriker, kan alla följande regler gälla för ett `h1`-element.

- En regel på elementnivå som skapar konsekvent `h1`-rendering på alla sidor på webbplatsen.
- En regel på klassnivå som definierar renderingen av `h1`-element som förekommer på specifika platser – till exempel titlarna på blogginlägg.
- Ett element på id-nivå som definierar renderingen av ett `h1`-element som används på bara ett ställe på en eller flera webbsidor – till exempel webbplatsens namn.
  
Hur kan en utvecklare skriva regler som är tillräckligt generella för att täcka varje `h1` men ändå tillräckligt specifika för att definiera stilar som bara ska visas på specifika instanser av ett givet element?

CSS-stilar följer två regler som du måste förstå för att skriva effektiv CSS. 

De två reglerna som styr hur CSS beter sig är arv och specificitet.

#### Cascading Arv

Varför kallas CSS-stilar cascading? När flera regler skrivs som står i konflikt med varandra, kommer den sist skrivna regeln att implementeras.

[Arv av stilar/ Inheritance of styles](https://developer.mozilla.org/en-US/docs/Web/CSS/inheritance) är ett annat exempel på överlappande beteende hos CSS-stilar.

När du definierar en stil för ett överordnat element får de underordnade elementen samma stil. Till exempel, om vi tillämpar färgstil på en oordnad lista, kommer de underordnade listobjekten att visa samma stilar. 

[Inte varje egenskap överförs från en överordnad till dess underordnade element](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Cascade_and_inheritance#inheritance). Webbläsare betraktar vissa egenskaper som icke-ärvda egenskaper. Marginaler är ett exempel på en egenskap som inte överförs från ett överordnat till ett underordnat element.

Ett vanligt css- strucuturad ser ut:
![Bild-3-CSS-Structure](/images/cssT2.png)

CSS har många Selectors och de mest grundläggande CSS-Selectors kan dela i fem kategorier:
   -  Simple selectors: (välj element baserat på `namn`, `id`, `klass`).
   -  Combinator selectors: (välj element baserat på ett specifikt förhållande mellan dem).
   - Pseudo-class selectors (välj element baserat på ett visst tillstånd).
   - Pseudo-elements selectors (välj och stil en del av ett element).
   - Attribute selectors (välj element baserat på ett attribut eller attributvärde).
  
En basic CSS-selectors exemplar:
![Bild-4-CSS-SELECTOR](/images/css-selectors.png)

### Specificitet

Den andra regeln som avgör vilka regler som tillämpas på varje HTML-element är [specificitetsregeln](https://developer.mozilla.org/en-US/docs/Web/CSS/Specificity).

CSS-regler med mer specifika väljare kommer att åsidosätta CSS-regler med mindre specifika väljare oavsett vad som inträffar först. Som vi diskuterade är de tre vanligaste väljarna elementtaggar, klasser och ID.

- Den minst specifika typen av väljare är elementnivåväljaren.
- När en klass används som väljare kommer den att åsidosätta CSS-regler skrivna med elementtaggen som väljare.
- När ett ID används som väljare kommer det att åsidosätta CSS-reglerna skrivna med element- eller klassväljare.
  
En annan faktor som påverkar specificiteten är platsen där CSS-stilarna skrivs. Stilar skrivna i linje med `Style` stilattributet åsidosätter stilar skrivna i en intern eller extern stilmall.

Ett annat sätt att öka specificiteten hos en väljare är att använda en serie element, klasser och ID:n för att lokalisera det element du vill adressera. Till exempel, om du vill peka ut oordnade listobjekt på en lista med klassen "exempel-lista" som innehåller en `div` med id:t "exempel-div" kan du använda följande väljare för att skapa en väljare med hög specificitet .
 
> div#example-div > ul.example-list > li {styles here}

Även om detta är ett sätt att skapa en mycket specifik väljare, rekommenderas det att begränsa användningen av dessa typer av väljare eftersom de tar längre tid att bearbeta än enklare väljare.

#### Vad kan CSS göra?
En bättre fråga kan vara: "Vad kan inte CSS göra?"

CSS kan användas för att förvandla ett HTML-dokument till en professionell, polerad design. Här är några av de saker du kan åstadkomma med CSS:

- Skapa ett flexibelt rutnät för att designa helt responsiva webbplatser som återges vackert på alla enheter.
- Style allt från typografi, till tabeller, till formulär och mer.
- Placera element på en webbsida i förhållande till varandra med hjälp av egenskaper som `float`, `position`, `overflow`, `flex` och `box-sizing`.
- Lägg till bakgrundsbilder till valfritt element.
- Skapa former, interaktioner och animationer.

Dessa koncept och tekniker går utöver den här inledande guiden, men följande resurser hjälper dig att ta itu med dessa mer avancerade ämnen.

#### Boxmodellen

Om du planerar att använda CSS för att bygga webbsideslayouter är ett av de första ämnena att bemästra boxmodellen. Boxmodellen är ett sätt att visualisera och förstå hur varje objekt på en webbsida är en kombination av innehåll, utfyllnad, kantlinje och marginal.

Att förstå hur dessa fyra delar passar ihop är ett grundläggande koncept som måste bemästras innan man går vidare till andra CSS-layoutämnen.

Två bra ställen att lära sig om boxmodellen inkluderar:

- En [förklaring av boxmodellen/explanation of the box model](https://www.w3.org/TR/CSS21/box.html) från World Wide Web Consortium.
- En [introduktion till CSS-boxmodellen/Introduction to the CSS box model](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Box_Model/Introduction_to_the_CSS_box_model) från Mozilla Developer Network.

#### Skapa layouter/ Creating Layouts

Det finns ett antal tekniker och strategier som används för att skapa layouter med CSS, och att förstå boxmodellen är en förutsättning för varje strategi.

Mozilla Developer Network erbjuder en [bra introduktion till CSS-layouter/Introduction to CSS layouts](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout). Denna korta läsning täcker de grundläggande begreppen bakom CSS-layouter och introducerar snabbt egenskaper som textjustering`text-align`, flytande`float` och position`position`.

En mycket mer omfattande och djupgående guide till CSS-layouter finns tillgänglig från W3C: CSS-layoutmodellen. Det här dokumentet är en resurs för professionella utvecklare, så om du är ny på CSS, ta dig tid att granska det. Det här är ingen snabb läsning. Men allt du behöver veta om att skapa CSS-layouter finns i det här dokumentet.

Grid-layouter har varit den vanligaste strategin för att designa responsiva layouter i flera år. CSS-grid har skapats från grunden i flera år och det finns många olika grid-genererande webbplatser och utvecklingsramverk på marknaden. Men inom några år kommer stöd för rutnätslayouter att vara en del av CSS3-specifikationen. Du kan lära dig mycket om rutnät genom att läsa om ämnet på W3C:s webbplats. För en lättare och kortare introduktion till rutnätslayouter, ta en titt på den här artikeln från Mozilla.
Inom några år förväntas CSS3 Flexible Box, eller flexbox, bli den dominerande modellen för att designa webblayouter. Flexbox-specifikationen är ännu inte helt komplett och slutförd, och stödet för flexbox är inte konsekvent mellan webbläsare. Men varje blivande CSS-utvecklare måste vara bekant med flexbox och beredd att implementera den inom en snar framtid. Mozilla Developer Network är ett av de bästa ställena att komma igång med flexbox.



## HC 1.2 Responsiv design

Responsiv design har ett unikt sätt att automatiskt anpassa designen på webbplatsen beroende på vilken enhet den visas på, och även om det tar lite arbete innan allt är konfigurerat och webbplatsen är helt anpassad, gör de enorma fördelarna det verkligen värt ansträngningen. Denna unika teknik gör att du sparar mycket tid och huvudvärk, och samtidigt kan du vara säker på att din sida kommer att se ut och fungera precis som du vill ha den, oavsett vilken enhet besökaren använder.


<img src="/images/responsiv.png" width="100%" height="50%">

Fördelar med responsiv-design:

- Snygg design för alla enheter och plattformar 
- Bättre för sökmotoroptimering 
- Billigare att utveckla en responsiv webbplats istället för flera för olika enheter 
- Användarupplevelsen förbättras 
- Förenklar administration och överblick 

Nackdelar är naturligtvis inte de enda fördelarna med att använda responsiv design:

-  Vissa delar av layouter kan vara svåra att göra responsiva. Avancerade tabeller är ett exempel. 
-  Ibland måste man kompromissa med estetiken. Funktion måste komma före estetik för att ytan ska vara lyhörd för att vara praktisk. 
-  Responsiva webbplatser kan ibland vara svårare att arbeta med i vissa publiceringsverktyg (CMS) eftersom det finns fler sidmallar att ta hänsyn till.
-  Om du jobbar mot målgrupper med väldigt gamla sajter kan de ha problem med responsiva sidor eftersom sajten kräver några nya kommandon för att hanteras.

## HC 1.3 Tillgänglighet inom webb

Webbtillgänglighet beskriver hur man gör webbinnehåll mer tillgängligt för personer med funktionsnedsättning. Tillgänglighet omfattar ett brett spektrum av funktionshinder, inklusive syn-, hörsel-, fysiska, tal-, intellektuella, språk-, inlärnings- och neurologiska funktionshinder. Även om dessa riktlinjer täcker ett brett spektrum av frågor, kan de inte tillgodose behoven hos människor med alla typer, grader och kombinationer av funktionshinder. Dessa riktlinjer gör webbplatsinnehåll mer användbart för äldre individer vars förmågor förändras på grund av åldrande och ofta förbättrar användarna överlag.

WCAG(Web Content Accessibility Guidelines) tas vissa standard fram W3C Web Accessibility Initiative:
  
- Märkbar - gör det enkelt för användare att se och höra innehåll etc.
- Manövrerbar - hjälp användare navigera och hitta innehåll etc. 
- Begriplig - hjälp användare att undvika och rätta till misstag etc.
- Robust - maximera kompabilitet med nuvarande och framtida användarverktyg.

## HC 1.4 Aktuella webbstandarder (gällande och kommande standarder)

Webbstandarder är rekommendationer från World Wide Web Consortium (W3C) och andra standardiseringsorgan, om hur webbaserat innehåll ska skapas och tolkas. Webbplatsstandarder har funnits sedan webbutvecklings gryning, och det är först på senare år som rekommendationerna har fått ett brett stöd över stora sajter.

Det finns att en hemsida följer för webbstandarder:

- Följer W3C:s rekommendationer 
- Använder giltig HTML eller XHTML 
- Använder CSS i stället för tabeller för layout 
- Har logiskt uppmärkt innehåll 
- är skapat för att fungera i alla webbläsare  

Webbstandarder syftar till att säkerställa hållbarheten hos information som publiceras på webben, vilket gör den tillgänglig för så många webbanvändare som möjligt. Webbplatser som utformats för att följa webbläsarstandarder kommer att fortsätta att fungera korrekt även på nya webbläsare.

## HC 1.5 CSS Pre-processorer (ex SASS/LESS)

Det finns tre primära CSS-Preprocessorer på marknaden idag, `Sass` , `Less`  och `Stylus`. I det här inlägget kommer vi att jämför de två preprocessorerna som verkar vara de mest använda bland utvecklare, Sass vs Less. Genom att byta en pre-processorn kan hjälpa till att effektivisera din utvecklingsprocess.
En CSS pre-processorn är i grunden ett skriptspråk som utökar CSS och sedan kompilerar det till vanlig CSS. 

En vanlig Sass kod:

![Bild-6-Sass](/images/sass.png)

#### Sass Vs Less

Sass och Less är båda mycket kraftfulla CSS-tillägg. Du kan tänka på dem som mer av ett programmeringsspråk som är utformat för att göra CSS mer underhållbar, teman och utbyggbar. Både Sass och Less är bakåtkompatibla så att du enkelt kan konvertera dina befintliga CSS-filer bara genom att byta namn på `.css` filtillägget till `.less` eller `.scss` respektive. Less är JavaScript baserat och Sass är Ruby baserat.  

## HC 1.6 Optimering och validering av HTML & CSS

Optimering, sökmotoroptimering eller positionering betyder att utveckla webbsidor så att de blir sökbara och att de verkligen hitta via sökmotorer på Internet. Webbsökaren letar efter en produkter eller en service på de förtsa  fem sidorna som en sökmotor visar oss optimering hjälper att placera dina sidor på de första fem sidorna på sökmotorerna. Optimering är den enda tekniken för webbsidor för att hitta nya besökare och klienter.

#### Hur optimerar man en webbsida för sökmotorerna

För att optimera webbsidor, så att de blir sökbara och för att webbesökaren ska hitta dem via sökmororer, behövs en webbteknik som anpassar sidorna till en algoritm med över 100 parameter. Detta börjar med en logisk hierarkisk strukturav en webbsida och en valid kod, fortsätter med web copywriting, redaktionen från länktexter och slutar sedan med att använda kunskapen av internet marketing.

Validering är att kontrollera att man följer aktuella standarer för HTML och CSS.
Hur kan man då validera en webbsida? Inget är enklare än en validering. Med hjälp av W3C-Validatoren kan varje webbmaster validera sina sidor, redan i början av utvecklingen och korrigera alla fel innan de kan komma att förorsaka problem. En validator är inget annat än en korrigerare för rättstavning och grammatik, som alla textprogram har. Skillnaden är endast att validatoren inspekterar koden `HTML` och `xhtml` och inte rättstavningen. En validator hjälper också nybörjaren att skriva den rätta koden.

En vanlig och mest känd HTML och CSS validation hemsida.
![Bild-7-HTML-validator](/images/html_validate.png)

Anledningen till validering är egentligen för att vi begår misstag. Därför att validering hjälper oss att enkelt fånga enkla misstag och snedsteg utan större huvudvärk. 

En vanlig och mest känd CSS och HTML validation hemsida.
![Bild-8-CSS-validator](/images/css_validate.png)

Naturligtvis, det är inte bara de här sidorna förutom det finns också många andra hemsidor som validerar HTML och CSS. 

<hr>

Källor:


https://www.w3schools.com/html/
https://www.svenskwebbhandel.se/blogg/vad-ar-html/1252
https://www.west-tech.se/vanliga-begrepp-inom-webbdesign/
https://webbyra-wordpress.se/responsive-design/
https://www.webbdesignguiden.se/responsiv-design/
https://responsivwebbdesign.wordpress.com/2013/07/05/10-nackdelar-med-responsive-web-design/
https://www.w3.org/TR/WCAG21/#time-based-media
https://www.happiness.se/artiklar/vad-ar-webbstandarder
http://validator.w3.org/
https://www.webbdesign-karlin.se/validator.html

[Responsive design bild källa](https://images.app.goo.gl/Jh4MJwtgAeqfVRU9A ) 

