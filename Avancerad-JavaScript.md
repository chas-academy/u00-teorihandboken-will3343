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

En utvecklare av integrationstjänster kan generera ett JavaScript-klient-API från en befintlig integrationstjänst. JavaScript-klientens API tillhandahåller operationsfunktioner som en JavaScript-utvecklare kan anropa från en applikation som körs i en JavaScript-miljö.

När utvecklaren av integrationstjänsten genererar JavaScript-klientens API för en integrationstjänst inträffar följande händelser:
JavaScript-klient-API-kod genereras från definitionen av det befintliga gränssnittet för integrationstjänsten. Du kan använda den här koden i JavaScript-applikationer för att anropa integrationstjänstens operationer utan att konfigurera den underliggande kommunikationsmekanismen. En JavaScript-metod skapas för varje integrationstjänstoperation.
En JSON/HTTP-bindning läggs till i integrationstjänsten så att JSON-meddelanden (JavaScript Object Notation) som skickas från JavaScript-klientens API kan bearbetas av integrationstjänsten. JSON/HTTP-bindningen är endast avsedd för användning av JavaScript-klientens API.
En webbsida som beskriver JavaScript-klientens API genereras. Från webbsidan kan JavaScript-utvecklaren ladda ner eller referera till JavaScript-klientens API-kod och kopiera exempelkod direkt till JavaScript-klientapplikationer. Webbsidan nås från integrationstjänstens URL.
Element som är definierade i den befintliga integrationstjänsten, såsom delade variabler och Java™-statik, gäller även för integrationstjänsten när integrationstjänsten anropas av JavaScript-klientens API.
Om integrationstjänsten uppdateras efter att JavaScript-klient-API:et har genererats, uppdateras JavaScript-klient-API-filen och den associerade webbsidan automatiskt när integrationstjänsten sparas.

### Restriktioner

Följande begränsningar gäller för JavaScript-klient-API:t som genereras från en integreringstjänstbeskrivning:
- Att anropa integrationstjänster med hjälp av JavaScript-klient-API stöds endast från klienter som initieras antingen av Node.js eller av en webbläsare i Google Chrome.
- JavaScript-klient-API-kod kan endast genereras från en befintlig integrationstjänst.
- Om du distribuerar ett webbläsarbaserat JavaScript-program måste HTTP-proxyservleten för IBM® Integration Bus distribueras på samma webbserver som din JavaScript-applikation. För information om HTTP-proxyservlet, se [HTTP-proxyservletöversikt.](https://www.ibm.com/docs/en/integration-bus/9.0.0?topic=availability-http-proxy-servlet)
- SOAP/HTTP-bindningen krävs inte för att integrationstjänsten ska kunna anropas av JavaScript-klientens API. Men om SOAP/HTTP-bindningen tas bort från en integrationstjänst är inte rot-URL:n för integrationstjänsten tillgänglig och därför är JavaScript-klientens API-kod och tillhörande webbsida inte tillgängliga.

### JavaScript i HTML-filen

I HTML-filen kan JavaScript-koden skrivas inuti skripttaggen som visas i koden nedan. Koden kommer att skriva meddelandet Hej JavaScript! på webbsidan. Kopiera denna kod till valfri textredigerare, spara filen som js.html. Öppna filen js.html i webbläsaren för att se meddelandet.

```  
    <!-- js.html -->

    <!DOCTYPE html>

         <html>

             <head>

                 <title>JavaScript</title>

             </head>

             <body>

                 <script type=''text/javascript''>

                 document.write(''Hello JavaScript!'');

                 </script>

             </body>

         </html>
```  

JavaScript har flera huvudverktyg som du kan använda för att arbeta med webbläsaregenskaper och händelser. Ett objekt är "fönster"-objektet. Detta objekt hanterar alla händelser och egenskaper som finns i användarens webbläsare. Ett nytt fönster öppnar en ny webbläsarinstans, så att du kan ha flera fönster öppna på användarens skrivbord. Kom ihåg att kod på klientsidan körs på användarens skrivbord, vilket innebär att användaren har viss kontroll över vilken typ av åtgärder du kan utföra. Du bör också ta hänsyn till användarens skrivbord när du arbetar med webbapplikationer. Popup-blockerare för webbläsare hindrar webbapplikationer från att öppna nya fönster, så du bör vara försiktig när du förlitar dig på fönsterobjektet i din JavaScript-kod.

De vanligaste fönstermetoderna är window.open(). Denna metod öppnar ett nytt webbläsarfönster på användarens skrivbord. Vanligtvis öppnar du ett nytt fönster när en användare klickar på en knapp på din webbsida. Till exempel kanske du vill öppna ett nytt fönster när användaren klickar på en knapp för att öppna ett kontaktformulär som sedan skickar feedback från användaren. Du kopplar din JavaScript-funktion till knappens onclick-händelse och öppnar ett nytt fönster för att ta emot feedback från användare. Låt oss använda det här scenariot för vårt nästa kodexempel. Ta en titt på följande kod.

```  
   <!DOCTYPE html>
         <html>

             <head>

                 <script> 

                     function OpenWindow(url) {

                         var myWindow = window.open(url, "New Window", "width=200, height=100");
                         myWindow.document.write("<p> This is a new window. </p>");
}
             </script>

     <body>

         <div id="mydiv">
             My First JavaScript code.
         </div>    

         <button type="button" onclick="OpenWindow('contact.html')">Contact me!</button>

     </body>
        </html>
 ``` 

Ovanstående kod liknar de tidigare exemplen vi använde. Vi har samma knapp och text som visas när användaren laddar sidan. Vi ändrade funktionen till "OpenWindow" med en url-parameter. URL-strängen som skickas är vad metoden window.open() använder när den öppnar ett nytt fönster. När fönstret har öppnats anropas metoden document.write() i det öppna fönstret. Observera att den nya objektvariabeln "myWindow" är specificerad. Vi kan använda huvudsidan för att redigera kod i det öppnade fönstret så länge vi tilldelar fönsterobjektet till en variabel behållare. Detta liknar tidigare lektioner där vi kallade metoder specifika för objektvariabelbehållaren. I det här fallet är fönsterbehållaren objektet, och vi använder objektinstansen för att redigera fönstrets egenskaper och anropsmetoder som är specifika för det specifika fönstret.

När knappen trycks in skickas URL:en "contact.html" till OpenWindow-funktionen. Denna URL används sedan i metoden window.open. Det sista strängvärdet i metoden window.open är valfritt. Dessa alternativ talar om för webbläsaren hur fönstret ska ändras. I det här fallet är fönstermåtten 200 i bredd och 100 för höjden. Den andra parametern window.open är namnet på fönstret, som också är valfritt. Du kan också anropa metoden window.open utan parametrar, vilket öppnar ett nytt webbläsarfönster som standard. Du kan använda flera alternativ som rullningslist, helskärm, bredd, höjd och tillåta användaren att ändra storlek på fönstret. Alla dessa alternativ är tillgängliga när du använder Windows-objektet.

Att komma igång med HTML och JavaScript tar lite tid när du lär dig språket. Arbeta med händelsehanterare och testa koden själv för att få en känsla av hur språket på klientsidan fungerar med användarens webbläsare.

### Dokument Object Model (DOM)

När du arbetar med JavaScript kommer du att höra termen "DOM" upprepas ofta. DOM är dokumentobjektmodellen. DOM representerar en HTML-sida och dess element. Rotelementet är HTML-taggen du använder i början och slutet av varje HTML-sida. Rotelementet innehåller sedan head- och body-taggarna, som är nästa del av modellen. Tänk på DOM som en HTML-struktur som har en huvudsaklig HTML-rotbehållare. Alla taggar i body-taggen är också en del av DOM. Du kan sedan använda DOM med JavaScript för att dynamiskt redigera tagginnehållet. Den här lektionen täcker grunderna i DOM och hur du kan använda den med JavaScript för att skapa dynamiska UI-element.

### DOM-element och struktur

DOM är inte olik alla andra klassobjekt. Du har ett huvud-DOM-objekt (dokument) och metoder och egenskaper inom objektet. Du kan använda DOM för att direkt komma åt element på en sida. Du kan komma åt ett eller flera element, som returneras i en array. I den föregående lektionen använde vi DOM:s getElementById-metod för att komma åt ett specifikt taggelement. Du kan också komma åt en grupp av element med hjälp av getElementsByTagName. Ta en titt på följande kod.

``` 
   <!DOCTYPE html>
         <html>

             <script>
                 var tags = document.getElementsByTagName("div");

                 tags[0].innerHTML = "My changed JavaScript code.";

             </script>

         <body>

             <div id="mydiv">My First JavaScript code.</div>

             <div id="mydiv2">My First JavaScript code.</div>

         </body>
         </html>
``` 

Observera att varje div-element har ett annat id-värde. Detta krävs som en del av standarden för HTML-sidor och kodningssyntax. Det finns två div-taggar i DOM. JavaScript-koden hämtar alla div-taggar och tilldelar arrayen till variabeln "taggar". Det andra JavaScript-uttrycket tilldelar det första elementet i arrayen texten "Min ändrade JavaScript-kod." Det betyder att "mydiv"-taggens inre HTML-taggtext ändras till denna fras när sidan läses in.

Varje element i body-taggen är tillgängligt i DOM, och JavaScript erbjuder flera egenskaper och metoder som du kan använda för att gå igenom sidans text, värden och egenskaper. Ovanstående exempel använder DOM för att ändra den första div-taggens text, men du kan också använda samma typ av kod för att få värdet på taggens text. Du måste ofta få taggens värde när du arbetar med användarinmatning, särskilt när du arbetar med formulär. Följande kod visar hur du tilldelar en variabel med värdet av den första div-taggens inre HTML.

``` 
   <!DOCTYPE html>
         <html>

             <script>
                 var tags = document.getElementsByTagName("div");

                 tags[0].innerHTML = "My changed JavaScript code.";

                 var firstDiv = tags[0].innerHTML

                 tags[1].innerHTML = firstDiv;
              
              </script>

             <body>

                 <div id="mydiv">My First JavaScript code.</div>

                 <div id="mydiv2">My First JavaScript code.</div>

             </body>
         </html>
``` 

Ovanstående HTML och JavaScript bygger på föregående avsnitts kod. De två första JavaScript-uttrycken utför samma utdata som föregående avsnitt. De följande två raderna med kod är olika. Nästa kodrad hämtar den inre HTML-koden från det första taggelementet och tilldelar sedan den inre HTML-texten till den andra taggen i arrayen. Ovanstående kod skriver ut "Min ändrade JavaScript-kod" till båda div-taggarna i DOM.

### Ändra elementegenskaper

Hittills har vi bara ändrat och läst en div-taggs innerHTML-egenskaper, men det finns flera egenskaper att arbeta med när du använder DOM. Alla egenskaper som är giltiga i HTML är också giltiga när du arbetar med JavaScript. Anta att du dynamiskt vill ändra bakgrunden för ett element när användaren klickar på en knapp. Du kan göra detta med DOM och JavaScript. Vi bygger vidare på de tidigare HTML-sidorna och ändrar JavaScript-koden för att ändra bakgrundsfärgen för den första div. Ta en titt på följande kod.

```
   <!DOCTYPE html>
         <html>

             <head>

                 <script> 

                     function ChangeBackgroundColor() {

                     var tags = document.getElementsByTagName("div");

                     tags[0].backgroundColor = "red";
}
                 </script>

             </head>

             <body>

                 <div id="mydiv">My First JavaScript code.</div>

                 <button type="button" onclick="ChangeBackgroundColor()">Change It</button>

             </body>
         </html>

```

Du kommer att känna igen koden ovan från föregående kapitel. Händelsehanteraren "onclick" tilldelas JavaScript-funktionen ChangeBackgroundColor. I den här exempelfunktionen ändras bakgrundsfärgen för den första div till röd. BackgroundColor-attributet är en del av DOM för div-taggar. Du kan också få den aktuella bakgrundsfärgen med liknande syntax. Följande kod tilldelar variabeln "bgcolor" den aktuella bakgrundsfärgen för div-elementet.

```
   <!DOCTYPE html>
         <html>

             <head>

                 <script> 

                      function GetBackgroundColor() {

                      var tags = document.getElementsByTagName("div");

                      var bgcolor = tags[0].backgroundColor;
}
                 </script>

             </head>

             <body>

                 <div id="mydiv">My First JavaScript code.</div>

                 <button type="button" onclick="GetBackgroundColor()">Get It</button>

             </body>
         </html>
```

Istället för att ändra bakgrundsfärgen får exemplet ovan den aktuella färgen från DOM. Observera att händelsehanterarens funktionsnamn ändrades för att matcha ett mer lämpligt namn för funktionen, vilket är GetBackgroundColor. Denna funktion aktiveras när användaren klickar på knappen.

### Arbeta med cookies

Har du någonsin sett formulär där webbsidan automatiskt känner till ditt användarnamn eller någon egendom som du har angett i webbplatsens lagrade data? Värden som lagras som kvarstår genom att lämna webbplatsen eller stänga webbläsaren använder cookies. Cookies är små filer som lagras i webbläsarens cookiekatalog. Dessa filer är i allmänhet ofarliga och hjälper en webbplats att identifiera dig och grundläggande information när du öppnar webbplatsen. En sak att notera är att du aldrig lagrar känslig information i en cookie. Till exempel skulle du inte lagra en användares lösenord i en cookie. Cookiefiler lagras i vanlig text, så alla som har tillgång till användarens cookies skulle kunna läsa denna känsliga information. Lagra inte lösenord, kreditkortsinformation eller personnummer i cookies.

Cookie-egenskapen lagras i dokumentobjektet. Du måste ge kakan ett namn och ett värde. Namnet används för att anropa cookien när användaren kommer tillbaka, och värdet är det du vill visa eller bearbeta när användaren kommer tillbaka.

Ta en titt på följande JavaScript-kod (HTML-koden är utesluten i det här exemplet).
```
document.cookie = "username=will";
```

Ovanstående kod tilldelar webbläsaren en ny cookie. Cookienamnet är "användarnamn" och värdet som tilldelas är "jdoe." När användaren återvänder till sidan kan du använda denna cookie för att automatiskt visa användarens namn.

När du skapar en cookie bör du också ge den ett utgångsdatum. Utgångsdatumet talar om för webbläsaren när den kan radera cookien. Till exempel kanske du vill tvinga en användare att ange sitt användarnamn och lösenord inom 30 dagar av säkerhetsskäl. Du kan sedan ställa in utgångsdatumet för en cookie till 30 dagar från det aktuella datumet. Följande kod visar dig hur du ställer in ett utgångsdatum för din nya användarnamnscookie.

```
var nu = new Date();

now.setDate(now.getDate() + 31);

document.cookie = "användarnamn=jdoe; expires=" + now.toString();
```

Du kommer att känna igen Date-objektet från ett tidigare kapitel. Den här koden får det aktuella datumet, lägger till 31 dagar till datumet och sedan tilldelar den detta värde till cookiens "expires"-egenskap. Nu, när användaren stänger sin webbläsare efter 31 dagar, kommer webbläsaren automatiskt att ta bort cookien. Kom ihåg att Date-objektet får datumet på användarens dator eftersom JavaScript är klientkod. Om datumet på användarens dator är fel kommer din kod att lägga till 31 dagar till användarens klockinställningar och inte din lokala servers tid. Arbetet med lokaliserad tid görs på serversidans kod som du kan skicka till webbläsaren. Du kan för övrigt tvinga en cookie att raderas direkt efter att användaren stänger webbläsaren. Om du ställer in cookiens utgångsdatum till ett passerat datum förfaller kakan automatiskt och webbläsaren tar bort den så snart användaren är klar med din webbapplikation.

Du har ställt in din cookie, men hur får du kakan och dess värde? Vad händer om du har flera cookies? Varje cookie separeras med semikolon. Du kan använda en "för"-slinga för att gå igenom varje kakobjekt och hitta den du vill använda. Följande kod ger dig ett exempel.

```
    var cookies = document.cookie.split(';');

    for(var i=0; i< cookies.length; i++) {

        var c = cookies [i];

        if (c.indexOf("username") != -1)

        document.getElementById("cookiediv").innerHTML = c. substring(("username").length,c.length);

    }
```

Ovanstående kod är lite komplex. Det finns inget sätt att läsa en cookie vid namn som de flesta språk. Ovanstående kod delar upp cookie-arrayen med semikolon och går igenom varje värde tills den hittar cookienamnet "användarnamn". Sedan identifierar den cookiens värde genom att hämta delsträngen från arraysträngen. Du kan behöva justera den här koden så att den matchar dina egna krav, men det viktiga är att du måste gå igenom JavaScript-cookies för att hitta den du vill läsa.

DOM är en del av all JavaScript-kodning. Du måste bli mycket bekant med objektmodellen för att komma åt data, ändra data och dynamiskt arbeta med användarinput för att skapa fantastiska användargränssnitt.


## AJ 1.8 Native bundeling av JavaScript för olika operativsystem och enheter

En bundler är ett utvecklingsverktyg som kombinerar många JavaScript-kodfiler till en enda som är produktionsklar och kan laddas i webbläsaren. En fantastisk egenskap hos en bundler är att den genererar en beroendegraf när den går igenom dina första kodfiler. Detta innebär att från och med den ingångspunkt du angav, håller modulbuntaren reda på både dina källfilers beroenden och tredjepartsberoenden. Denna beroendegraf garanterar att alla källfiler och tillhörande kodfiler hålls uppdaterade och felfria.

Du kan bara föreställa dig hur komplicerat proceduren var innan buntarna. Att hålla alla filer och deras beroenden uppdaterade och redo var en stor uppgift för webbutvecklare.

Överväg en grundläggande JavaScript CRUD-app (Skapa, Läs, Uppdatera och Ta bort) som en inköpslista. I pre-bundler-eran kan du ha konstruerat dessa funktioner i separata JS-filer. Du kan till och med välja att göra din app lite mer snygg genom att inkludera tredjepartsbibliotek, och detta skulle behöva din fil för att göra flera frågor vid inläsning, som i det här exemplet.

```
<head>
       <script src="https://unpkg.com/@popperjs/core@2/dist/umd/popper.min.js"></script>
       <script type='text/javascript' src='tinycolor.js'></script>
       <script type='text/javascript' src='/nav.js'></script>
       <script type='text/javascript' src='/crud.js'></script>
       <script type='text/javascript' src='/main.js'></script>
</head>
```

Men om du använder en buntare kommer filerna och deras beroenden att slås samman till en enda fil.

```
<head>
       <script type='text/javascript' src='/bundle.js'></script>
</head>
```

Anta att du utvecklar eller underhåller en stor app som en e-handelssida som ger åtkomst till tusentals produkter till flera användare. För ett användningsfall som detta kommer du sannolikt att behöva använda anpassade bibliotek eller tredjepartsbibliotek för att driva några av dina mer komplexa uppgifter. I så fall skulle utveckling utan en JavaScript-modulbuntare göra att hålla alla beroenden uppdaterade till den senaste versionen till en uttömmande process.

Förutom att tillhandahålla en konsekvent verktygsmiljö som räddar dig från smärtan av beroenden, kommer många populära modulbuntare också med prestandaoptimeringsfunktioner. [Koddelning](https://developer.mozilla.org/en-US/docs/Glossary/Code_splitting) och [byte av heta moduler](https://webpack.js.org/concepts/hot-module-replacement/) är exempel på dessa funktioner. JavaScript-buntare har också produktivitetshöjande funktioner som robust felloggning, vilket gör att utvecklare enkelt kan felsöka och reparera fel.

### Hur fungerar en bundler?

Efter att ha diskuterat vad bundlers är och hur avgörande de är i dagens webbutvecklingsekosystem, låt oss titta på hur dessa beroendehanteringsverktyg fungerar. Sammantaget är en buntares verksamhet uppdelad i två steg: generering av beroendediagram och eventuell buntning.

#### Kartläggning av ett beroendediagram

Det första en modulbuntare gör är att skapa en relationskarta över alla serverade filer. Denna process kallas Dependency Resolution. För att göra detta kräver buntaren en inmatningsfil som helst bör vara din huvudfil. Den analyserar sedan denna postfil för att förstå dess beroenden.

Efter det går den igenom beroenden för att bestämma beroenden för dessa beroenden. Knepigt, va? Den tilldelar unika ID:n till varje fil som den ser under hela processen. Slutligen extraherar den alla beroenden och genererar en beroendegraf som visar förhållandet mellan alla filer.

Varför är denna process nödvändig?

- Det gör det möjligt för modulen att konstruera en beroendeordning, avgörande för att hämta funktioner när en webbläsare begär dem.
```
   return {  id,  filename,  dependencies,  code,  };
```

- Det förhindrar namnkonflikter eftersom JS-bundlaren har en bra källkarta över alla filer och deras beroenden.

- Den upptäcker oanvända filer så att vi kan bli av med onödiga filer.

#### Bundling

Efter att ha tagit emot indata och gått igenom dess beroenden under beroendeupplösningsfasen, levererar en bunter statiska tillgångar som webbläsaren framgångsrikt kan bearbeta. Detta slutsteg kallas för packning. Under denna process kommer buntaren att utnyttja beroendediagrammet för att integrera våra flera kodfiler, injicera den nödvändiga funktionen och module.exports-objektet och returnera ett enda körbart paket som webbläsaren kan ladda.

### JavaScript-modulbuntare

Vikten av JavaScript-modulbuntare och hur de fungerar, kanske du undrar vilken typ av paketerare som är bäst för dig. Det finns många olika modulbuntare i JavaScript-ekosystemet och var och en med sin unika buntningsmetod. Vi kommer att titta på fem av de mest populära modulbuntarna i Javascript-ekosystemet, och utforska hur de fungerar samt deras fördelar och nackdelar.

### Webpack

Som alla moderna JavaScript-buntlare börjar Webpack buntningsprocessen genom att sammanställa en beroendegraf. För att förstå hur det utför steget för beroendeupplösning måste du först förstå sex nyckelbegrepp:

- Entry: anger var Webpack ska initiera sitt beroendediagram. Du kan ha en eller flera ingångspunkter beroende på din app arkitektur. Webpack itererar genom modulen/modulerna som anges i konfigurationsfilen webpack.config.js och identifierar ingångspunktens direkta och indirekta beroenden.
```
module.exports = { entry: './app/index.js', };
```
- Utdata: anger önskad destination för den slutliga utmatningen efter att Webpack har slutfört packningsprocessen. Egenskapen Output innehåller två undervärden: filsökvägen, vanligtvis mappen /dist, och det önskade filnamnet.

```
    const path = require('path');  module.exports = {  entry: './app/index.js',  output: {  path: path.resolve(__dirname, 'dist'),  filename: 'webpack-app.bundle.js',  },  };
```

- Laddare: tillåter Webpack att transformera och bunta icke-JS-filer.

- Plugins: tillåt Webpack att utföra mer avancerade åtgärder som anpassad resursoptimering och hantering.

- Läge: låter Webpack konfigurera sin verksamhet till produktions- eller utvecklingslägen dynamiskt.

- Webbläsarkompatibilitet: låt Webpack bygga paket som stöder moderna och gamla webbläsare med funktioner som löften och polyfills.

Efter att ha skapat den interna modulkartan, använder Webpack sedan funktioner för att slå in de associerade modulerna som buntar ihop för att anropas av en enda körtidsfunktion som kallas webpackStart.

Att komma igång är lika enkelt som att köra npm i webpack

### Fördelar

#### Stöd för flera resurser

Förutom att tillhandahålla direkt support för JS-filer, har Webpack ett rikt plugin-ekosystem som det är beroende av för att bunta andra filer som CSS och bilder.

#### Tillgångsoptimering

Funktioner som koddelning gör att du kan dela upp kodfiler i bitar och därigenom minska laddningstiden. Det finns Hot-modulersättningen som hjälper dig att hantera moduler utan att ladda om webbläsaren helt. Utvecklare kan använda Loaders för att förbehandla sina filer, vilket resulterar i en snabbare appkörning. Dessa och fler mycket anpassningsbara optimeringsfunktioner har gjort Webpack till den mest populära JS-buntaren.

#### Utvecklares produktivitet

När du arbetar med en komplicerad uppgift som modulpaketering som utvecklare är det avgörande att ha:

- Omfattande dokumentation.

- Ett solidt ekosystem av tredjepartsverktyg som du kan luta dig mot.

- Effektiv felsökningsprocess som gör ditt arbete enklare.

Webpack uppfyller dessa tre krav genom att erbjuda ett enormt ekosystem av plugins och laddare, samt källkartadriven felsökning. Det är inte allt. Webpack har ett internt cachningssystem som ger utvecklare möjlighet att bygga appar på kort tid.

### Nackdelar

#### Komplex

Webpacks sofistikerade är ett tveeggat svärd för många utvecklare som har ett hat-kärleksförhållande till det. Det är också komplext och har en brant inlärningskurva.

#### Buggy och Slow

Webpacks tillvägagångssätt med alla batterier som ingår kan ibland göra att Webpack-appintegrationer blir överkonstruerade. Övertilltro till plugins för att göra enkla funktioner kan göra att buntaren långsammare W, vilket kräver teknisk felsökning för att göra den väl optimerad.

### Browserify 

[Browserify](https://browserify.org/) är ett Javascript-paket med öppen källkod som låter dig bunta ihop Node.js-filer som webbläsaren kan köra. Med Browserify kan utvecklare använda nod-style require() för att ladda npm-moduler i webbläsaren. JS-buntaren släpptes ursprungligen 2010 och har haft hyfsad framgång bland utvecklare. Den laddas ner nästan 2 miljoner gånger varje vecka och har över 13 000 GitHub-stjärnor.

#### Hur fungerar det?

Precis som alla andra JavaScript-buntlare går Browserify igenom definierade stadier vid buntning av moduler. Den första är bildandet av beroendediagrammet. I detta skede startar Browserify från de angivna ingångspunktsfilerna och söker sedan rekursivt efter alla require()-anrop i dina filer. Varje require()-anrop löses med en filsökväg, och varje filsökväg korsas ytterligare för fler require()-anrop.

Efter att hela appens beroendediagram har kartlagts helt, skapar den ett fristående paket som består av filer som har slagits samman och mappats till unika ID:n. Det är värt att notera att Browserfy också erbjuder avancerade anpassningar, såsom möjligheten att ersätta dessa ID:n med hashade.

Du kan sedan placera den sista bunten i ett enda ```<script>``` för eventuell webbläsning. Att komma igång med Browserify är lika enkelt som att köra npm i webpack och köra Browserify mot din inmatningsfil.

```
    $ browserify main.js > bundle.js
```

Bundleren tillhandahåller också några inbyggda alternativ som --debug och --ignore-missing.

### Fördelar

#### Enkelhet

För de flesta applikationer med färre funktioner tycker många utvecklare att Browserify är perfekt för deras behov. Det ger enkla npm-integreringar som låter dig återanvända din nodkod utan att behöva en inbyggd CLI.

#### Utvecklares produktivitet

Browserifys viktigaste försäljningsargument är att det låter dig dra fördel av det rika npm-ekosystemet. Det är lätt att lära sig och har utmärkt dokumentation. Dessutom kommer den med ett inbyggt automatiskt byggsystem som gör byggmoduler snabba och enkla. Allt detta ger en fantastisk upplevelse när du utvecklar din applikation.

### Nackdelar

#### Inget stöd för flera resurser

Till skillnad från Webpack ger Browserify inte stöd för flera tillgångar. Du kan dock använda ett Gulp-arbetsflöde för att hitta runt detta. Processen introducerar ändå onödig komplexitet.

#### Brist på avancerade hanteringsfunktioner

Browserify begränsar dig till Node.js npm-ekosystemet och saknar kraftfulla verktyg för tillgångshantering som kan hjälpa dig att optimera dina moduler. Detta inkluderar bristande stöd för dynamisk laddning.

### Parcel 

[Parcel](https://parceljs.org/) är ett plug-and-play-byggverktyg med noll konfiguration som gör det möjligt för utvecklare att snabbt konfigurera multi-tillgångar (t.ex. JS, CSS och HTML) moduler som är nödvändiga för utveckling. Den har över 39 000 stjärnor på Github, vilket gör den till den näst mest populära JS-buntaren bakom Webpack.

Hur fungerar det?
Pakets paketeringsprocess innefattar tre steg:

- Konstruktion av tillgångsträd: I detta skede tar Parcel en ingångspunktstillgång och går igenom filen för att identifiera de beroenden som används för att skapa ett träd med tillgångar som liknar beroendegrafen.

- Bundle Tree-konstruktion: Här kombineras individuella tillgångar i Asset Tree med deras länkade beroenden för att bilda ett buntträd.

- Paketering: Detta är det sista steget där varje bunt i buntträdet associeras med sina specifika paketeringsfiltyper och omvandlas till en slutlig kompilerad fil.

Efter det kan du sedan tillhandahålla en engångstillgång mot Parcel. Se till att notera att Parcel stöder flera ingångspunkter.

För att komma igång, kör npm i parcel.

Låt oss säga att du har ett exempel på HTML-kod.

```
   <html>
         <body>
                 <script src="./index.js"></script>
         </body>
  </html>
```

Du kan sedan använda Parcel för att bygga HTML-filen genom att köra: parcel index.html. Det som är imponerande är att Parcel kommer att kompilera HTML-filen som pekade på den och index.js som HTML-koden länkar till.

### Fördelar

#### Noll konfiguration 
Parcel löser konfigurationsproblemen med Webpack och Browserify som ger utvecklare en presterande arkitektur som behövs för snabb webbutveckling. Det finns också stöd för flera tillgångar som Webpack som möjliggör paket för alla typer av icke-JavaScript-tillgångar som CSS, HTML och bilder.

#### Snabbhet
Parcel tillhandahåller snabbt förstklassiga resursoptimeringsfunktioner som utbyte av heta moduler och lat inläsning av delad kod. Enligt de senaste riktmärkena är Parcels paketeringshastighet 9,98s, jämfört med Browserifys 22,98s och Webpacks 20,71s. Att använda Parcels inbyggda cachningsteknik kan till och med leverera snabbare resultat, med en benchmarktid på 2,64s.

### Nackdelar

#### Brist på avancerade anpassningar

Som en mycket ansedd buntare är Parcel perfekt för små och medelstora applikationer. Icke desto mindre kan det vara tråkigt att få det att fungera för komplexa applikationer där du behöver ändra konfigurationerna. I den här situationen föredrar de flesta utvecklare att använda Webpack.

### Fusebox

Fusebox är en öppen källkod för Javascript och Typescript buntare och laddare. Den kombinerar Webpacks bästa optimeringstekniker till en snabb, lätt buntare som ger en rik API-upplevelse.

#### Hur fungerar det?

Fusebox-buntningsprocessen tillhandahåller ett par standardinställningar som gör det enkelt att komma igång utan att kräva omfattande modifieringar.

För att komma igång, installera Fusebox med kommandot: npm i fuse-box. Efter det måste du skapa huvudkonfigurationsskriptfilen, vanligtvis med titeln fuse.js eller fuse.ts. Här är ett exempel på ett kodavsnitt som inkluderar ingångspunkten och destinationsfilen, såväl som det önskade läget.

```
   import { fusebox } from 'fuse-box';  fusebox({  target: 'browser',  entry: 'src/index.tsx',  webIndex: {  template: 'src/index.html',  },  devServer: true,  }).runDev();
```

Fusebox initierar buntningsprocessen genom att bygga en virtuell filstruktur som efterliknar en beroendegraf. Dessa filer sänds sedan ut och buntas ihop.

### Fördelar

#### Utmärkt utvecklarupplevelse

Fusebox har en minimal standardstil som resulterar i en enkel inlärningskurva för nybörjare. Detta möjliggör en snabb start utan mycket konfiguration.

### Snabbhet

Det ger en snabb upplevelse tack vare ett par tillgångsoptimeringsfunktioner den har. Funktioner som HMR (Hot Module Replacement) gör att buntaren kan hantera tillgångar utan att helt uppdatera webbläsaren. Det finns ett kraftfullt cachesystem och inbyggt kodspill, vilket resulterar i snabbare webbläsarladdningar.

### Nackdelar

#### Dåligt stöd för flera tillgångar

Fusebox är Javascript och Typescript-centrerad, vilket ger inbyggt stöd för båda filerna. Att arbeta med andra filer som CSS skulle kräva integration av CSSPlugin eller SassPlugin. Eftersom det är en nyare paketerare saknar den det robusta ekosystemet som ses i Webpack.


### Rollup

[Rollup,](https://rollupjs.org/) som släpptes 2018, är en nästa generations JavaScript-paketerare vars primära försäljningsargument är dess trädskakningsfunktion, vilket gör det möjligt för den att sålla bort oanvända resurser innan enstaka, mindre moduler paketeras till större. På grund av denna förmåga har den fått en viss dragning bland utvecklare och har laddats ner över 4 miljoner gånger varje vecka, och den har också mer än 20 000 GitHub-stjärnor.

### Hur fungerar det?

Samlad konfiguration använder huvudkonfigurationsfilen, vanligtvis kallad rollup.config.js, för att definiera buntningsspecifikationer. Därefter analyserar den ingångspunktsfilen och sorterar sedan beroenden samtidigt som den skapar en beroendeordning. Under denna analysprocess implementeras också trädskakningsfunktionen. Slutligen kompileras alla deklarerade funktioner som påträffas i de specificerade modulerna till ett enda globalt omfång samtidigt som man uppmärksammar potentiell namnkollision.

För att komma igång, kör npm i rollup för att installera rollup. Du kan utföra buntningsprocessen antingen genom en CLI med hjälp av en konfigurationsfil eller via buntande JavaScript API.

Här är ett exempel på en konfigurationsfil som innehåller ingångspunkten, utdatafilens destination och formattyp.

```
    export default {  input: 'src/app.js',  output: {  file: 'bundle.js',  format: 'cjs'  }  };
```

Liksom många andra JavaScript-buntlare stöder Rollup också flera ingångspunkter.

### Fördelar

#### Tillgångsoptimering

Sammanfattning ger dig tillgång till funktioner som gör att du kan koddela dina paket för snabbare inläsning av webbläsaren. Det finns också funktionen Tree-shaking som hjälper utvecklare att bli av med onödiga variabler eller funktioner.

### Native ES6-stöd

För bättre webbläsarkompatibilitet vid delning av import och export släpptes Javascripts ES6-version. Rollups stöder detta nya ES6-modulsystem som behåller befintliga import- och exportfunktioner samtidigt som du kan omvandla dem till andra modulformat som CommonJS och AMD.

### Nackdelar

#### Spirande utvecklarekosystem

En av de växande smärtorna med ett nytt utvecklingsverktyg är den tid det tar att bygga ett fullfjädrat ekosystem. Även om Rollup är idealiskt för snabba uppgifter, kan utvecklare bli besvikna när de skapar stora, komplexa appar på grund av brist på plugins för nödvändiga funktioner.

### Vite.js

[Vite.js](https://vitejs.dev/) är ett nästa generations frontendbyggande verktyg med öppen källkod. Vite.js är ett nästa generations frontendbyggande verktyg med öppen källkod. Vue.js-skaparen Evan Du skapade Vite.js 2020 för att förbättra paketeringsekosystemet genom att utnyttja de senaste ES-modulernas förbättringar för att lösa några av byggnadsprestandaproblemen som tidigare buntleverantörer stött på.

![Bild-5-Node](/images/js/vite.png)

För närvarande har Vite.js över 33,9 000 stjärnor på Github och har över 340 000 nedladdningar varje vecka.

  Hur fungerar det?
En av Vite.js unika funktioner är att den kommer med en dev-server och ett buntningskommando. Dev-servern analyserar dina applikationsmoduler och delar upp dem i två grupper: De beroenden som oftast inte uppdateras ofta är förbuntade med esbuild, en JavaScript-bundler som är extremt snabbare än Webpack, Rollup och Parcel. Applikationskällkodens andra grupp kräver frekventa uppdateringar och serveras på begäran utan att buntas till webbläsaren med hjälp av webbläsarens kraftfulla ESM-modulkapacitet.

Å andra sidan paketerar build-kommandot din kod med hjälp av Rollup, en JS-bundler som vi har undersökt tidigare. Vite.js startar från en ingångspunkt när du korsar din kodbas för att konvertera dem till produktionsklara statiska tillgångar. Liksom flera andra JS-bundlare stöder Vite.js också flera ingångspunkter.

```
   // vite.config.js
    const { resolve } = require('path')
    const { defineConfig } = require('vite')
 
    module.exports = defineConfig({
    build: {
         rollupOptions: {
             input: {
             main: resolve(__dirname, 'index.html'),
             nested: resolve(__dirname, 'nested/index.html')
     }
   }
 }
})
```

### Fördelar

#### Slank och snabb

Genom att utnyttja det inbyggda ES6-modulsystemet kan Vite.js servera applikationskod snabbare genom att minska antalet webbläsarförfrågningar den gör. Det är inte allt. Vite.js kommer också med Hot Module Replacement (HMR), vilket gör redigeringen snabbare och nästan omedelbar.

### Stöd för flera ramar

Vite.js är ramagnostisk med out-of-box-stöd för många populära Javascript-ramverk som React.js, Vue.js, Typescript och Preact. De senaste versionerna har också integrerat stöd för CSS-moduler, förprocessorer och andra statiska tillgångar. Till exempel kan du snabbt konfigurera en Vue.js-app med Vite med följande kommando:

npm init vite@senaste my-vue-app -- --mall vue

Den har också ett rikt plugin-ekosystem som utnyttjar andra buntare som esbuild och Rollup plugin-ekosystem för att ge utvecklare en omfattande uppsättning alternativ.

### Nackdelar

#### Beroende på ESM-moduler

Vite.js förlitar sig starkt på webbläsarens inhemska ESM-system för att producera den otroliga hastigheten den är känd för. Detta innebär att utvecklare kan stöta på problem när de hanterar äldre webbläsare som inte stöder dessa uppgraderingar.





</div>


Källor:

- Lektionsmaterial
- Eloquent Javascript  av Marijin Haverbeke  4th edition
- [Vite](https://vitejs.dev/)
- [Rollup](https://rollupjs.org/)
- [Fusebox](https://fuse-box.org/)
- [Parcel](https://parceljs.org/)
- [Browserify](https://browserify.org/)
- [TypeScript](https://www.typescriptlang.org/)
- [Express.js]( https://expressjs.com/)



      
