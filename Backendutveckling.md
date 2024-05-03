# Teorihandboken - Backendutveckling (BE)

Inlämningsdatum: 2024

Studerande: 

### William Berhane 

### FWD-23 - Chas Academy

<br>

## Begrepp ord:

### cURL 
         
         står för Client URL används att utbyta data mellan en enhet och en server via ett kommandoradsgränssnitt(CLI).  

### Databas

        är en organiserad samling av strukturerad information, eller data, vanligtvis lagrad elektroniskt i ett datorsystem.

### ER-modellering

        står för Entity-Relationship model(ER-modellering), beskrivs inbördes relaterade saker av intresse inom en specifik kunskapsdomän. 

### Heirarkiska 

        är ett system som organiserar eller rangordnar saker, ofta efter makt eller betydelse.

### HTTP

        står för Hyper Transfer Protocol(HTTP), är protokollet som möjliggör kommunikation online och överför data från en maskin till en annan. 

### MVC

      står för Model-View-Controller (MVC), är ett mönster inom mjukvarudesign som vanligtvis används för att implementera användargränssnitt, data och styrlogik.

### OOP
       
       står för Object-Oriented Programming (OOP), klasser och objekt är grundläggande begrepp som låter dig modellera och organisera din kod på ett mer modulärt och återanvändbart sätt.

### PHP

       står för Hypertext Preprocessor (PHP), är ett populärt programmeringsspråk för webbutveckling. 

### Protokollet

       är en uppsättning regler för formatering och bearbetning av data.

### REST 

       står för REpresentational State Transfer(REST), är en arkitektonisk stil för att tillhandahålla standarder mellan datorsystem på webben, vilket gör det lättare för system att kommunicera med varandra.

### SQL

       står för Structured Query Language (SQL),  är ett programmeringsspråk för att lagra och bearbeta information i en relationsdatabas.

### Webbserver 

       är en server som lagrar information som är tillgänglig genom webben och levererar den som webbsidor till besökare.  

### Wordpress

       är ett av det mest populära hemsideverktyget att skapa webbplatser med.

### XML 

       står för Extensible Markup Language (XML), är ett märkningsspråk som tillhandahåller regler för att definiera all data.


## BE 1.1 PHP

PHP är ett skriptspråk på serversidan med öppen källkod som många utvecklare använder för webbutveckling. Det är också ett allmänt språk som du kan använda för att göra många projekt, inklusive grafiska användargränssnitt (GUI).

![Bild-1-PHP](/images/BE/php.jpeg)

### PHP Syntax 

För att komma igång med PHP är det viktigt att förstå PHP-syntaxens grunder. PHP-variabler visas med ett dollartecken följt av variabelnamnet, och de kan lagra olika datatyper, som t.ex

```php
<?php
echo "<p> Detta är PHP syntax. </p>"; 
?>

```

- Strängar/strings
- Heltal/Integers
- Flytare/Floats
- Booleans/Booleaner
- Arrayer/Arrays

Kontrollstrukturer som "if-satser" och "loopar" tillåter utvecklare att implementera villkorlig logik och repetitiva uppgifter. PHP stöder även funktioner och objekt, vilket möjliggör skapandet av återanvändbar kod och modulär programmering.

PHP introducerades av Rasmus Lerdorf 1994 i den första versionen och deltog i de senare versionerna. Det är ett tolkat språk och det kräver ingen kompilator. PHP stod ursprungligen för "Personlig hemsida." Under åren har det utvecklats till "PHP:
PHP är öppen källkod och har en stor gemenskap av utvecklare som bidrar till dess utveckling.



### Fördelaren med PHP

PHP har några fördelar som har gjort det så populärt, och det har varit det vanliga språket för webbservrar i mer än 15 år nu. Här är några av PHPs fördelar:

- <b><i>Cross-Platform:</i></b> PHP är plattformsoberoende. Du behöver inte ha ett speciellt operativsystem för att använda det eftersom det körs på alla plattformar, oavsett om det är Mac, Windows eller Linux.

- <b><i>Öppen källkod:</i></b> PHP är öppen källkod. Den ursprungliga koden görs tillgänglig för alla som vill bygga vidare på den. Detta är en av anledningarna till att ett av dess ramverk, Laravel, är så populärt.

- <b><i>Lätt att lära sig:</i></b> PHP är inte svårt att lära sig för absoluta nybörjare. Du kan plocka upp det ganska om du redan har programmeringskunskaper.

- <b><i>PHP synkroniserar med alla databaser:</i></b> Du kan enkelt koppla PHP till alla databaser, relationella och icke-relationella. Så den kan ansluta på nolltid till MySQL, Postgress, MongoDB eller någon annan databas.

- <b><i>Stödjande gemenskap:</i></b> PHP har en mycket stödjande gemenskap på nätet. Den officiella dokumentationen ger guider om hur du använder funktionerna och du kan enkelt fixa ditt problem medan du fastnar.

### Att skriva "Hello-World" i PHP 

Först och främst måste man ha PHP installerat på sin lokala dator. Man kan få det gjort genom att installera en XAMP-server (Cross-Platform, Apache, MySQL och PHP) eller WAMP (Windows, Apache, MySQL och PHP). Jag använder XAMP-Server. 

XAMP fungerar på alla operativsystem och WAMP fungerar bara i Windows. Jag kommer att använda XAMP.

En Xamp-server ser ut så efter installation.

![Bild-2-PHP](/images/BE/xamp.png)

<b>Öppna installationskatalogen, Jag använder Mac, Under Application - XAMPP mapp </b> 

![Bild-4-PHP](/images/BE/app-Xamp.png)

<b> XAMPP - htdocs mapp. I htdocs skapa en mapp som heter Php </b>

![Bild-3-PHP](/images/BE/CIndex.png)

<b> Öppna mappen PHP, i PHP mappen skapa en fil som heter main.php i VISUAL STUDIO CODE och skriv php  koder </b>

![Bild-5-PHP](/images/BE/helloworld-1.png)



## BE 1.2 OOP i PHP

Objektorienterad programmering (OOP) är ett programmeringsparadigm som gör det möjligt för utvecklare att strukturera och behandla sina applikationer som verkliga objekt genom att använda klasser för att bunta data och funktioner i en enda enhet och använda dem i hela applikationen, och därigenom förbättra läsbarheten, återanvändbarheten, underhållbarhet med mera.

Förutom att vara ett av de mest populära programmeringsparadigmen, är det också det mest använda i PHP. De flesta PHP-ramverk och CMS, som Laravel, Drupal, Symphony, October, CodeIgniter och många andra använder OOP i sin kärna. Även delar av världens mest populära webbplatsbyggare, WordPress, använder OOP.

### Klasser 

Som nämnts i föregående avsnitt är objektorienterad programmering baserad på klasser, och kommer att utforska dem i det här avsnittet. Om du till exempel vill skapa <i>en användarklass</i> kan du använda klassnyckelordet:

```
<?php
    class student { 

    }
?>    
```

Koden ovan definierar två offentliga egenskaper ($name och $age), en skyddad egenskap ($email) och en privat egendom ($password) i Student-klassen. Alla klassegenskaper definieras genom att egenskapen prefixeras med offentliga, skyddade eller privata nyckelord.

Det finns tre åtkomstnivåer i PHP. Offentliga egenskaper kan nås inom och utanför klassen, och skyddade egenskaper kan användas i klassen som definierar dem och klasserna som ärver dem. Däremot kan privata egenskaper endast nås inom den klass som definierar dem.

### Klassegenskaper 

PHP låter dig lägga till egenskaper till klasser. Klassegenskaper är variabler som du definierar inom klassens parenteser { } och kan användas inom och utanför klassen. Du kan definiera en egenskap i en klass:

```
<?php
class student {
       public $name = 'William Berhane';
       public $age = '35';
       protected $email = 'william.berhane@chasstudent.se';
       private $password = 'admin123';
}
?>  
```

### Klassmetoder 

Du kan lägga till funktioner i klasser genom att definiera dem inom klassens hängslen { }:

```
<?php
    class student {
       function greeting(){
              echo ' Hello,  '  .$this -> name . ' and welcome to the site!';
       }
    }
?>     

```

Koden ovan definierar en hälsningsfunktion som skriver ut ett meddelande till användaren. Funktioner kan också vara antingen offentliga eller privata, och du kan definiera offentliga, skyddade och privata funktioner i klassen genom att prefixa dem med antingen offentliga, skyddade eller privata nyckelord:

```
<?php
    class student {
       public function getPassword(){
             return $this -> $password;
       }

       private function setPassword(password){
              $this -> $password = $password;
       }
    }
?>     

```

Koden ovan deklarerar en offentlig funktion, getPassword, och en privat funktion, setPassword. Nyckelordet $this används för att komma åt klassegenskaperna och metoderna i klassen, vilket betyder att du måste använda $this->age istället för $age för att komma åt egenskapen public age.


### Skapa Objekt

Studentklassen som skapade i de föregående avsnitten gör ingenting ännu; för att använda klassen måste man skapa ett objekt från klassen. Till exempel, för att skapa ett objekt baserat på klassen Student använder du det nya nyckelordet:

```
    $student = new Student;
```

Koden ovan skapade ett objekt, student1, med klassen Student som en ritning. Du kan nu använda egenskaperna och funktionerna för studentklassen så här:

```
    echo $student -> name . ' is ' .$student-> age . ' years old. ';
    echo "<br>";
    echo $student -> greeting();
    echo "<br>";
    echo $student -> getPassword();
    echo "<br>";
```

Koden ovan använder syntaxen med en pil (->) för att komma åt egenskaperna och funktionerna för användarobjektet och skriver ut följande i webbläsaren:

<mark> William Berhane is 35 years old.  </mark> <br>
<mark> Hello, William Berhane and Welcome to the site! </mark> <br>
<mark> Admin123  </mark>

Klassen du skapade i det här avsnittet är inte skalbar eftersom alla objekt som skapas med den alltid kommer att ha samma namn, ålder, e-post och Password-värden. Låt oss undersöka hur man gör det dynamiskt i följande avsnitt.

### _Konstruktormetoden

PHP tillhandahåller en magisk metod, __construct, även känd som konstruktormetoden. Det används i klasser för att initiera egenskaper för nya objekt. Låt oss skriva om klassen Student för att använda en konstruktormetod:

```
<?php

    class Student {
    public $name;
    public $age;
    public $email;
    private $password;

    function __construct($name, $age, $email, $password) {
        $this->name = $name;
        $this->age = $age;
        $this->email = $email;
        $this->password = $password;
    }

    function greeing() {
        echo 'Hello,  ' . $this->name . ' and welcome to the site!';
    }

    public function getPassword() {
        return $this->ssn;
    }

    private function setPassword($Password) {
        $this->password = $password;
    }
}

?>
```

Koden ovan skapar en dynamisk studentklass genom att kräva att varje objekt anger dess namn, ålder, e-post och Password-egenskaper vid skapandet. Du kan nu skapa ett objekt i klassen Student:

```
<?php

$student1 = new Student('Elijah William', 25, "ElijahWilliam@gmail.com", '123-456');

$student2 = new Student('Eva Willliam', 20, "Evawilliam@gmail.com", '654-321');

echo $student1->name . ' is ' . $student1->age . ' years old.';
echo "<br>";
echo $student1->greeting();
echo "<br>";
echo $student1->getPassword();

echo "<br>"; 
echo "<br>";

echo $Student2->name . ' is ' . $Student2->age . ' years old.';
echo "<br>";
echo $Student2->greet();
echo "<br>";
echo $Student2->getSSN();

?>
```

Koden ovan kommer att skriva ut följande resultat med namn, ålder, e-post och SSN-egenskaper när objekt skapas:

<mark> Elijah William is 25 years old. </mark> <br>
<mark> Hello, Elijah William and welcome to the site! </mark><br>
<mark>  123-456 </mark> <br>
<br></br>

<mark>  Eva William is 20 years old. </mark> <br>
<mark> Hello, Eva William and welcome to the site! </mark> <br>
<mark>  654-321 </mark> <br>

Med denna syntax kan du nu skapa hur många objekt du vill med olika detaljer. Dessutom kommer du att få ett felmeddelande om du inte tillhandahåller alla egenskaper som anges i konstruktorn för varje objekt du skapar.

```
   Obs: Klassnamn är skiftlägesokänsliga, vilket innebär att du kan skapa ett användarobjekt så här: $student2 = new student(... )eller så här: $student2 = new STundent(.... ) Du bör dock alltid försöka överensstämma med namngivningen genom att använda den konventionella kamelbokstaven, som börjar med en stor bokstav.
```

### Inkapsling i PHP

Inkapsling i programmering avser att bunta relaterade data och funktioner i en enda enhet. Detta tillvägagångssätt förbättrar återanvändbarhet, läsbarhet och underhållsbarhet.

Inkapsling kan uppnås i PHP genom att använda klasser för att organisera din kod. Om du till exempel bygger en e-handelsapplikation kan du ha en klass som hanterar användarautentisering och en annan som hanterar kassaprocessen. Detta gör att flera utvecklare kan samarbeta och arbeta med ett projekt med minimal eller ingen konflikt samtidigt som de fokuserar på olika delar av koden.

### Klassarv 

När du utvecklar applikationer med ett objektorienterat paradigm kan du skriva ännu mindre kod genom att använda klassarv i PHP. Till exempel, när du bygger en e-handelsapplikation kan du ha en klass som heter Produkt med egenskaper som namn, pris, beskrivning och bild och metoder som formatPrice och addToCart. Du kan skapa klassen så här:

```
class Product {
    public $name;
    public $price;
    public $desc;
    public $image;

    function __construct($name, $price, $desc, $image) {
        $this->name = $name;
        $this->price = $price;
        $this->desc = $desc;
        $this->image = $image;
}
    final function formatPrice(){
        return "$". $this->price . "<br>";
    }
    public function addToCart(){
        return $this->name . " has been added to cart  <br> <br>";
    }
}
```

Koden ovan definierar en klass Produkt med fyra egenskaper ($namn, $price, $desc och $image) och två metoder (formatPrice och addToCart).

```
   Det sista nyckelordet som föregår formatPrice-funktionerna innebär att funktionen inte kan åsidosättas i klasserna som ärver klassen Product.
```


Du kan nu skapa flera klasser baserat på produktklassen:


```
class Laptop extends Product {
    public $cpu;
    public $ram;
    public $storage;

    function __construct($name, $price, $desc, $image, $cpu, $ram, $storage) {
        parent::__construct($name, $price, $desc, $image);
        $this->cpu = $cpu;
        $this->ram = $ram;
        $this->storage = $storage;
    }

    public function addToCart(){
        return $this->name . " has been overidden  <br> <br>";
    }

    public function formatLaptopSpecs(){
        return $this->name . "<br>" . "i" . $this->cpu . " Processor <br>" . $this->ram . "GB RAM <br>" . $this->storage . "GB SSD <br> <br>";

    }
}

class Phone extends Product {
    public $os;
    public $ram;
    public $storage;

    function __construct($name, $price, $desc, $image, $os, $ram, $storage) {
        parent::__construct($name, $price, $desc, $image);
        $this->os = $os;
        $this->ram = $ram;
        $this->storage = $storage;
    }

    public function formatPhoneSpecs(){
        return $this->name . "<br>" . $this->os . "<br>" . $this->ram . "GB RAM <br>" . $this->storage . "GB <br> <br>";

    }
}

class TV extends Product {
    public $screenSize;
    public $resolution;
    public $refreshRate;

    function __construct($name, $price, $desc, $image, $screenSize, $resolution, $refreshRate) {
        parent::__construct($name, $price, $desc, $image);
        $this->screenSize = $screenSize;
        $this->resolution = $resolution;
        $this->refreshRate = $refreshRate;
    }

    public function formatTVSpecs(){
        return $this->name . "<br>" . "Screen Size: " . $this->screenSize . "<br>" . "Resolution: " .$this->resolution . "<br>" . "Refresh Rate: " .$this->refreshRate . "<br> <br>";
    }
}
```

Koden ovan definierar tre olika produkter med ytterligare egenskaper och metoder genom att utöka klassen Produkt. Nyckelordet extends används för att utöka produktklassen, även känd som överordnad klass i detta fall.


```

    Obs:   Laptopklassen åsidosatte produktklassens addToCart-funktion genom att definiera en annan addToCart-funktion.

```

Du kan nu använda klasserna så här:


```

$tv = new TV('LG TV', 1000, 'A TV', 'image.jpg', '55"', '4K', '60Hz');
echo $tv->formatTVSpecs();
echo $tv->addToCart();

$phone = new Phone('iPhone 12', 1000, 'A phone', 'image.jpg', 'iOS', 8, 256);
echo $phone->formatPhoneSpecs();
echo $phone->addToCart();

$laptop = new Laptop('Macbook Pro', 1000, 'A laptop', 'image.jpg', '5', 16, 512);
echo $laptop->formatLaptopSpecs();
echo $laptop->addToCart();  

```

Koden ovan definierar en instans av klasserna som utökar produktklassen och kommer att returnera följande resultat:

<mark> LG TV </mark>  <br>
<mark> Screen Size: 55" </mark>  <br>
<mark> Resolution: 4K </mark>  <br>
<mark> Refresh Rate: 60 Hz </mark>  <br></br>

<mark> LG TV has been added to cart </mark>  <br></br>

<mark> iPhone 12 </mark>  <br>
<mark> iOS </mark>  <br>
<mark> 8GB RAM </mark>  <br>
<mark> 256 GB </mark>  <br> </br>

<mark> iPhone 12 has been added to cart </mark>  <br></br>

<mark> Macbook Pro </mark>  <br>
<mark> i5 Processor </mark>  <br>
<mark> 16 GB RAM </mark>  <br>
<mark> 512 GB SSD </mark>  <br></br>

<mark> Macbook Pro has been overidden </mark>  <br>

```
   En klass som utökar en annan klass kallas en barnklass, medan en klass som utökas kallas en föräldraklass.
```

### Fördelar med arv

Arv låter dig återanvända kod genom att skapa nya klasser som ärver attributen och metoderna för befintliga klasser. Detta kan spara mycket tid eftersom du inte behöver skriva samma kod upprepade gånger. Det kan göra koden lättare att underhålla eftersom om en bugg hittas i föräldraklassen behöver den bara fixas en gång, och alla underordnade klasser kommer automatiskt att ärva korrigeringen.

Arv skapar en hierarkisk klassstruktur, vilket gör koden lättare att förstå och organisera. Du kan använda förälder-barn-relationen för att gruppera klasser i logiska kategorier, vilket gör det lättare att navigera och underhålla kodbasen. Slutligen gör det att du kan lägga till nya funktioner eller funktionalitet till en applikation utan att ändra den befintliga koden.

### Statiska medlemmar 

PHP låter dig definiera egenskaper och metoder bundna till klassen och inte instanser med hjälp av det statiska nyckelordet. Vi kommer att utforska hur man gör det i det här avsnittet.

### Statiska Egenskaper 

Statiska egenskaper är endast tillgängliga att använda på själva klassen och inte instanserna. Om du till exempel vill hålla reda på hur många gånger användarklassen har använts kan du göra det så här:

```
class User {
    public $name;
    public $email;
    public $password;

    function __construct($name, $email, $password) {
        $this->name = $name;
        $this->email = $email;
        $this->password = $password;
    }
    static $usersCount = 0;
}
```

Koden ovan definierar en statisk egenskap, med hjälp av Count, inuti klassen User. Du kan nu komma åt egenskapen genom att prefixa den med self:: syntax:

```
    $user = new User('Eva William', 'williameva@gmail.com', 'password');
    echo User::$usersCount; // 0

```

Koden ovan returnerar värdet för usersCount, 0.

```
  Obs: Du måste lägga till $ till egenskapen.
```

Låt oss ta en titt på statiska metoder härnäst.

### Statiska Metoder

Om du vill uppdatera usersCount varje gång en instans av User skapas kan du använda den statiska metoden:

```

   class Student {
    // same as above...

    static function updateUsersCount(){
        self::$usersCount++;
        return self::$usersCount . " users registered";
    }
}

```

Koden ovan definierar en updateUsersCount-metod som uppdaterar egenskapen usersCount. Du kan nu anropa funktionen updateUsersCount på klassen varje gång en instans av klassen User skapas:

```

   $student = new Student('Eva William', 'williameva@gmail.com', 'password');
   echo User::updateUsersCount(); // 1 users registered
   echo User::$usersCount; // 0

```

### Abstrakta klasser och metoder 

PHP låter dig definiera klasser med funktioner som inte är definierade ännu, men tvingar klasser som utökar dem att definiera deras implementering. Abstrakta klasser och metoder skapas genom att prefixet klass- och metodnamnen läggs till det abstrakta nyckelordet.

Om du till exempel vill tvinga varje underordnad klass som utökar produktklassen att implementera en formatSpec-funktion, kan du göra det med en abstrakt klass:

```

abstract class Product {
    public $name;
    public $price;
    public $desc;
    public $image;

    function __construct($name, $price, $desc, $image) {
        $this->name = $name;
        $this->price = $price;
        $this->desc = $desc;
        $this->image = $image;
    }

    public function addToCart(){
        return $this->name . " has been added to cart  <br> <br>";
    }

    abstract function formatSpec();
}

```

Koden ovan definierar en abstrakt produktklass med en abstrakt formatSpec-metod. Du kan inte skapa ett objekt baserat på en abstrakt klass. Du måste skapa klasser som utökar den.

```
   En abstrakt klass måste ha minst en abstrakt metod.
```

Du kan nu skapa en barnklass som utökar den abstrakta klassen:

```
class Laptop extends Product {
    public $cpu;
    public $ram;
    public $storage;

    function __construct($name, $price, $desc, $image, $cpu, $ram, $storage) {
        parent::__construct($name, $price, $desc, $image);
        $this->cpu = $cpu;
        $this->ram = $ram;
        $this->storage = $storage;
    }

    public function formatSpec(){
        return $this->name . "<br>" . "i" . $this->cpu . " Processor <br>" . $this->ram . "GB RAM <br>" . $this->storage . "GB SSD <br> <br>";
    }
}
```

Koden ovan definierar en Laptop-klass som utökar produktklassen och implementerar formatSpec-funktionen inuti den.

### Gränssnitt

PHP tar abstraktionen till nästa nivå genom att låta dig definiera funktioner som klasser måste implementera i ett gränssnitt. Ett gränssnitt liknar en abstrakt klass men kan bara ha publika funktioner och kan inte innehålla egenskaper och definierade metoder. Här är ett exempel på ett gränssnitt:

```

interface ProductInterface {
    public function addToCart();
    public function formatSpec();
}

```

Koden ovan definierar ett ProductInterface med två metoder som den underordnade klassen måste implementera. En child klass som implementerar produktgränssnittet kommer att se ut så här:

```

class Phone implements ProductInterface {
    public $name;
    public $price;
    public $desc;
    public $image;
    public $os;
    public $ram;
    public $storage;

    function __construct($name, $price, $desc, $image, $os, $ram, $storage) {
        $this->name = $name;
        $this->price = $price;
        $this->desc = $desc;
        $this->image = $image;
        $this->os = $os;
        $this->ram = $ram;
        $this->storage = $storage;
    }

    public function addToCart(){
        return $this->name . " has been added to cart  <br> <br>";
    }

    public function formatSpec(){
        return $this->name . "<br>" . $this->os . "<br>" . $this->ram . "GB RAM <br>" . $this->storage . "GB <br> <br>";
    }
}

```

Koden ovan definierar en telefonklass baserad på produktgränssnittet med hjälp av nyckelordet implements.


### Skillnaden mellan Abstrakta Klasser och gränssnitt
<hr>

|               |Klasser        |Gränssnitt    |
|---------------|---------------|--------------|
| Implementering | Kan ha både abstrakta och konkreta metoder med full implementering | Kan bara ha abstrakta metoder |
| Egenskaper | Kan ha egenskaper | Kan inte ha egenskaper |
| Konstanter  | Kan ha konstanter | Kan ha konstanter |
| Arv  | Kan utöka en abstrakt klass (enkelt arv), men det kan implementera flera gränssnitt (flera pseudo-arv)  | n/a | 
| SynlighetsMetoder | Kan ha offentliga och skyddade klasssynligheter | Alla metoder måste vara offentliga |
| Design Syfte | Används när klasser delar en gemensam bas av operationer | Används när man upprättar ett gemensamt gränssnitt för olika klasser oavsett arvshierarkin. |


### Polymorfism

Ordet polymorfism kommer från två grekiska ord, poly, som betyder olika eller många, och morph, som betyder form eller form. Polymorfism är ett grundläggande koncept i OOP som gör att objekt av olika klasser kan användas omväxlande samtidigt som de behåller sitt unika beteende. Det gör att du kan skriva mer flexibel, modulär och lättare att underhålla kod.

Polymorfism i PHP uppnås genom att använda abstrakta klasser eller gränssnitt för att skriva kod som enkelt kan utökas och modifieras utan att modifiera den befintliga koden. Det låter dig också skriva mer generisk kod som kan fungera med objekt i olika klasser istället för att skriva separat kod för varje klass. Detta minskar kodduplicering och ökar kodåteranvändbarheten, vilket gör din kod mer effektiv och underhållbar.

### Egenskaper

PHP låter dig definiera och använda funktioner som inte passar i en klass med egenskaper. En egenskap är en samling funktioner som kan användas i klasser utan att ärva, utöka eller implementera en klass eller gränssnitt.

Till exempel kan du definiera en egenskap som innehåller en addBrandLogo-funktion, som kan användas i alla andra klasser för att lägga till en varumärkeslogotyp till produktbilder:

```

trait AllProductsFunctions {
    public function addBrandLogo(){
        return "Brand logo added";
    }
}

```

Koden ovan definierar en egenskap (AllProductsFunctions) med en metod (addBrandLogo) inuti den. Denna egenskap kan nu användas i andra klasser med hjälp av nyckelordet use:

```

class Phone implements ProductInterface {
           // same as before...
    use AllProductsFunctions;
          // same as before...
}

```

Funktionen i egenskapen AllProductsFunctions kan nu användas på alla objekt baserat på Phone-klassen. Du kan använda flera egenskaper i en klass genom att separera egenskapernas namn med ett kommatecken.

### Fördelar med objektorienterad programmering

Nu när du har lärt dig alla grunder och avancerade begrepp du behöver veta för att börja objektorienterad programmering i PHP och hur det hjälper dig att designa och skapa skalbara, underhållsbara och återanvändbara applikationer, låt oss utforska några av de betydande fördelarna med OOP i följande avsnitt.

### Kod återanvändbarhet

En av de främsta fördelarna med OOP i PHP är kodåteranvändning. Det betyder att du kan återanvända kodblock och funktioner i applikationer utan att behöva skriva om hela koden från början. Med OOP kan du skapa objekt som kapslar in en specifik uppsättning funktioner och återanvända dessa objekt över flera applikationer eller till och med inom samma applikation. Detta hjälper till att minska utvecklingstiden och ansträngningen som krävs för att skapa komplexa applikationer samtidigt som den övergripande kvaliteten på koden förbättras.

### Skalbarhet

OOP i PHP gör det också lättare att skala applikationer när de växer. Genom att använda objekt för att kapsla in olika delar av applikationen kan du ändra eller lägga till nya funktioner utan att påverka andra delar av kodbasen. Detta gör det lättare att underhålla och uppdatera applikationer samtidigt som risken för introduktion av buggar eller fel minskar. Dessutom gör OOP det lättare att modularisera kod, vilket gör att flera utvecklare kan arbeta med specifika delar av applikationen utan att behöva förstå hela kodbasen.

### Inkapsling

Inkapsling är en avgörande princip för OOP i PHP som hjälper till att förbättra en applikations säkerhet och underhållbarhet. Med inkapsling kan du dölja ett objekts interna funktion från resten av applikationen. Detta innebär att objektet endast kan nås via dess publika gränssnitt, vilket hjälper till att förhindra obehörig åtkomst till kritiska delar av applikationen. Inkapsling gör det också lättare att modifiera eller uppdatera ett objekts interna funktion utan att påverka andra delar av kodbasen.

### Arv

Arv är ett annat viktigt koncept i OOP som låter utvecklare skapa nya klasser baserat på befintliga klasser. Med arv kan du ärva egenskaperna och metoderna för en överordnad klass och sedan ändra eller utöka dem för att skapa ny funktionalitet. Detta gör återanvändning av kod enklare, minskar redundans och skapar effektivare applikationer. Dessutom bidrar arv till att främja konsistens över olika delar av en applikation, vilket gör det lättare att underhålla och uppdatera kodbasen.

### Testbarhet

Slutligen, OOP i PHP gör det lättare att testa och felsöka applikationer. Genom att kapsla in kod i objekt kan du isolera specifika delar av applikationen och testa dem isolerade från andra delar av kodbasen. Detta hjälper till att identifiera buggar och fel snabbare och gör det lättare att fixa dem utan att påverka resten av applikationen. Dessutom gör OOP det enklare att skriva automatiserade tester som kan användas för att testa applikationen i skala, vilket hjälper till att förbättra den övergripande kvaliteten på koden.

Att använda OOP i PHP erbjuder en rad fördelar som kan hjälpa dig att skapa mer skalbara, underhållsbara och återanvändbara applikationer. Som sådan har OOP blivit en populär programmeringsteknik för att bygga moderna webbapplikationer och kommer sannolikt att förbli en viktig del av verktygslådan för utvecklare i flera år.

#### Slutsats

Och det är allt! Jag hoppas att den här artikeln uppnådde sitt syfte att lära dig objektorienterad programmering i PHP. Du lärde dig om klasser i PHP, inklusive klassegenskaper, klassmetoder, kedjeklassmetoder i PHP, vanliga klasskonstanter i PHP och klassarv. Vi undersökte också hur man använder statiska medlemmar, abstrakta klasser och metoder, gränssnitt, polymorfism och egenskaper.

## BE 1.3 Säkerhet i PHP
Beskriv rubriken här

## BE 1.4 MVC
Beskriv rubriken här

## BE 1.5 Wordpress
Beskriv rubriken här

## BE 1.6 Heirarkiska databaser
Beskriv rubriken här

## BE 1.7 Relationsdatabaser, SQL och ER-modellering
Beskriv rubriken här

## BE 1.8 OAuth i backend
Beskriv rubriken här

## BE 1.9 HTTP-protokollet
Beskriv rubriken här

## BE 1.10 cURL
Beskriv rubriken här

## BE 1.11 REST
Beskriv rubriken här

## BE 1.12 XML och andra dataformat
Beskriv rubriken här

## BE 1.13 Webbservrar
Beskriv rubriken här



### Källor:

(OOP i PHP) https://medium.com/@imadevguyanand/php-what-is-oop-413b566f9a94 