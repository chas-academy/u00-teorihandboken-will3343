<div class="name">

# Teorihandboken - Avancerad JavaScript (AJ)

Inlämningsdatum: 2024

Studerande: 

### William Berhane 

### FWD-23 - Chas Academy

</div>

<br>
<style>
    .blue{
        background-color: #AED6F1 ;
        color: #34495E;
        font-style: Roboto;
    }
    .begrepp{
        background-color: #5D6D7E  ;
        color: #34495E;
        font-style: Roboto;
    }
    .name{
       background-color: #212F3C;
        color: white;
        font-style: Roboto;
    }
</style>

<div class="begrepp"> 

## Begrepp ord:

### Node 
         är en grundläggande datastruktur som innehåller data och en eller flera länkar till andra noder.

### Typingssystem 
         gör det möjligt att definiera gränssnitt mellan olika delar av ett datorprogram och sedan kontrollera att delarna har kopplats samman på ett konsekvent sätt.

### Javascript
         är ett skriptspråk som används för att utveckla webbsidor.

### Integrerade System 
         innebär att flera olika fristående system kopplas ihop för att fungera tillsammans.

### Operativesystem 
         (OS) är det program som, efter att ha laddats in i datorn av ett startprogram, hanterar alla andra applikationsprogram i en dator.

  
   </div>      

<div class="blue">

## AJ 1.1 Node.js

Node.js är en JavaScript-runtimemiljö med öppen källkod och plattformsoberoende. Det är ett populärt verktyg för nästan alla typer av projekt!

En Node.js-app körs i en enda process, utan att skapa en ny tråd för varje begäran. Node.js tillhandahåller en uppsättning asynkrona I/O-primitiver i sitt standardbibliotek som förhindrar JavaScript-kod från att blockera och generellt skrivs bibliotek i Node.js med hjälp av icke-blockerande paradigm, vilket gör blockeringsbeteende till undantag snarare än norm.

När Node.js utför en I/O-operation, som att läsa från nätverket, komma åt en databas eller filsystemet, istället för att blockera tråden och slösa CPU-cykler på att vänta, kommer Node.js att återuppta operationerna när svaret kommer tillbaka.

Detta gör att Node.js kan hantera tusentals samtidiga anslutningar med en enda server utan att införa bördan av att hantera trådsamtidighet, vilket kan vara en betydande källa till buggar.

Node.js skapades för att ta itu med begränsningarna hos traditionella server-side-teknologier, såsom ett högt samtidighetskrav, långsamma I/O-operationer och blockerande kodexekvering. Det syftade till att tillhandahålla en plattform som är mycket skalbar, effektiv och kapabel att hantera ett stort antal samtidiga anslutningar.

### Huvudfunktioner i Node.js

- Asynkrona och icke-blockerande I/O-operationer
- Händelsedriven arkitektur
- Enkeltrådad händelseslinga
- Skalbarhet och hög samtidighet
- Effektivt modulsystem med npm (Node Package Manager)
- Plattformsöverskridande kompatibilitet

Node.js följer en modulär arkitektur, där varje modul utför en specifik uppgift och kan kombineras för att skapa komplexa applikationer. Kärnmodulerna hanterar lågnivåoperationer, medan ytterligare moduler kan installeras med npm för att utöka funktionaliteten i Node.js-applikationer.

![Bild-1-Node](/images/js/node.png)

En av de definierande egenskaperna hos Node.js är dess händelsedrivna arkitektur, vilket innebär att den kan hantera flera samtidiga operationer utan att blockera exekveringen av andra uppgifter. Detta uppnås genom icke-blockerande I/O, där in- och utgångsoperationer utförs asynkront, vilket gör att programmet kan fortsätta att utföra andra uppgifter i väntan på att I/O-operationer ska slutföras.

Node.js följer en enkeltrådad händelseloopmodell, där en enda tråd ska hantera alla förfrågningar och återuppringningar. Denna händelseslinga letar kontinuerligt efter nya händelser och utför callbacks när händelser inträffar och går vidare till nästa händelse. Även om det kan verka kontraintuitivt att ha en enda tråd, utnyttjar Node.js sin icke-blockerande I/O-modell för att hantera flera samtidiga anslutningar effektivt.

Node.js utmärker sig i att bygga skalbara applikationer på grund av dess händelsedrivna, icke-blockerande karaktär. Den kan hantera ett stort antal samtidiga anslutningar med begränsade resurser, vilket gör den idealisk för realtidsapplikationer, chattapplikationer och streamingplattformar. Dessutom stöder den klustring av flera processer för att ytterligare förbättra prestanda och skalbarhet.

Node.js använder ett modulsystem som låter utvecklare organisera sin kod i återanvändbara moduler. Dessa moduler kan delas och användas av andra utvecklare genom npm, den officiella pakethanteraren för Node.js. npm är värd för tusentals moduler som ger ytterligare funktionalitet, vilket gör det lättare att snabbt bygga komplexa applikationer.

Node.js tillhandahåller flera verktyg och ramverk för att testa och felsöka applikationer. Populära ramverk som Mocha, Jasmine och Jest kan användas för att skriva enhetstester, medan debuggers som Node Inspector och ndb låter utvecklare gå igenom sin kod och identifiera potentiella problem och flaskhalsar.

### Användningsfall av Node.js

Node.js har ett brett utbud av användningsfall, inklusive:

- Chattapplikationer i realtid
- Strömmande plattformar
- Samarbetsverktyg
- Mikrotjänster arkitektur
- RESTfulla API:er
- Ensidiga applikationer
- Internet of Things (IoT) applikationer


Node.js är känt för sin exceptionella prestanda och skalbarhet. På grund av dess händelsedrivna och icke-blockerande I/O-karaktär kan Node.js hantera ett stort antal samtidiga anslutningar och utföra I/O-operationer effektivt. Det är dock viktigt att designa och optimera applikationer noggrant för att säkerställa optimal prestanda.

Även om Node.js tillhandahåller kraftfulla funktioner, bör säkerheten inte förbises. Det är avgörande att validera och sanera användarinmatning, skydda mot vanliga sårbarheter som cross-site scripting (XSS) och SQL-injektion, och följa bästa praxis för autentisering och auktorisering. Dessutom är regelbunden övervakning och uppdateringar viktiga för att åtgärda säkerhetsbrister i beroenden.

Node.js är en spelväxlare i världen av utveckling på serversidan, och erbjuder en effektiv och skalbar plattform för att bygga högpresterande applikationer. Dess händelsedrivna, icke-blockerande I/O-modell, tillsammans med ett stort ekosystem av moduler, gör den till ett populärt val bland utvecklare. Genom att utnyttja Node.js kan utvecklare dra fördel av JavaScripts mångsidighet och bygga robusta applikationer som kan hantera ett stort antal samtidiga användare.


## AJ 1.2 Express

Express.js är ett snabbt, flexibelt och minimalistiskt webbramverk för Node.js. Det är faktiskt ett verktyg som förenklar att bygga webbapplikationer och API:er med JavaScript på serversidan. Express är en öppen källkod som utvecklas och underhålls av Node.js-stiftelsen.

Express.js erbjuder en robust uppsättning funktioner som förbättrar din produktivitet och effektiviserar din webbapplikation. Det gör det lättare att organisera din applikations funktionalitet med mellanprogram och routing. Det lägger till användbara verktyg till Node HTTP-objekt och underlättar renderingen av dynamiska HTTP-objekt.

![Bild-2-Express](/images/js/express.jpeg)

[Express](https://expressjs.com/) är ett användarvänligt ramverk som förenklar utvecklingsprocessen för Node-applikationer. Den använder JavaScript som programmeringsspråk och ger ett effektivt sätt att bygga webbapplikationer och API:er. Med Express kan du enkelt hantera rutter, förfrågningar och svar, vilket gör processen att skapa robusta och skalbara applikationer mycket enklare.

Dessutom är det ett lätt och flexibelt ramverk som är lätt att lära sig och kommer laddat med mellanprogramsalternativ. Oavsett om du är nybörjare eller erfaren utvecklare är Express ett utmärkt val för att bygga din applikation.

Express nyckelfunktioner
- Middleware och routing: Express.js gör det enkelt att organisera din applikations funktionalitet med hjälp av middleware och routing. Middleware-funktioner låter dig hantera uppgifter som autentisering, loggning och felhantering. Routing säkerställer att inkommande förfrågningar riktas till lämpliga hanterare.
- Minimalistisk design: Express.js följer en enkel och minimalistisk designfilosofi. Denna enkelhet gör att du snabbt kan konfigurera en server, definiera rutter och hantera HTTP-förfrågningar effektivt. Det är ett utmärkt val för att bygga webbapplikationer utan onödig komplexitet.
- Flexibilitet och anpassning: Express.js kräver inte en strikt applikationsarkitektur. Du kan strukturera din kod enligt dina preferenser. Oavsett om du bygger ett RESTful API eller en fullfjädrad webbapp, anpassar Express.js sig efter dina behov.
- Skalbarhet: Designad för att vara lätt och skalbar, Express.js hanterar ett stort antal förfrågningar asynkront. Dess händelsedrivna arkitektur säkerställer lyhördhet även under tunga belastningar.

Hur man skapar ett express projekt app 

![Bild-3-Node](/images/js/installEX.png)

Webbapplikationer kommer en webbserver att vänta på att HTTP-förfrågningar ska skickas från klienten. Vid mottagande av en HTTP-begäran kommer servern att välja motsvarande rutthanterare och delegera ytterligare åtgärder till den för den begäran. Normalt kan det vara lite betungande att skriva en rutthanterare från början i Node. Lyckligtvis tillhandahåller Express metoder för att specificera vilken funktion som kallas för ett visst HTTP-verb (GET, POST, PUT, etc.) och URL-mönster (Route). Ett exempel på en Express-rutt visas i kodavsnittet nedan. Här deklarerar Express att alla GET-förfrågningar som görs till rutten, /, kommer att hanteras med en funktion som svarar klienten med "Hello World!"

```
    const express = require('express');
    const app = express();
    const port = 3000;

    app.get('/', (req, res) => res.send('Hello World!')); 

    app.listen(port, () => console.log (`Example app at http://localhost:${port}`));

```

## AJ 1.3 Progressive Web Apps

Progressiva webbapplikationer (PWA) är appar byggda med webbteknologier som vi förmodligen alla känner till och älskar, som HTML, CSS och JavaScript. Men de har känslan och funktionaliteten som en verklig inbyggd app. Vänta en minut! Native Apps, vad menar vi med detta?

En Native App är en mjukvaruapplikation byggd i ett specifikt programmeringsspråk för en specifik enhetsplattform, antingen IOS eller Android.
PWA är byggda med funktioner som push-meddelanden och möjligheten att arbeta offline. De är också byggda på och förbättrade med moderna API:er som gör det enkelt att leverera förbättrade funktioner tillsammans med tillförlitlighet och möjligheten att installera dem på vilken enhet som helst.

PWA:er drar fördel av det enorma webbekosystemet som detta inkluderar plugins och community och den relativa lättheten att distribuera och hålla en webbplats i motsats till en inbyggd applikation som är ganska svår att utveckla. Det betyder att du kan bygga en PWA snabbt och enkelt.

En vanlig funktion med dessa produkter är att de alla är installerade på din hemskärm, kan arbeta offline från där du senast lämnade och erbjuder en jämförbar upplevelse och funktioner till deras inhemska appar.

Precis som när man bygger en inbyggd mobilapp finns det vissa förväntningar som bör uppfyllas för att göra en bra produkt för konsumentbruk, samma sak gäller PWA:er. Låt oss diskutera vad som gör en bra PWA.

Karakteristika för PWA
Nedan är vad man bör tänka på när man utvecklar en PWA:

- Lyhördhet
- Installerbar
- Oberoende anslutning
- Upptäckbarhet
- Utseende
- Cross Platform


### Skillnader mellan PWA:er och inbyggda appar

- Utvecklingskostnad

PWA:er är billigare att utveckla jämfört med Native AppsNär du utvecklar en inbyggd app måste du lära dig ett visst programmeringsspråk och sedan bygga en version av appen för varje typ av enhet, Android och iOS. Å andra sidan kan du välja att anlita en erfaren fackman för att göra jobbet åt dig, vilket till och med kommer att visa sig vara dyrare.

På vägen kommer du också att behöva resurser för att underhålla och uppdatera appen, vilket innebär att det krävs mycket pengar och tid.

I fallet med en PWA kan du ha en enda kodbas för de olika plattformarna. Det är också tidsbesparande eftersom du inte behöver utveckla den från början, du kan konfigurera din nuvarande webbplats så att den passar.

Och om du väljer att anlita utvecklare blir det bara en jämfört med native där du kan anställa upp till två beroende på var du behöver din app.

- Upptäckbarhet

Native appar kan inte indexeras av sökmotorerna, de kan bara hittas via App/Play-butikens webbplats. Du kan göra din app mer upptäckbar i App/Play Store genom att använda App Store Optimization (ASO), men det är en annan historia.

### Fördelar med PWA

Många organisationer, både privata och offentliga, byter till PWA inte bara för att de är billiga att utveckla utan också för att de erbjuder ett större engagemang.
Låt oss nu titta på en snabb sammanfattning av fördelarna med en PWA:

- De är lyhörda och fungerar med många olika skärmstorlekar.
- De kan köras på flera plattformar och vilken enhet som helst med en modern webbläsare.
- De fungerar precis som vanliga inbyggda appar.
Uppdateringarna är oberoende, du behöver inte besöka play store för en uppdatering.
- De är byggda med vanliga webbteknologier.
- De är snabba och lätta.
- De fungerar offline till skillnad från andra webbplatser.
- De kan upptäckas via sökmotorn.
- De är lätta att installera.
- Låg underhållskostnad.

### Krav för att komma igång med PWA Development

Det krävs inte mycket för att komma igång med att bygga en PWA. Du behöver bara några saker och du är redo att gå.

- Verktyg

Den mest kända teknikstacken för att utveckla PWA är AngularJS. På tal om Angular, här är en fyndig guide om hur du kan konvertera din redan befintliga Angular-app till PWA. Andra stackar inkluderar ReactJS och Polymer.

- HTTPS

Du behöver en server med en HTTPS-anslutning. Detta säkerställer att din användares data är säker. Det lägger till ett extra lager av säkerhet till din webbplats.

- Applikationsskal

Det ger ett bra första intryck när din app laddas. Med enklare ord är detta vad användaren ser när de interagerar med din app för första gången.

- Servicearbetare

Detta är en av nyckelteknologierna bakom PWA. De hjälper till att stödja ditt apparbete offline, och de utför avancerad cachelagring och kör bakgrundsuppgifter. Servicearbetare kan utföra uppgifter även när din PWA inte körs. Några andra funktioner som är associerade med Service Worker inkluderar:

- Skickar push-meddelande
- Badging ikoner
- Kör bakgrundshämtning osv...

### Manifestfil

Detta är en JSON-fil som skapas med en [Web App Manifest Generator.](https://app-manifest.firebaseapp.com/) Den här filen innehåller informationen som talar om hur din PWA ska se ut och fungera. Det låter dig bestämma namn, beskrivning, ikon, färger och andra funktioner för din PWA.

## AJ 1.4 Typningssystem för Javascript (ex TypeScript, Flow)

I JavaScript rapporteras alla typfel vid körning. Den största fördelen är en syntax som är lätt att lära sig och använda, men det kostar pengar. När ett projekt växer och mognar kan bekvämligheten med dynamisk typning ge vika för frustration med kodkvalitet och underhållsbarhet. Den här artikeln introducerar en lågfriktionslösning, typad JavaScript.

Skrivet Javascript är ett system med verktyg och metoder som avslöjar typfel före körning. Till skillnad från andra alternativ körs Skrivet JavaScript utan ändringar varhelst JavaScript körs. Skrivet JavaScript erbjuder statisk typkontroll, utan kompilatorer eller ovanliga verktyg. Du kan använda så mycket eller så lite Skrivet JavaScript som du vill. Om saker och ting inte fungerar är ändringar lätta att återställa.

För att få en uppfattning om hur Skrivet JavaScript fungerar, överväg en funktion som lägger till två siffror.

```
   const add = (i, j) => {
        return i + j;
   };
```

Även om syftet med tillägget är numeriskt tillägg, accepterar JavaScript ovillkorligen argument av vilken typ som helst för parametrarna i och j. Vad händer om det första argumentet är en sträng istället för ett tal? Vi kommer inte att få ett fel, men vi kommer förmodligen inte att få vad vi är ute efter heller.

```
    console.log(add(4, 5))     // => 9 
    console.log(add('4', 5))   // => '45'
```

Det är lätt att fånga felet genom inspektion i detta enkla exempel eftersom båda argumenten är bokstavliga och implementeringen av add är en enda rad. Men i komplexa JavaScript-projekt kan argument och returvärde separeras av flera funktionsanrop. Detta avstånd i tid och rum kan göra felsökning mycket svårt.

Även om ett typfel kan spåras är det knappast enkelt att förhindra att det upprepas. För att eliminera alla möjliga typfel kan vi lägga till vaktkod som i följande exempel. Ändå är det bästa vi skulle få körtidsmeddelanden om ett fel. Användaren skulle fortfarande möta de fulla konsekvenserna av det felet.

```
     const addWithCheck = (i, j) => {
        if (typeof i !== 'number' ||  typeof j !== 'number') {
            throw new Error ('arguments must be numbers or number');
        }

        return i + j;
     }; 
```

Typed JavaScript löser detta problem genom typkommentarer (alias "typtips"). En typanteckning begränsar intervallet av typer som ett givet värde kan anta. Skrivet JavaScripts anteckningar implementeras genom taggade [JSDoc](https://jsdoc.app/) - kommentarer. Till exempel kan intervallet av tillåtna in- och utgångar för tilläggsfunktionen begränsas på så sätt.

```
   /**
   * @param {number} i
   * @param {number} j
   * @param {number}
   */

   const addSafely = (i, j) => {
    return i + j;
   };
```

Med rätt verktyg kommer typfel som involverar addSafely-funktionen att bli synliga när du skriver. [Visual Studio Code,](https://code.visualstudio.com/) till exempel, stöder interaktiv typcheckning ur lådan.


## Typescript

TypeScript ger en mycket rik verktygslåda. Det inkluderar mappade typer, villkorstyper med kontrollflödesbaserad analys, typinferens och många fler.

Det är inte en lätt uppgift för många JavaScript-utvecklare som är nya för TypeScript att byta från löst skrivande till statiskt skrivande. Även för utvecklare som har arbetat med TypeScript i flera år kan det vara förvirrande eftersom skrivsystemet kontinuerligt utvecklas.

![Bild-4-TypeScript](/images/js/typescript.jpeg) 

En vanlig myt om avancerade typer är att den främst ska användas för att bygga typbibliotek och inte krävs för det dagliga TypeScript-arbetet.

Sanningen är att avancerade TypeScript-typer är mycket användbara för dagligt TypeScript-arbete. De är ett bra verktyg för att bygga ett starkt skrivet system i din kod, uttrycka dina avsikter tydligt och göra din kod säkrare.

Syftet med att introducera konceptet typflöde är att tänka på typsystemet på ett sätt som liknar hur vi tänker om reaktivt programmeringsdataflöde.

Genom att se på skrivsystemet ur ett nytt perspektiv kommer det att hjälpa oss att "tänka i typer" och använda de mer avancerade verktygen i TypeScript-verktygslådan på ett systematiskt sätt.

### Typer kan flöda

Vid reaktiv programmering flyter data mellan reaktiva komponenter. I TypeScript-skrivsystemet kan typer också flyta.

Första gången jag stötte på konceptet "Type flowing" var i Basarat Ali Syeds TypeScript-bok. Han förklarar denna idé på följande sätt:

```Typerna som flödar är precis hur jag föreställer mig flödet av typinformation i min hjärna.```

Inspirerad av detta ville jag utöka konceptet typflöde till typsystemnivån. Min definition av typ flytande är:

```Typflöde är när en eller flera undertyper mappas och transformeras från en källtyp. Dessa typer bildar ett starkt begränsat typsystem genom typoperationer.```

Den grundläggande formen av typflöde kan göras via typalias.

Typalias låter dig skapa ett nytt typnamn för en befintlig typ. I exemplet nedan är typaliaset TargetType tilldelat som en referens till SourceType, så typen överförs.

```typ SourceType = { id: string, quantity: number };```
```typ TargetType= SourceType; // { id: sträng, kvantitet: antal };```

Tack vare kraften i typinferenser kan typer flyta på några olika sätt. Dessa inkluderar:

- Genom datatilldelning
- Med returtypsfunktionen, som härleds av retursatserna; t.ex. antas följande funktion returnera en nummertyp
- Mönstermatchning med funktionsparametrar: som illustreras i exemplet nedan, omvandlar minskningsfunktionen med typen "DecreaseType" värdet a,b till en taltyp


Flow utvecklas och underhålls av Facebook. Det är en statisk typkontroll, utformad för att snabbt hitta fel i JavaScript-applikationer. Varken mer eller mindre. Det är inte en kompilator, utan en checker. Det kan fungera utan någon typ av anteckningar och det är väldigt bra på att sluta sig till typer. För att aktivera skriv checking in [flow](https://flow.org/) lägg till // @flow överst i filen. Den kontrollerar typer lokalt och har ingen språkserver eller typdefinitioner som TypeScript.

|   S.N°            |FLOW       |TYPESCRIPT    |
|---------------|---------------|--------------|
| 1.    | Det utvecklades av Facebook 2014.  |  Det utvecklades av Microsoft 2012.  |
| 2.    | Huvudfunktionerna i Flow är Precision, Realtidsfeedback, Lätt att integrera, Tillförlitlighet, Hastighet, Hög genomströmning, Sökvägskänslighet, Låg latens, Typinferens, Lättförståeliga JavaScript-mönster.  |  Huvudfunktionerna i Typescript är typkontroll vid kompilering, Uppräknad typ, Gränssnitt, Namnutrymmen, Typkommentarer, Typradering, Typinferens, Generisk, Tuples. |
| 3. | Dess verktygsstorlek är 68,4 MB.   | Dess verktygsstorlek är 42,4 MB.  |
| 4. | Det är det bästa valet vi arbetar med React eftersom det enkelt integreras med babel och den redan befintliga infrastrukturen. | Det är det bästa valet när vi arbetar med Angular 2 eller högre versioner. |  
| 5. | Det stöder inte riktigt inkapsling. | Den stöder inkapsling med offentliga, privata, skyddade modifierare och skrivskyddad sedan TypeScript 2.0. | 
| 6. | Det stöds endast av React. |  Det är mycket bättre eftersom det stöder stora frontend-ramverk som Vue, Angular och Facebooks egna React. |
| 7. | Det stöder väldigt få bibliotek. | Det stöder många bibliotek. |
| 8. | Tillsammans med tillhandahållandet av statisk typning ger det oss också ett brett utbud av inter-proceduranalys och utvecklar en djupgående förståelse av vår kod. | Tillsammans med tillhandahållandet av statisk typning ger det oss också fantastiska språktjänster och lämpliga verktyg som inkluderar kodrefaktorering, navigering och autokomplettering. |
||||


Två alternativ till Skrivet JavaScript är tillgängliga: [Typescript](https://www.typescriptlang.org/) och [Flow](https://flow.org/). Båda närmar sig problemet med typer i JavaScript genom att introducera en kompilator och anpassad syntax. Båda delar samma mål som Typed Javascript, nämligen att lägga till typsäkerhet till JavaScript. Flow och Typescript är dock distinkta språk. Varken kan köras i en webbläsare eller av Node.js. Det obligatoriska kompileringssteget gör Flow och TypeScript svårare att använda i vissa situationer än Typat JavaScript.

Skrivet JavaScript är ett löstagbart typsystem som tar statisk typkontroll till JavaScript. I motsats till alternativ som Typescript och Flow kräver typad JavaScript inget kompileringssteg och stöds ändå direkt av populära verktyg som VS Code. Om du gillar idén med statisk typkontroll och vill fortsätta använda JavaScript är typad JavaScript värt att överväga. En framtida artikel kommer att diskutera Typed JavaScripts typsystem i detalj.


## AJ 1.5 Funktionell programmering i JavaScript

Funktionell programmering är ett paradigm för att bygga datorprogram med hjälp av uttryck och funktioner utan att mutera tillstånd och data.

Genom att respektera dessa begränsningar syftar funktionell programmering till att skriva kod som är tydligare att förstå och mer felbeständig. Detta uppnås genom att undvika att använda flödeskontrollsatser (```for,```  ```while,```  ```break,```  ```continue,```  ```goto```) som gör koden svårare att följa. Funktionell programmering kräver också att vi skriver rena, deterministiska funktioner som är mindre benägna att vara buggiga.

I den här artikeln kommer vi att prata om att göra funktionell programmering med JavaScript. Vi kommer också att utforska olika JavaScript-metoder och funktioner som gör det möjligt. I slutändan kommer vi att utforska olika koncept förknippade med funktionell programmering och se varför de är så kraftfulla.

Innan man börjar med funktionell programmering måste man dock förstå skillnaden mellan rena och orena funktioner.

### Ren vs. orena funktioner

Rena funktioner tar viss input och ger en fast utgång. Dessutom orsakar de inga biverkningar i omvärlden.

```
    const add = (a,b) => a + b;
```

Här är ```add``` en ren funktion. Detta beror på att för ett fast värde på ```a``` och ```b``` kommer utsignalen alltid att vara densamma.

```
const SECRET = 42;
const getId = (a) => SECRET * a;
```

```getId``` är inte en ren funktion. Anledningen är att den använder den globala variabeln ```SECRET``` för att beräkna utdata. Om ```SECRET``` skulle ändras kommer ```getId```-funktionen att returnera ett annat värde för samma ingång. Det är alltså inte en ren funktion.

```
låt id_count = 0;
const getId = () => ++id_count;
```

Detta är också en oren funktion, och det också av ett par anledningar—(1) den använder en icke-lokal variabel för att beräkna dess utdata, och (2) den skapar en bieffekt i omvärlden genom att modifiera en variabel i det värld.

```
          getId() =>  1 
```

### Grundsatserna för funktionell programmering

Hittills har vi lärt oss att funktionell programmering är beroende av några regler. De är följande.

1. Mutera inte data
2. Använd rena funktioner: fast utgång för fasta ingångar och inga biverkningar
3. Använd uttryck och deklarationer
När vi uppfyller dessa villkor kan vi säga att vår kod är funktionell.

### Funktionell programmering i JavaScript

JavaScript har redan några funktioner som möjliggör funktionell programmering. Exempel: ```String.prototype.slice,```  ```Array.protoype.filter,```  ```Array.prototype.join.```

Å andra sidan är ```Array.prototype.forEach,``` ```Array.prototype.push``` orena funktioner.

Man kan hävda att Array.prototype.forEach inte är en oren funktion till sin design men tänk på det – det är inte möjligt att göra något med det förutom att mutera icke-lokal data eller göra biverkningar. Därför är det okej att placera det i kategorin orena funktioner.

JavaScript har också en const-deklaration, som är perfekt för funktionell programmering eftersom vi inte kommer att mutera några data.

### Rena funktioner i JavaScript

Låt oss titta på några av de rena funktionerna (metoderna) som ges av JavaScript.

### Filtrera

Som namnet antyder filtrerar detta arrayen.

``` 
array.filter(condition); 
```
Villkoret här är en funktion som hämtar varje objekt i arrayen, och det bör avgöra om objektet ska behållas eller inte och returnera det sanna booleska värdet för det.
```
const filterEven = x => x%2 === 0;
[1, 2, 3].filter(filterJämnt);
// [2]
```

Lägg märke till att filterEven är en ren funktion. Om det hade varit orent, då hade det gjort att hela filtret kallades orent.

### Karta

```map``` mappar varje objekt i array till en funktion och skapar en ny array baserat på returvärdena för funktionsanropen.

```
array.map(mapper)
```

mapper är en funktion som tar ett objekt i en array som indata och returnerar utdata.
```
const dubbel = x => 2 * x;
[1, 2, 3].map(dubbel);
// [2, 4, 6]
```

### Minska

reduce reducerar matrisen till ett enda värde.

```
array.reduce(reducer);
```

reducer är en funktion som tar det ackumulerade värdet och nästa objekt i arrayen och returnerar det nya värdet. Det kallas så här för alla värden i arrayen, en efter en.

```
const summa = (ackumuleradSumma, arrayItem) => accumulatedSum + arrayItem
[1, 2, 3]. reducera(summa);
// 6
```

### Concat

concat lägger till nya objekt till en befintlig array för att skapa en ny array. Det skiljer sig från push() i den meningen att push() muterar data, vilket gör det orent.

```
[1, 2].concat([3, 4])
// [1, 2, 3, 4]
```

Du kan också göra samma sak med spridningsoperatorn.

```
[1, 2, ...[3, 4]]
```

### Objekt.tilldela

Object.assign kopierar värden från det angivna objektet till ett nytt objekt. Eftersom funktionell programmering bygger på oföränderlig data, använder vi den för att skapa nya objekt baserat på befintliga objekt.

```
const obj = {a: 2};
const newObj = Object.assign({}, obj);
newObj.a = 3;
obj.a;
// 2
```

Med tillkomsten av ES6 kan detta också göras med spridningsoperatorn.

```
const newObj = {...obj};
```


Vi kan skapa vår rena funktion också. Låt oss göra en för att duplicera en sträng ett antal gånger.
```
const duplicate = (str, n) =>
n < 1 ? '' : str + duplicate(str, n-1);
```

Denna funktion duplicerar en sträng n gånger och returnerar en ny sträng.
```
duplicate('hurra!', 3)
// hurra!hurra!hurra!
```

### Funktioner av högre ordning

Funktioner av högre ordning är funktioner som accepterar en funktion som ett argument och returnerar en funktion. Ofta används de för att lägga till funktionaliteten hos en funktion.

```
const withLog = (fn) => {
return (...args) => {
console.log(`ringer ${fn.name}`);
returnera fn(...args);
};
};
```

I exemplet ovan skapar vi en withLog högre ordningsfunktion som tar en funktion och returnerar en funktion som loggar ett meddelande innan den omslutade funktionen körs.

```
const add = (a, b) => a + b;
const addWithLogging = withLog(add);
addWithLogging(3, 4);
// ringer add
// 7
```

withLog HOF kan användas med andra funktioner också och det fungerar utan några konflikter eller att skriva extra kod. Det här är skönheten med en HOF.

```
const addWithLogging = withLog(add);
const hype = s => s + '!!!';
const hypeWithLogging = withLog(hype);
hypeWithLogging('Rea');
// ringhype
// Rea!!!
```

Man kan också kalla det utan att definiera en kombinerande funktion.

```
withLog(hype)('Rea');
// ringhype
// Rea!!!
```

### Curry

Currying innebär att bryta ner en funktion som tar flera argument till en eller flera nivåer av högre ordningsfunktioner.

Låt oss ta tilläggsfunktionen.

```
const add = (a, b) => a + b;
```

När vi ska curry det, skriver vi om det och fördelar argument i flera nivåer enligt följande.

```
const add = a => {
returnera b => {
returnera a + b;
};
};
add(3)(4);
// 7
```

Fördelen med att currya är memorisering. Vi kan nu memorera vissa argument i ett funktionsanrop så att de kan återanvändas senare utan duplicering och omräkning.

```
// antar att anropet getOffsetNumer() är dyrt
const addOffset = add(getOffsetNumber());
addOffset(4);
// 4 + getOffsetNumber()
addOffset(6);
```

Detta är verkligen bättre än att använda båda argumenten överallt.
```
// (X) GÖR INTE DETTA
add(4, getOffsetNumber());
add(6, getOffsetNumber());
add(10, getOffsetNumber());
```
Vi kan också formatera om vår curryfunktion så att den ser kortfattad ut. Detta beror på att varje nivå av currying-funktionsanropet är en enkelradsretursats. Därför kan vi använda pilfunktioner i ES6 för att omstrukturera den enligt följande.
```
const add = a => b => a + b;
```

### Sammansättning

I matematik definieras komposition som att överföra utdata från en funktion till input från en annan för att skapa en kombinerad utdata. Detsamma är möjligt i funktionell programmering eftersom vi använder rena funktioner.

För att visa ett exempel, låt oss skapa några funktioner.

Den första funktionen är range, som tar ett startnummer a och ett slutnummer b och skapar en array som består av tal från a till b.
```
const range = (a, b) => a > b ? [] : [a, ...område(a+1, b)];
```

Sedan har vi en funktion multiplicera som tar en array och multiplicerar alla siffror i den.

const multiplicera = arr => arr.reduce((p, a) => p * a);
Vi kommer att använda dessa funktioner tillsammans för att beräkna faktorial.
```
const factorial = n => multiplicera(intervall(1, n));
factorial(5);
// 120
factorial(6);
// 720
```

Ovanstående funktion för att beräkna faktorial liknar f(x) = g(h(x)), vilket visar kompositionsegenskapen.


## AJ 1.6 Avancerad funktionalitet i ES.next

När du läser om JavaScript kommer du oundvikligen att se en av dessa termer: ES3, ES5, ES6, ES7, ES8, ES2015, ES2016, ES2017, ECMAScript 2017, ECMAScript 2016, ECMAScript 2015... vad betyder de?

De hänvisar alla till en standard, kallad ECMAScript. ECMAScript är standarden som JavaScript bygger på, och den förkortas ofta till ES. Förutom JavaScript implementerar andra språk ECMAScript, inklusive:

- ActionScript (Flash-skriptspråket), som tappar i popularitet eftersom Flash officiellt kommer att upphöra 2020
- JScript (Microsofts skriptdialekt), eftersom JavaScript vid den tiden endast stöddes av Netscape och webbläsarkrigen var på topp, var Microsoft tvungen att bygga sin egen version för Internet Explorer.

men naturligtvis är JavaScript den mest populära och mest använda implementeringen av ES. Varför detta konstiga namn? Ecma International är en schweizisk standardiseringsorganisation som ansvarar för att definiera internationella standarder. När JavaScript skapades presenterades det av Netscape och Sun Microsystems för Ecma och de gav det namnet ECMA-262 alias ECMAScript.

Detta pressmeddelande från Netscape och Sun Microsystems (tillverkaren av Java) kan hjälpa till att ta reda på namnvalet, vilket kan inkludera juridiska frågor och varumärkesfrågor från Microsoft som var i kommittén, enligt Wikipedia. Efter IE9 slutade Microsoft att märka sitt ES-stöd i webbläsare som JScript och började kalla det JavaScript (åtminstone kunde jag inte hitta referenser till det längre).
Så från och med 201x är det enda populära språket som stöder ECMAScript-specifikationen JavaScript.

### Aktuell ECMAScript-version

Den nuvarande ECMAScript-versionen är ES2018.
Den släpptes i juni 2018.

Vad är TC39
TC39 är kommittén som utvecklar JavaScript.
Medlemmarna i TC39 är företag som är involverade i JavaScript och webbläsarleverantörer, inklusive Mozilla, Google, Facebook, Apple, Microsoft, Intel, PayPal, SalesForce och andra.
Varje standardversionsförslag måste gå igenom olika stadier, vilka förklaras här.

### ES-versioner

Jag tyckte att det var förbryllande varför ibland en ES-version refereras av upplaganummer och ibland efter år, och jag är förvirrad av att årtalet av en slump är -1 på numret, vilket ökar den allmänna förvirringen kring JS/ES
Före ES2015 kallades ECMAScript-specifikationer vanligtvis av deras utgåva. Så ES5 är det officiella namnet för ECMAScript-specifikationsuppdateringen som publicerades 2009.
Varför händer detta? Under processen som ledde till ES2015 ändrades namnet från ES6 till ES2015, men eftersom detta gjordes sent hänvisade folk fortfarande till det som ES6, och communityn har inte lämnat namngivningen bakom upplagan — världen kallar fortfarande ES-släpp av upplaga nummer.

Den här tabellen borde klargöra saker och ting lite:

| Upplagans  |  Officiella Namn |  Datum publicera |
|------------|------------------|------------------|
| ES9   | ES2018 |  Jun, 2018   |
| ES8   | ES2017 |  Jun, 2017 |
| ES7   | ES2016 |  Jun, 2016 |
| ES6   | ES2015 |  Jun, 2015 |
| ES5.1 | ES5.1  |  Jun, 2011 |
| ES5   | ES5    |  Dec, 2009 |
| ES4   | ES4    |  Abandoned |
| ES3   | ES3    |  Dec, 1999 |
| ES2   | ES2    |  Jun, 1998 |
| ES1   | ES1    |  Jun, 1997 |

### Let och konst

Fram till ES2015 var var den enda tillgängliga konstruktionen för att definiera variabler.

```
var a = 0
```

Om du glömmer att lägga till var kommer du att tilldela ett värde till en odeklarerad variabel, och resultaten kan variera.

I moderna miljöer, med strikt läge aktiverat, kommer du att få ett felmeddelande. I äldre miljöer (eller med strikt läge inaktiverat) kommer detta att initiera variabeln och tilldela den till det globala objektet.

Om du inte initierar variabeln när du deklarerar den kommer den att ha det odefinierade värdet tills du tilldelar den ett värde.

```
var a //typeof a === 'odefinierad'
```

Du kan deklarera om variabeln många gånger och åsidosätta den:

```
var a = 1
var a = 2
```
Du kan också deklarera flera variabler samtidigt i samma sats:
```
var a = 1, b = 2
```
Omfattningen är den del av koden där variabeln är synlig.

En variabel initierad med var utanför valfri funktion tilldelas det globala objektet, har ett globalt omfång och är synlig överallt. En variabel initierad med var inuti en funktion tilldelas den funktionen, den är lokal och är endast synlig inuti den, precis som en funktionsparameter.

Varje variabel som definieras i en funktion med samma namn som en global variabel har företräde framför den globala variabeln och skuggar den.

Det är viktigt att förstå att ett block (identifierat av ett par lockiga hängslen) inte definierar ett nytt omfång. Ett nytt scope skapas bara när en funktion skapas, eftersom var inte har block scope, utan funktionsomfång.

Inuti en funktion är vilken variabel som helst som definieras i den synlig i hela funktionskoden, även om variabeln deklareras i slutet av funktionen kan den fortfarande refereras till i början, eftersom JavaScript innan koden körs faktiskt flyttar alla variabler överst (något som kallas hissning). För att undvika förvirring, deklarera alltid variabler i början av en funktion.

### Använder let

let är en ny funktion som introducerades i ES2015 och det är i huvudsak en blockomfattad version av ```var```. Dess omfång är begränsat till blocket, satsen eller uttrycket där det definieras, och alla inneslutna inre block.

Moderna JavaScript-utvecklare kan välja att bara använda let och helt ignorera användningen av var.

Om låt verkar vara en obskyr term, läs bara låt färg = 'röd' eftersom låt färgen vara röd och allt är mycket mer meningsfullt

Att definiera let utanför någon funktion - i motsats till var - skapar inte en global variabel.

Med hjälp av konst
Variabler som deklarerats med ```var``` eller ```let``` kan ändras senare i programmet och tilldelas om. När en const väl har initierats kan dess värde aldrig ändras igen, och den kan inte omtilldelas till ett annat värde.

```
const a = 'test'
```

Vi kan inte tilldela en annan bokstavlig till a-konst. Vi kan dock mutera ```a``` om det är ett objekt som tillhandahåller metoder som muterar dess innehåll.

const ger inte oföränderlighet, ser bara till att referensen inte kan ändras.

```const``` har block scope, samma som let.

Moderna JavaScript-utvecklare kanske väljer att alltid använda const för variabler som inte behöver tilldelas om senare i programmet, eftersom vi alltid bör använda den enklaste konstruktionen som finns tillgänglig för att undvika att göra fel på vägen.

### Pilfunktioner

Pilfunktioner, sedan de introducerades, har för alltid förändrat hur JavaScript-kod ser ut (och fungerar).

Enligt min mening var denna förändring så välkommen att du nu sällan ser användningen av funktionsnyckelordet i moderna kodbaser. Även om det fortfarande har sin användning.

Visuellt är det en enkel och välkommen förändring, som låter dig skriva funktioner med en kortare syntax, från:
```
const myFunction = function() {
   //...
}
```
till
```
const myFunction = () => {
   //...
}
```
Om funktionskroppen bara innehåller en enda sats kan du utelämna parenteser och skriva allt på en enda rad:

```
const myFunction = () => doSomething()
```

Parametrar skickas inom parentes:
```
const myFunction = (param1, param2) => doSomething(param1, param2)
```

Om du har en (och bara en) parameter kan du utelämna parenteserna helt:
```
const myFunction = param => doSomething(param)
```

Tack vare denna korta syntax uppmuntrar pilfunktioner användningen av små funktioner.

Implicit retur
Pilfunktioner låter dig ha en implicit retur: värden returneras utan att du behöver använda nyckelordet return.

Det fungerar när det finns en enradssats i funktionskroppen:
```
const myFunction = () => 'test'
myFunction() //'test'
```

Ett annat exempel, när du returnerar ett objekt, kom ihåg att linda de krulliga parenteserna inom parentes för att undvika att det anses vara omslagsfunktionens kroppsparenteser:
```
const myFunction = () => ({ värde: 'test' })
myFunction() //{värde: 'test'}
```

Hur detta fungerar i pilfunktioner
detta är ett koncept som kan vara komplicerat att förstå, eftersom det varierar mycket beroende på sammanhanget och även varierar beroende på JavaScript-läget (strikt läge eller inte).

Det är viktigt att förtydliga detta koncept eftersom pilfunktioner beter sig väldigt annorlunda jämfört med vanliga funktioner.

När det definieras som en metod för ett objekt, i en vanlig funktion hänvisar detta till objektet, så du kan göra:
```
const bil = {
   modell: 'Fiesta',
   manufacturer: 'Ford',
   fullName: function() {
           return `${this.manufacturer} ${this.model}` 
   }
}
  
  
   ```  

<div class="blue">   

anropar car.fullName() kommer att returnera "Ford Fiesta".

Detta omfång med pilfunktioner ärvs från exekveringskontexten. En pilfunktion binder inte alls detta, så dess värde kommer att slås upp i anropsstacken, så i den här koden fungerar inte car.fullName() och returnerar strängen "undefined undefined":
```  
const bil = {
   modell: 'Fiesta',
   tillverkare: 'Ford',
   fullständigt namn: () => {
     returnera `${this.manufacturer} ${this.model}`
   }
}
```  

På grund av detta är pilfunktioner inte lämpade som objektmetoder.

Pilfunktioner kan inte heller användas som konstruktorer, när instansiering av ett objekt kommer att uppstå en TypeError.

Det är här vanliga funktioner ska användas istället, när dynamisk kontext inte behövs.

Detta är också ett problem vid hantering av händelser. DOM-händelseavlyssnare ställer in detta som målelementet, och om du litar på detta i en händelsehanterare är en vanlig funktion nödvändig:
```  
const link = document.querySelector('#link')
link.addEventListener('klick', () => {
   // detta === fönster
})
```  
```  
const link = document.querySelector('#link')
link.addEventListener('klick', function() {
   // denna === länk
})
```  



## AJ 1.7 JavaScript i integrerade system
Beskriv rubriken här

## AJ 1.8 Native bundeling av JavaScript för olika operativsystem och enheter
Beskriv rubriken här

</div>


Källor:
      
