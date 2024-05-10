# Teorihandboken - Avancerad JavaScript (AJ)

Inlämningsdatum: 2024

Studerande: 

### William Berhane 

### FWD-23 - Chas Academy

<br>

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

    app.listen(port, () => console.log (`Example app listening at http://localhost:${port}`));

```


## AJ 1.3 Progressive Web Apps



## AJ 1.4 Typningssystem för Javascript (ex TypeScript, Flow)
Beskriv rubriken här

## AJ 1.5 Funktionell programmering i JavaScript
Beskriv rubriken här

## AJ 1.6 Avancerad funktionalitet i ES.next
Beskriv rubriken här

## AJ 1.7 JavaScript i integrerade system
Beskriv rubriken här

## AJ 1.8 Native bundeling av JavaScript för olika operativsystem och enheter
Beskriv rubriken här



Källor:
      
