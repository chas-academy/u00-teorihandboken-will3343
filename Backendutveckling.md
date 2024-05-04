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

När du använder PHP finns alltid en risk att dina script blir manipulerade. Målsättningen med den här guiden är att göra dig medveten om problemen. 

### SQL-Injektion

SQL-injektion är möjligen den vanligaste attacken mot PHP-applikationer. Det fungerar genom att lura kod på serversidan att skicka skadliga SQL-kommandon till databasen. Dessa SQL-frågor kan returnera information som den ursprungliga webbapplikationsutvecklaren inte vill avslöja – inklusive hela innehållet i databasen, personlig information, lösenord etc. I andra fall kan skadliga frågor användas för att äventyra databasen eller värdsystemet.

Till exempel använder följande fråga nedan osanifierad användarinmatning direkt i SQL-frågan:

```
    // Skapa SQL

$sql = "VÄLJ * FRÅN 'användare' WHERE 'id'=”’” . mysql_stgring($_GET[id]) . "'";

// Kör frågan

$users = mysql_query($sql);
```

Detta gör att en hackare kan bryta uttalandet och fråga efter ytterligare information, inklusive alla användares data.

### XSS (Cross-Site Scripting)

Cross Site Scripting (XSS) tillåter angripare att köra skadlig JavaScript på webbplatser för att utföra skadliga åtgärder mot webbplatsanvändare. Detta fungerar vanligtvis genom att injicera skriptkod på klientsidan tillsammans med legitimt innehåll. När en intet ont anande användare försöker besöka webbplatsen, körs koden i användarens webbläsare och kan användas för att kapa deras session, ladda ner skadlig programvara eller omdirigera användaren till en skadlig webbplats.

### Cross-Site Request Forgery (CSRF)

Cross-Site Request Forgery (CSRF)-attacker tvingar slutanvändare att utföra oönskade åtgärder på en webbapp där de är autentiserade. Genom att använda social ingenjörsteknik, som att skicka skadliga länkar i ett e-postmeddelande, kan angripare lura användare av ett målprogram att köra skadliga skript.

Om en CSRF-attack framgångsrikt riktar sig mot normala användare, kan den tvinga dem att utföra förfrågningar som ändrar applikationsstatus, som att överföra pengar eller ändra deras e-postadresser. Om attacken riktar sig mot ett administrativt konto kan det äventyra hela webbapplikationen.

### Session och Cookie-kapning

Cookies är filer som lagrar användaruppgifter och hjälper användare att upprätthålla en session även efter att de lämnat en webbplats. Det betyder att om en hackare stjäl en användares cookie kan de logga in på sitt konto utan inloggningsuppgifter.

Webbplatser som hanterar PHP-sessioner tenderar att lagra sessionsdata på webbservern. Men när webbläsaren skickar en sessionsidentifierare som en cookie kan angripare fånga upp detta och använda det för att utge sig för användaren.

### Buffertspill

Ett buffertspill är ett vanligt programmeringsfel i programmeringsspråken C och C++. PHP-kod kan inte direkt orsaka buffertspill, men C-kod i PHP-motorn kan resultera i buffertspill. Detta innebär att många PHP-system är sårbara för denna attack.

En buffert är ett minneslagringsområde som tillfälligt lagrar data medan det överförs mellan olika platser. Ett buffertspill (eller överskridande) inträffar när datavolymen överstiger minnesbuffertens lagringskapacitet. Som ett resultat kommer ett program som försöker skriva data till bufferten att skriva över angränsande minneslagringsplatser.

### Källkodsexponering

PHP är ett språk på serversidan. Precis som skript på serversidan är kodens källkod inte avsedd att delas med användare. Till exempel, om du begär källan till en .php-tilläggsfil, kommer servern att köra PHP-koden som finns i filen och returnera den resulterande HTML-koden till användaren, vilket innebär att tredje part inte ska ha tillgång till PHP-skripten.

Men om servern är felkonfigurerad kommer den att returnera skriptet i vanlig text och ange deras ursprung. Vissa av dessa skript är mycket exploaterbara eftersom de sannolikt innehåller känslig information som databasuppgifter och konfigurationsfildetaljer.

### Uppdatera din PHP-version regelbundet

Det är viktigt att använda en uppdaterad PHP-version, eftersom nya versioner vanligtvis innehåller patchar för nyupptäckta säkerhetsproblem. Om man inte uppdaterar till den senaste stabila versionen kan hackare utnyttja kända sårbarheter.

PHP tillhandahåller förhandsversioner av nyare versioner, men det är vanligtvis inte en bra idé att delta i förhandsgranskningstestning, eftersom förhandsversioner kan innehålla okända säkerhetsbrister.

### Använd SSL-certifikat för HTTPS

Alla moderna webbläsare som Google Chrome, Opera och Firefox rekommenderar att man använder HTTPS-protokollet för webbapplikationer. HTTPS tillhandahåller en säker, krypterad kanal för att komma åt webbplatser. Det härdar också webbapplikationer mot XSS-attacker och förhindrar hackare från att fånga upp överförd data (känd som man i mitten-attacker).

För att stödja HTTPS måste din PHP-webbplats ha ett SSL-certifikat installerat och omdirigera all trafik från HTTP till HTTPS, för att undvika all trafik som flyter över en osäker HTTP-kanal.

### Logga alla fel och visa dem inte i produktionen

När du har utvecklat en PHP-webbplats och distribuerat den till en liveserver är det första du bör göra att inaktivera felvisning, eftersom hackare kan hämta värdefull information från fel. Ställ in följande parameter i din php.ini-fil:

```
display_errors=OFF
```

Se dock till att fel loggas och sparas på en säker plats för senare användning. Filsökvägen nedan är bara ett exempel.

```
log_errors=På

error_log=/var/log/httpd/php_scripts_error.log
```

### Använd förberedda SQL-satser

Att infoga användarindata direkt i en SQL-sats är ett vanligt misstag. Det lämnar dörren öppen för SQL-injektionsattacker eftersom användaren kan undergräva avsedda SQL-frågor och exekvera godtyckliga frågor.

Förberedda uttalanden är en databasfunktion som säkerställer att frågor byggs på serversidan, utan att direkt använda användarindata för att strukturera frågan. Detta kan förhindra de flesta SQL-injektionsattacker.

Så här ser den förberedda uttalandekoden ut:

```
$stmt = $conn->prepare("INSERT INTO användare (förnamn, efternamn) VÄRDEN (?, ?)");

$stmt->bind_param("ss", $förnamn, $efternamn);
```

Funktionen bind_param anger vilken typ av data som SQL-frågan ska skicka, vilket säkerställer att parametrar inuti frågan är av typen String. Detta är en stark säkerhetsåtgärd som validerar indata.

### Validera alltid användarinmatning

Förutom förberedda uttalanden är en sekundär säkerhetsåtgärd att validera alla användarinmatningar som accepteras av applikationen, för att säkerställa att all data är av rätt typ och format. Det är viktigt att validera datatyp, längd och format för användarinmatning och avvisa indata som inte matchar förväntade konventioner. Om möjligt, använd en godkännandelista med förväntade värden och validera indata endast om den matchar ett av de tillåtna värdena.

### Använd URL-kodning

PHP förser utvecklare med urlencode-funktionen för att säkert konstruera giltiga webbadresser. Enligt PHP-dokumentation kan denna funktion användas för att koda en sträng som används i frågedelen av en URL.

I allmänhet rekommenderas det inte att inkludera användarinmatningar i webbadresser. Men eftersom detta ibland görs i praktiken är det viktigt att koda alla dynamiskt genererade webbadresser för att säkerställa att skadliga indata automatiskt konverteras till strängar.

## BE 1.4 MVC

MVC är ett mjukvaruarkitektoniskt mönster för att implementera användargränssnitt på datorer. Den delar upp en given applikation i tre sammankopplade delar. Detta görs för att skilja interna representationer av information från hur information presenteras för och accepteras av användaren.

- MVC står för "Model view And Controller".
- Huvudsyftet med MVC Architecture är att separera affärslogik och applikationsdata från ANVÄNDARgränssnittet.
- Olika typer av arkitekturer finns tillgängliga. Dessa är 3-tier Architecture, N-tier Architecture, MVC Architecture, etc.
- Den största fördelen med arkitektur är återanvändbarhet, säkerhet och ökad applikations prestanda.

![Bild-6-PHP](/images/BE/mvc.png)

- Modell: Databasoperation som att hämta data eller uppdatera data etc.

- Visa: GUI för slutanvändare genom vilket användaren kan interagera med systemet, dvs HTML, CSS.

- Controller: Innehåller affärslogik och ger en länk mellan modell och vy.


### Model 

- Modellobjektet vet allt om all data som behöver visas.
- Modellen representerar applikationsdata och affärsregler som styr en uppdatering av data.
- Modellen är inte medveten om presentationen av data och hur data kommer att visas för webbläsaren.

### View 

- Vyn representerar presentationen av applikationen.
- View-objektet hänvisar till att modellen förblir densamma om det finns några ändringar i affärslogiken.
- Med andra ord kan vi säga att det är åsiktens ansvar att upprätthålla konsekvens i sin presentation och modellförändringar.

### Kontroller 

- Närhelst användaren skickar en begäran om något går det alltid via Controller.
- En personuppgiftsansvarig är ansvarig för att avlyssna begäran från synhåll och övergår till modellen för lämplig åtgärd.
- Efter att åtgärden har vidtagits på uppgifterna är den personuppgiftsansvarige ansvarig för att direkt överföra lämplig vy till användaren.
- I grafiska användargränssnitt arbetar styrenhet och vy väldigt nära varandra.


## BE 1.5 Wordpress

WordPress är en gratis plattform för att skapa webbplatser med öppen källkod. På en mer teknisk nivå är WordPress ett innehållshanteringssystem (CMS) skrivet i PHP som använder en MySQL-databas. I non-geek talk är WordPress den enklaste och mest kraftfulla blogg- och webbplatsbyggaren som finns idag.

WordPress är en utmärkt webbplatsplattform för en mängd olika webbplatser. Från bloggande till e-handel till företag och portföljwebbplatser, WordPress är ett mångsidigt CMS. Designad med användbarhet och flexibilitet i åtanke, WordPress är en bra lösning för både stora och små webbplatser.

![Bild-7-PHP](/images/BE/wordpress.png)

En WordPress-webbplats är vilken webbplats som helst som använder WordPress som sitt innehållshanteringssystem [CMS](https://kinsta.com/knowledgebase/content-management-system/). WordPress driver både backend av webbplatsen (gränssnittet där en användare loggar in för att göra ändringar eller lägga till nytt innehåll) och frontend (den synliga delen av webbplatsen som dina besökare ser på webben).

Här är bara några exempel på de typer av webbplatser du kan bygga med WordPress:

- Blogg – En blogg är en speciell typ av webbplats som ägnar sig åt att dela tankar, foton, recensioner, handledning, recept och mycket mer. Bloggar visar vanligtvis det senast publicerade innehållet först.
- e-handelswebbplats – En e-handelswebbplats låter dig sälja varor eller tjänster online och samla in betalning via ett onlinebetalningssystem. Du kan ladda ner och installera ett WordPress-e-handelsplugin för att utöka standardfunktionaliteten för WordPress så att du kan ha en onlinebutik på din webbplats.
- Företagswebbplats – Många företag kommer att dra nytta av att ha en onlinenärvaro i form av sin egen webbplats. Om ditt företag behöver en webbplats för kunder att lära sig om ditt företag och vad du har att erbjuda är WordPress ett utmärkt alternativ. Kunder kan kontakta dig, be om offert, boka tid och mycket mer.
- Medlemskapswebbplats – En medlemswebbplats låter dig lägga innehåll bakom en betalvägg eller en kontoinloggning. För att komma åt sidor eller inlägg måste användare logga in eller betala för innehållet. WordPress kan även hantera medlemswebbplatser med ytterligare plugins.
- Portföljwebbplats – Visa upp dina konstverk, designkunskaper och mer med en portföljwebbplats byggd på WordPress.
- Forumwebbplats – En forumwebbplats kan vara en användbar plats för användare att ställa frågor eller dela med sig av råd. Tro det eller ej, många forumwebbplatser körs på WordPress.
- Evenemangswebbplats – värd för ett event? WordPress gör det enkelt för dig att dela dina eventdetaljer och sälja biljetter.
- Webbplats för e-lärande – Studenter kan ta onlinekurser, spåra deras framsteg, ladda ner resurser och mycket mer från en e-lärande webbplats. Med en speciell typ av plugin som kallas WordPress LMS-plugin kan du erbjuda onlinekurser från en WordPress-webbplats.
- Bröllopswebbplats – Dela detaljerna om din stora dag med en bröllopswebbplats byggd på WordPress. Med en rad WordPress-bröllopsteman kan du få upp en webbplats snabbt och enkelt.

Möjligheterna är oändliga när det kommer till att anpassa en WordPress-webbplats. WordPress-teman och plugins kan lägga till nya designalternativ och extra funktionalitet. Kolla in WordPress.org för gratis teman och plugins.

### Några fördelar med WordPress

- Enkelhet: WordPress låter dig publicera och bygga ditt webbplatsinnehåll snabbt. Även som nybörjare kan du enkelt använda WordPress.
- Kostnaden är gratis – Själva WordPress-programvaran som finns tillgänglig på WordPress.org är gratis att ladda ner och använda. Du kommer dock att behöva betala för webbhotell och ett domännamn.
- Flexibilitet: WordPress låter dig skapa många typer av webbplatser, från personliga bloggar och nätbutiker till onlinetidningar och tidningar.
- Lätt att använda – Om du kan använda ett ordbehandlingsprogram som Microsoft Word kan du använda WordPress för att bygga och hantera en webbplats.
- Programvara med öppen källkod – WordPress är programvara med öppen källkod som är licensierad under [GNU General Public License (GPL)](https://wordpress.org/about/license/), vilket innebär att den inte ägs av ett enda företag eller enhet. Hundratals utvecklare och användare samarbetar och bidrar till programvaran för att förbättra den. Andan med öppen källkod innebär ständiga förbättringar, ansvarighet och gratis användning för alla.
- Inget behov av att känna till kod – WordPress tar bort kravet på att behöva veta hur man kodar för att bygga en webbplats. Medan WordPress använder en mängd olika kodspråk, behöver du inte känna till något av dem för att använda WordPress.
- Kan utökas med WordPress-plugins – WordPress-programvaran kan utökas med WordPress-plugins. WordPress-plugins är mjukvara som du kan ladda upp till din webbplats för att lägga till fler funktioner (som e-handel, SEO, säkerhetskopior, kontaktformulär och mer). Det finns tusentals gratis WordPress-plugins tillgängliga i WordPress.org-pluginkatalogen och en blomstrande premium (betalda) plugin-industri.
- Mycket anpassningsbar med WordPress-teman – WordPress-teman ger designen och layouten på din webbplats. Med ett klick på en knapp kan du ändra hela utseendet på din webbplats genom att använda ett nytt WordPress-tema. Mer avancerade WordPress-teman är mer som WordPress-sidbyggare, vilket ger dig ännu mer kontroll över dina layouter.
- Webbplatssäkerhet – Även om ingen webbplatsplattform är 100 % säker, fortsätter WordPress-säkerheten att förbättras med ett vaksamt säkerhetsteam av kärnutvecklare och användare. Vanliga WordPress-säkerhetsproblem beror vanligtvis på användarfel snarare än själva programvaran.
- En blomstrande gemenskap av användare och utvecklare – När du har en WordPress-webbplats kan du också engagera dig i den större WordPress-gemenskapen genom din lokala [WordPress Meetup](https://www.meetup.com/topics/wordpress/), [WordCamps](https://central.wordcamp.org/) och mer. WordPress-communityt har ett rykte om sig att vara otroligt välkomnande, hjälpsam och innovativ.


## BE 1.6 Heirarkiska databaser

En hierarkisk databas är en datamodell där data lagras i form av poster och organiseras i en trädliknande struktur, eller förälder-underordnad struktur, där en föräldernod kan ha många underordnade noder kopplade via länkar.

![Bild-8-PHP](/images/BE/hierarkiskaDB.png)

### Vad är en hierarkisk databas?

Som namnet antyder är den hierarkiska databasmodellen mest lämplig för användningsfall där huvudfokus för informationsinsamlingen baseras på en konkret hierarki, som att flera enskilda anställda rapporterar till en enskild avdelning på ett företag.

Schemat för hierarkiska databaser definieras av dess trädliknande organisation, där det vanligtvis finns en "överordnad" rotkatalog med data lagrad som poster som länkar till olika andra underkataloggrenar, och varje underkataloggren, eller underordnad post, kan länka till olika andra underkataloggrenar.

Den hierarkiska databasstrukturen dikterar att medan en överordnad post kan ha flera underordnade poster, kan varje underordnad post bara ha en överordnad post. Data i poster lagras i form av fält, och varje fält kan bara innehålla ett värde. Att hämta hierarkisk data från en hierarkisk databasarkitektur kräver att man korsar hela trädet, med början vid rotnoden
‍

### Hierarkisk databas vs relationsdatabas

En [relationsdatabas](https://cloud.google.com/learn/what-is-a-relational-database) är en digital databas baserad på relationsmodellen, som organiserar data i uppsättningar av tabeller med kolumner och rader. Raderna, även kända som poster, representerar en samling relaterade värden, och varje rad identifieras med en unik nyckel. Varje kolumn innehåller attribut av en specifik datatyp, och varje post har vanligtvis ett värde för varje attribut.

Skillnaden mellan relationella och hierarkiska databaser ligger i datastrukturerna. Medan den hierarkiska databasarkitekturen är trädliknande, lagras data i en relationsdatabas i tabeller med en unik identifierare för varje post. En relationsdatabasstruktur underlättar enkel identifiering och åtkomst av data i förhållande till andra datapunkter i databasen. Tabellerna är separata från fysiska lagringsstrukturer, vilket gör det möjligt för databasadministratörer att ändra fysisk datalagring utan att omorganisera själva databastabellerna.

Karakteristika för hierarkiska databasmodeller inkluderar deras enkelhet, men också deras brist på flexibilitet. Hierarkiska strukturer, till skillnad från relationsdatabaser, beskriver inte många-till-en-relationer eller många-till-många-relationer på grund av det faktum att underordnade poster bara kan ha en ensam förälder.
‍

### Hierarkisk databasmodell Fördelar och nackdelar

Den viktigaste fördelen med en hierarkisk databas är dess användarvänlighet. En-till-många-organisationen av data gör det enkelt och snabbt att gå igenom databasen, vilket är idealiskt för användningsfall som rullgardinsmenyer på webbplatser eller datormappar i system som Microsoft Windows OS. På grund av separationen av tabellerna från fysiska lagringsstrukturer kan information enkelt läggas till eller raderas utan att hela databasen påverkas. Och de flesta större programmeringsspråk erbjuder funktionalitet för att läsa trädstrukturdatabaser.

Den största nackdelen med hierarkiska databaser är deras oflexibla karaktär. En-till-många-strukturen är inte idealisk för komplexa strukturer eftersom den inte kan beskriva relationer där varje barnnod har flera föräldrarnoder. Också den trädliknande organisationen av data kräver sekventiell sökning från topp till botten, vilket är tidskrävande och kräver repetitiv lagring av data i flera olika enheter, vilket kan vara redundant.

## BE 1.7 Relationsdatabaser, SQL och ER-modellering

Entitetsrelationsmodellen är en modell för att identifiera enheter som ska representeras i databasen och representation av hur dessa enheter är relaterade. ER-datamodellen specificerar företagsschema som representerar den övergripande logiska strukturen för en databas grafiskt.

Entity Relationship Diagram förklarar förhållandet mellan de enheter som finns i databasen. ER-modeller används för att modellera verkliga objekt som en person, en bil eller ett företag och relationen mellan dessa verkliga objekt. Kort sagt är ER-diagrammet det strukturella formatet för databasen.

### Varför använda ER-diagram i DBMS?

- ER-diagram används för att representera E-R-modellen i en databas, vilket gör dem lätta att konvertera till relationer (tabeller).
- ER-diagram ger syftet med verkliga modellering av objekt som gör dem mycket användbara.
- ER-diagram kräver ingen teknisk kunskap och inget hårdvarustöd.
Dessa diagram är mycket lätta att förstå och lätta att skapa även för en naiv användare.
- Det ger en standardlösning för att visualisera data logiskt.
Symboler som används i ER-modellen
- ER Model används för att modellera den logiska vyn av systemet ur ett dataperspektiv som består av dessa symboler:

- Rektanglar: Rektanglar representerar enheter i ER-modellen.
- Ellipser: Ellipser representerar attribut i ER-modellen.
- Diamant: Diamanter representerar relationer mellan enheter.
- Linjer: Linjer representerar attribut till entiteter och entitetsuppsättningar med andra relationstyper.
- Dubbel ellips: Dubbla ellipser representerar Multi-Valued Attribut.
- Dubbel rektangel: Dubbel rektangel representerar en svag enhet.

![Bild-9-PHP](/images/BE/er-modelling.gif)

### Entitet

En Entitet kan vara ett objekt med en fysisk existens – en viss person, bil, hus eller anställd – eller det kan vara ett objekt med en konceptuell existens – ett företag, ett jobb eller en universitetskurs.

Entitetsuppsättning: En Entitet är ett objekt av Entitetstyp och en uppsättning av alla entiteter kallas en entitetsuppsättning. Till exempel är E1 en enhet som har Entity Type Student och uppsättningen av alla studenter kallas Entity Set. I ER-diagrammet representeras Entity Type som:

1. Stark enhet
En stark enhet är en typ av entitet som har ett nyckelattribut. Strong Entity är inte beroende av annan Entity i Schemat. Den har en primärnyckel, som hjälper till att identifiera den unikt, och den representeras av en rektangel. Dessa kallas Strong Entity Types.

2. Svag enhet
En enhetstyp har ett nyckelattribut som unikt identifierar varje entitet i entitetsuppsättningen. Men det finns en enhetstyp för vilken nyckelattribut inte kan definieras. Dessa kallas Weak Entity-typer.

Till exempel kan ett företag lagra information om anhöriga (föräldrar, barn, make) till en anställd. Men de anhöriga kan inte existera utan den anställde. Så beroende kommer att vara en svag enhetstyp och anställd kommer att identifiera enhetstyp för beroende, vilket betyder att det är stark enhetstyp.

En svag enhetstyp representeras av en dubbel rektangel. Deltagandet av svaga enhetstyper är alltid totalt. Relationen mellan den svaga entitetstypen och dess identifierande starka entitetstyp kallas identifierande relation och den representeras av en dubbel diamant.

### Attribut

Attribut är de egenskaper som definierar entitetstypen. Till exempel är Roll_No, Name, DOB, Age, Address och Mobile_No de attribut som definierar enhetstypen Student. I ER-diagrammet representeras attributet av en oval.

1. Nyckelattribut
Attributet som unikt identifierar varje entitet i entitetsuppsättningen kallas nyckelattributet. Till exempel kommer Roll_No att vara unikt för varje elev. I ER-diagrammet representeras nyckelattributet av en oval med underliggande linjer.

2. Sammansatt attribut
Ett attribut som består av många andra attribut kallas ett sammansatt attribut. Till exempel består adressattributet för eleventitetstypen av Gata, Stad, Stat och Land. I ER-diagrammet representeras det sammansatta attributet av en oval som består av ovaler.

3. Attribut med flera värden
Ett attribut som består av mer än ett värde för en given enhet. Till exempel, Phone_No (kan vara mer än ett för en given elev). I ER-diagrammet representeras ett flervärdigt attribut av en dubbel oval.

4. Härlett attribut
Ett attribut som kan härledas från andra attribut av entitetstypen är känt som ett härlett attribut. t.ex.; Ålder (kan härledas från DOB). I ER-diagrammet representeras det härledda attributet av en streckad oval.



## BE 1.8 OAuth i backend

OAuth är en öppen standard för åtkomstdelegering som tillåter användare att ge begränsad åtkomst till sina resurser på en plats till en annan applikation utan att dela sina lösenord.

Den använder auktoriseringstoken istället för autentiseringsuppgifter för att ge applikationer åtkomst till specifika resurser. OAuth etablerar förtroende mellan användaren, klientappen och auktoriseringsservern för att aktivera detta delegerade auktoriseringsflöde på ett säkert sätt.

### Varför använda OAuth

- Ger åtkomst till användarresurser utan att kompromissa med lösenord
- Användare kan ge begränsad åtkomst utan att ge full kontroll
- Decentraliserar autentisering genom tokens
- Används på stora plattformar som Facebook och Google
- Branschstandard för behörighetsdelegering

![Bild-10-PHP](/images/BE/oauthIBackend.png)


### Autentisering vs auktorisering

OAuth 2.0 är byggd för auktoriseringsändamål och inte för autentisering, så det är viktigt att förstå skillnaden mellan dessa två termer mycket tydligt.

Du kan gå vidare och Google efter dessa termer och ta reda på deras definitioner, men efter att ha läst det kanske du fortfarande inte har en klar uppfattning. Så jag kommer att använda det här exemplet för att förstå idén:

Föreställ dig bara att du flyger till Paris med din flickvän för en romantisk semester! När du går genom flygplatsen kommer flygplatsens säkerhets-/immigrationstjänstemän att kontrollera ditt pass och din biljett för att kontrollera om du är den person du säger att du är (kontrollerar din identitet). Detta är autentisering!

Efteråt, när du och din tjej går ombord på planet och om boardingkortet anger att du är en förstaklasspassagerare, kommer privilegierna du får ombord att vara fler än en passagerare i ekonomiklass. Detta är auktorisation!

### OAuth 2.0-terminologi

OK! Låt oss nu börja utforska OAuth2.0 steg för steg! För att du ska förstå resten av artikeln väl är det viktigt för dig att bekanta dig med dessa termer som används i OAuth2.0. Dessa terminologier är oftast namn som ges till redan existerande termer så det är inte så svårt att förstå.

- Resursägare: applikationsanvändaren, som äger den data applikationen vill få
- Klient: Applikationen
- Auktoriseringsserver: System som kan användas för att fråga och bevilja behörigheter
- Resursserver: Systemet som innehåller data
- Auktorisationsbeviljande: Det som bevisar att användaren har gett tillstånd att komma åt data
- Redirect Uri: Platsen som användaren omdirigeras till när tillstånd ges
- Åtkomsttoken: Nyckeln som används för att hämta data från resursservern
- Omfattning: Det som definierar nivån på behörigheter som applikationen har för att manipulera användarnas data

### OAuth-flöde

Om du har gått igenom sekvensen av steg som visas nedan (i valfri mobil- eller webbapplikation).

### Vad är skillnaden mellan en konfidentiell och icke-konfidentiell oAuth2-applikation?

När du väljer oAuth2-protokollet för din applikation kan antingen en konfidentiell eller icke-konfidentiell applikation skapas.

### Konfidentiell

En konfidentiell oAuth2-applikation ska kunna lagra hemligheter säkert och måste därför vara en något kontrollerad miljö, som en server eller ett skript på en lokal maskin.

Både ett klient-id och en klienthemlighet måste tillhandahållas för att kunna identifiera applikationen. I gengäld kan vissa säkerhetsmekanismer ställas in för att vara bekvämare. Refresh-tokens tillåts ha en längre livslängd och kan återanvändas flera gånger.

### Icke-konfidentiell

En icke-konfidentiell oAuth2-applikation är avsedd att representera en applikation i en mindre kontrollerad miljö, som en webbapplikation som körs i en användares webbläsare.

Klient-id är tillräckligt för att identifiera applikationen. Säkerhetsmekanismerna är dock mer strikta för dessa applikationer. Refresh-tokens har en begränsad livslängd och förbrukas vid användning.


## BE 1.9 HTTP-protokollet

HTTP är ett kommunikationsprotokoll som används för att ladda webbsidor på Internet via World Wide Web (WWW). Med hjälp av HTTP kan din dator, smartphone, surfplatta eller annan enhet kommunicera med servrar så att din webbläsare kan läsa in innehållet (content) från olika hemsidor.

HTTP betyder HyperText Transfer Protocol. Vi kan dela upp det i sina beståndsdelar:

- Hypertext: En text som har så kallade hyperlänkar (eller kort och gott ”länkar”) vilka kopplar ihop texten med andra texter. Den vanligaste användningen av hypertexter är på World Wide Web men de används även bland annat på intranät.
- Transfer: Ordet transfer i HTTP indikerar att det handlar om att skicka och ta emot information.
- Protocol: Ett protokoll är en slags överenskommelse mellan två eller fler enheter om hur kommunikationen ska gå till. För att HTTP ska fungera måste det finnas regler och det är det ”protocol” i namnet syftar på.

### När används HTTP?

HTTP används när en webbläsare (HTTP-klient) ska hämta innehåll från en webbserver. Vanligtvis handlar det om HTML-filer och bilder, men det kan även handla om andra typer av filer, till exempel video eller zip-filer.

Hela World Wide Web är uppbyggt av denna typ av nätverkskommunikation (samt det nyare protokollet HTTPS – se nedan). HTTP styr hur data hämtas och skickas mellan hemsidor och servrar runt hela världen. Man kan säga att HTTP fungerar som en slags sändare mellan din dator och den server som har informationen som eftersöks – en slags mellanhand.

### Vem använder HTTP?

Varje gång HTTP används finns det alltid två parter; en klient och en server:

- Klienten är vanligtvis en webbläsare, till exempel Safari, Chrome, Microsoft Edge eller Firefox.
- HTTP-server är mjukvara som finns på en webbserver. Denna webbserver kan i sin tur innehålla en eller flera webbsidor, till exempel genom webbhotell, VPS eller dedikerad server.

### Hur används HTTP?

Så här använder klient och server HTTP steg för steg:

1. Du som användare anger en webbadress i adressfältet eller klickar på en länk i din webbläsare.
2. Klienten (webbläsaren) skickar en HTTP-förfrågan till en HTTP-server.
3. HTTP-servern tar emot förfrågan.
4. Servern bearbetar förfrågan.
5. Därefter skickar servern tillbaks ett HTTP-svar till klienten (webbläsaren).
6. Klienten (webbläsaren) tar emot svaret och visar innehållet på skärmen.

I själva verket fungerar HTTP genom olika slags förfrågningar:

- GET: Klienten ber servern att skicka en viss fil, till exempel en HTML-sida eller en bild. Detta är det vanligaste HTTP-kommandot.
- HEAD: Klienten ber servern att berätta mer om innehållet utan att skicka över det.
- POST: Klienten ber servern att lagra viss information, till exempel i samband med uppladdning av fil eller då ett formulär skickas.
- PUT: Klienten laddar upp en fil på servern. Det kan hända att servern nekar förfrågan.
- DELETE: Klienten säger åt servern att ta bort en fil. Används nästan aldrig.
- TRACE: Klienten ber servern att skicka tillbaks förfrågan. Kan användas för att kontrollera ifall tredje part manipulerat den ursprungliga förfrågan.
- OPTIONS: Visar en lista över serverns samtliga HTTP-kommandon.
- CONNECT: Omvandlar förfrågan till en TCP/IP-tunnel, till exempel för att möjliggöra SSL/HTTPS.
- PATCH: Ett sätt att delvis byta ut innehållet i en fil på servern.

Visste du att det endast är GET och HEAD som samtliga HTTP-servrar måste ha stöd för?

![Bild-11-PHP](/images/BE/http-protokol.jpeg)


### HTTP statuskoder

När en klient gör en förfrågan via HTTP svarar webbservern alltid med en statuskod så att webbläsaren (klienten) vet vad som gäller. HTTP-statuskoderna kan grupperas i fem kategorier:

- 1xx: Servern har mottagit meddelandet.
- 2xx: Servern har mottagit meddelandet och accepterat förfrågan.
- 3xx: Servern dirigerar om förfrågan. Detta kallas även för redirect eller omdirigering.
- 4xx: Fel som har med klienten att göra.
- 5xx: Fel som har med servern att göra.

Varje typ av statuskod specificeras mer i detalj genom ett exakt nummer. Här är några av de vanligaste HTTP-statuskoderna:

- 200: Servern har accepterat HTTP-förfrågan från klienten.
- 301: Servern har permanent dirigerat om förfrågan till en annan adress (URI). Denna kod kan användas till exempel om ett blogginlägg har bytt adress internt på webbplatsen. Den fungerar även för att dirigera om trafik till en annan server.
- 404: Servern kunde inte hitta den sida som klienten efterfrågar.
- 503: Vanligt felmeddelande när servern inte kan svara på förfrågan från klienten. Det kan till exempel inträffa om serverns resurser är otillräckliga för att hantera de förfrågningar som kommer in.

### HTTPS ersätter HTTP

Idag är det allt fler hemsidor som använder HTTPS istället för HTTP. Orsaken är att HTTPS är mycket säkrare än HTTP genom att det använder kryptering av överföringen via SSL. Detta görs för att skydda den information som skickas så att obehörig tredje part inte kan komma åt den. Dessutom har Google sagt att sidor rankar högre med HTTPS än med HTTP. Dina besökares säkerhet och din webbplats chanser att ranka bättre i Google är alltså två bra argument för att använda HTTPS istället för HTTP.
Du känner igen hemsidor som använder HTTPS istället för HTTP genom att det finns ett hänglås i adressfältet i webbläsaren.


## BE 1.10 cURL

[Klient-URL, cURL](https://curl.se/) (cURL, uttalas "curl") är ett kommandoradsverktyg som möjliggör datautbyte mellan en enhet och en server via en terminal. Med hjälp av detta kommandoradsgränssnitt (CLI) anger en användare en server-URL (platsen dit de vill skicka en förfrågan) och de data de vill skicka till den serverns URL.

[API-verktyg](https://owasp.org/www-community/api_security_tools) som Postman och Insomnia tillhandahåller ett interaktivt användargränssnitt (UI) som låter dig göra olika förfrågningar till webbadresser för att ta emot och bearbeta förfrågningar. Kommandot cURL gör samma sak, förutom i din terminal. cURL fungerar på Linux, Mac och Windows.

Kommandot cURL använder URL-överföringsbiblioteket på klientsidan libcURL. Det här biblioteket stöder många olika överföringsprotokoll, inklusive HTTPS, SMTP och FTP. Det låter dig också inkludera cookies, ställa in proxyservrar och lägga till autentiseringsuppgifter när du gör förfrågningar.

Användningsfall av cURL inkluderar att testa API:er, ladda ner data från källor, testa webbplatser och följa omdirigeringar från terminalen.

### Syntax för ett cURL-kommando

Den grundläggande syntaxen för curl-kommandot kan inkludera alternativ och URL:en:

#### cURL [alternativ] [URL]

- alternativ: Jag utnyttjar alternativen när jag vill anpassa beteendet för min förfrågan.
- URL: Den angivna URL:en eller platsen talar om för cURL-kommandot var jag vill komma åt data från eller skicka data.

![Bild-12-PHP](/images/BE/cURL.jpeg)

De två komponenterna i cURL fungerar på olika sätt.

### Vad används libcurl till?

Programvarubiblioteket libcurl tillhandahåller funktioner för överföring av data i datornätverk. Det finns språkbindningar för dussintals populära programmeringsspråk. Dessa gör det enkelt för libcurl-funktioner att användas i en mängd olika program som kommunicerar med servrar.

### Vad används cURL till?

Kommandoradsprogrammet cURL används för webbutveckling. Den enklaste metoden är att ange cURL-kommandon på kommandoraden. Med rätt know-how kan den användas för att testa och felsöka servrar och API:er.

Istället för att skriva kommandon på kommandoraden manuellt, kan de buntas ihop i skript. Detta gör att komplexa operationer kan standardiseras och automatiseras. Detta inkluderar både upp- och nedladdning av data och att programmatiskt fylla i formulär och spegla hela webbplatser.

## BE 1.11 REST

REST, eller REpresentational State Transfer, är en arkitektonisk stil för att tillhandahålla standarder mellan datorsystem på webben, vilket gör det lättare för system att kommunicera med varandra. REST-kompatibla system, ofta kallade RESTful-system, kännetecknas av hur de är tillståndslösa och separerar klientens och serverns bekymmer. Vi kommer att gå in på vad dessa termer betyder och varför de är fördelaktiga egenskaper för tjänster på webben. Var noga uppmärksam: Om du letar efter en karriär inom teknik kan du bli ombedd att definiera vila under en intervju.

### Separation av klient och server

I REST-arkitektonisk stil kan implementeringen av klienten och implementeringen av servern göras oberoende utan att var och en känner till den andra. Detta innebär att koden på klientsidan kan ändras när som helst utan att påverka driften av servern, och koden på serversidan kan ändras utan att påverka driften av klienten.

Så länge varje sida vet vilket format av meddelanden som ska skickas till den andra, kan de hållas modulära och separata. Genom att separera problem med användargränssnittet från problem med datalagring förbättrar vi flexibiliteten i gränssnittet över plattformar och förbättrar skalbarheten genom att förenkla serverkomponenterna. Dessutom tillåter separationen varje komponent förmågan att utvecklas oberoende.

Genom att använda ett REST-gränssnitt träffar olika klienter samma REST-slutpunkter, utför samma åtgärder och får samma svar.

![Bild-13-PHP](/images/BE/Rest.png)

### Statslöshet

System som följer REST-paradigmet är tillståndslösa, vilket innebär att servern inte behöver veta något om vilket tillstånd klienten är i och vice versa. På så sätt kan både servern och klienten förstå alla mottagna meddelanden, även utan att se tidigare meddelanden. Denna begränsning av statslöshet upprätthålls genom användning av resurser, snarare än kommandon. Resurser är webbens substantiv - de beskriver alla objekt, dokument eller saker som du kan behöva lagra eller skicka till andra tjänster.

Eftersom REST-system interagerar genom standardoperationer på resurser, är de inte beroende av implementeringen av gränssnitt.

Dessa begränsningar hjälper RESTful-applikationer att uppnå tillförlitlighet, snabb prestanda och skalbarhet, som komponenter som kan hanteras, uppdateras och återanvändas utan att påverka systemet som helhet, även under driften av systemet.

Nu ska vi utforska hur kommunikationen mellan klienten och servern faktiskt sker när vi implementerar ett RESTful-gränssnitt.

### Kommunikation mellan klient och server

I REST-arkitekturen skickar klienter förfrågningar för att hämta eller modifiera resurser, och servrar skickar svar på dessa förfrågningar. Låt oss ta en titt på de vanliga sätten att göra förfrågningar och skicka svar.

### Göra förfrågningar

REST kräver att en klient gör en begäran till servern för att hämta eller ändra data på servern. En förfrågan består i allmänhet av:

- ett HTTP-verb, som definierar vilken typ av operation som ska utföras
- en rubrik som låter klienten vidarebefordra information om begäran
- en väg till en resurs
- en valfri meddelandetext som innehåller data

### HTTP-verb

Det finns fyra grundläggande HTTP-verb vi använder i förfrågningar om att interagera med resurser i ett REST-system:

- GET — hämta en specifik resurs (efter id) eller en samling resurser
- POST — skapa en ny resurs
- PUT — uppdatera en specifik resurs (efter id)
- DELETE — ta bort en specifik resurs med id

## BE 1.12 XML och andra dataformat

[XML (Extensible Markup Language)](https://support.microsoft.com/sv-se/office/xml-f%C3%B6r-nyb%C3%B6rjare-a87d234d-4c2e-4409-9cbc-45e4eb857d44) är ett märkningsspråk som definierar en uppsättning regler för kodning av dokument i ett format som är både läsbart för människor och maskinläsbart. Den används för att lagra och transportera data och används ofta för att utbyta information mellan olika applikationer. XML-dokument är sammansatta av element som innehåller data och andra element, vilket gör det möjligt att skapa komplexa dokument med en hierarkisk struktur.

### Vad står XML-filformat för?

XML står för eXtensible Markup Language.

![Bild-14-PHP](/images/BE/XML.jpeg)

### XML-filinformation

XML är ett filformat som används för att lagra och transportera data. XML-filer kan användas för att lagra och dela data mellan applikationer, tjänster och system. XML-filer är organiserade i taggar och attribut som möjliggör strukturerad datalagring. XML-filer kan också användas för att lagra text, siffror och bilder. XML-filer används vanligtvis i applikationer som webbtjänster, databaser och programmeringsspråk. XML-filer kan tolkas och manipuleras med hjälp av programmeringsspråk som JavaScript, PHP och Java.

### Programvara, verktyg eller redigerare som används för att skapa XML-fil

XML-filer kan skapas med en mängd olika program, verktyg och redigerare. Populära alternativ inkluderar Notepad, Microsoft Word, XML Notepad, Oxygen XML Editor, Visual Studio Code och Adobe Dreamweaver.

### Programvara, verktyg eller redigerare som används för att öppna XML-fil

XML-filer kan öppnas med vilken textredigerare som helst, som Notepad, Notepad++, TextEdit eller Sublime Text. De kan också öppnas med valfri XML-redigerare, som XMLSpy, Oxygen XML Editor eller Altova XMLSpy.

### Licenstyp för XML-filformat

XML-filformatet är en öppen standard och är inte föremål för någon licens. Det ägs och underhålls av World Wide Web Consortium (W3C).

### Användning av XML-filformat

1. Lagring och transport av data
2. Definiera data på ett självbeskrivande sätt
3. Utveckla plattformsoberoende dokument
4. Skapa och underhålla webbtjänster
5. Skapa dokumenttypsdefinitioner (DTD)
6. Skapa och underhålla XML-scheman
7. Skapa och hantera RSS-flöden
8. Utveckla och underhålla webbsidor i XHTML
9. Lagra data för kontorsproduktivitetsverktyg, till exempel Microsoft Office

### Struktur för ett XML-filtillägg

- Prolog: Prologen är det första elementet i XML-filen och den innehåller information om XML-dokumentet, såsom dess versionsnummer och teckenkodning.

- Dokumentelement: Dokumentelementet är rotelementet i XML-filen. Den innehåller alla andra element och krävs för att XML-dokumentet ska vara välformaterat.

- Element: Element kan innehålla information, såsom text, attribut och andra element.

- Attribut: Attribut är namn/värdepar som anges i ett element.

- Kommentarer: Kommentarer används för att ge ytterligare information om dokumentet eller elementen.

- Bearbetningsinstruktioner: Bearbetningsinstruktioner används för att ge instruktioner till XML-behandlare, till exempel hur man formaterar dokumentet.

- CDATA-sektioner: CDATA-sektioner används för att lagra teckendata som inte bör tolkas av en XML-processor.

### Framtiden för XML-format

XML är ett mångsidigt filformat som har blivit en industristandard för datalagring och utbyte. Det förväntas att XML kommer att fortsätta att användas i framtiden för en mängd olika applikationer, eftersom det är en pålitlig och allmänt accepterad metod för datautbyte. Det är troligt att XML även fortsättningsvis kommer att användas inom webbutveckling, mjukvaruutveckling, datautbyte mellan olika system och som ett sätt att lagra data i ett strukturerat format. Det är också troligt att XML kommer att fortsätta att utvecklas för att anpassas till nya teknologier och applikationer. Till exempel utvecklas nya XML-standarder som XML Schema Definition (XSD) för att göra det lättare att definiera och validera XML-dokument. Dessutom nya teknologier som XQuery, XSLT och XP. 

## BE 1.13 Webbservrar

Webbsidor är en samling data, inklusive bilder, textfiler, hyperlänkar, databasfiler etc., som alla finns på någon dator (även känd som serverutrymme) på Internet. En webbserver är dedikerad programvara som körs på serversidan. När en användare ber sin webbläsare att köra en webbsida, placerar webbservern allt datamaterial ihop till en organiserad webbsida och skickar dem tillbaka till webbläsaren med hjälp av Internet. Därför kan vi dra slutsatsen att: -

En webbserver är en dedikerad dator som ansvarar för att köra webbplatser som sitter ute på dessa datorer någonstans på Internet. De är specialiserade program som cirkulerar webbsidor som kallas av användaren. Det primära syftet med en webbserver är att samla in, bearbeta och tillhandahålla webbsidor till användarna.

Denna interkommunikation av en webbserver med en webbläsare görs med hjälp av ett protokoll som heter HTTP (Hypertext Transfer Protocol). Dessa lagrade webbsidor använder för det mesta statiskt innehåll, som innehåller HTML-dokument, bilder, stilmallar, textfiler, etc. Webbservrar kan dock tjäna både statiskt och dynamiskt innehåll. Webbservrar hjälper också till med e-posttjänster och lagring av filer. Därför använder den också protokollen SMTP (Simple Mail Transfer Protocol) och FTP (File Transfer Protocol) för att stödja respektive tjänster. Webbservrar används huvudsakligen i webbhotell eller hosting av webbplatsens data och för att köra webbaserade applikationer.

Hårdvaran på webbservrarna är ansluten till Internet som hanterar datautbyte inom olika anslutna enheter. Däremot är webbserverns programvara ansvarig för att kontrollera hur en användare kommer åt levererade filer. Webbserverhantering är vanligtvis ett idealiskt exempel på klient/server-modellen. Därför är det obligatoriskt för alla datorer som är värd för webbplatser (oavsett om de har statligt eller dynamiskt webbsideinnehåll) att ha webbserverprogramvara.

XAMPP är en av de mycket använda plattformsoberoende webbservrarna, som hjälper utvecklare att skapa och testa sina program på en lokal webbserver. Den har utvecklats av Apache Friends, och dess ursprungliga källkod kan revideras eller modifieras av publiken. Den består av Apache HTTP Server, MariaDB och tolk för de olika programmeringsspråken som PHP och Perl. Den är tillgänglig på 11 språk och stöds av olika plattformar som IA-32-paketet för Windows och x64-paketet för macOS och Linux.

![Bild-15-PHP](/images/BE/webbserver%20.jpeg)

### Hur fungerar webbservrar?

Termen webbserver kan beteckna serverhårdvara eller servermjukvara, eller i de flesta fall kan både hårdvara och mjukvara samverka.

1. På hårdvarusidan definieras en webbserver som en dator som lagrar programvara och annan webbplats rådata, såsom HTML-filer, bilder, textdokument och JavaScript-filer. Webbservrarnas hårdvara är ansluten till webben och stöder datautbyte med olika enheter anslutna till internet.
2. På mjukvarusidan innehåller en webbserver serverprogramvara som nås via webbplatsens domännamn. Den styr hur webbanvändare får tillgång till webbfilerna och säkerställer leverans av webbplatsinnehåll till slutanvändaren. Webbservern innehåller flera komponenter, inklusive en HTTP-server.

Närhelst någon webbläsare, som Google Chrome, Microsoft Edge eller Firefox, begär en webbsida på en webbserver, kommer webbläsaren att bearbeta begäran vidare med hjälp av HTTP. Vid serveränden, när den tar emot begäran, kommer HTTP-servern att acceptera begäran och omedelbart börja leta efter den begärda informationen och vidarebefordra den tillbaka till webbläsaren via HTTP.

Låt oss ta reda på steg-för-steg-processen för vad som händer när en webbläsare närmar sig webbservern och begär en webbfil eller fil. Följ stegen nedan:

- Först måste alla webbanvändare skriva in webbadressen till webbsidan i adressfältet i din webbläsare.
- Med hjälp av URL:en kommer din webbläsare att hämta IP-adressen till ditt domännamn antingen genom att konvertera URL:en via DNS (Domain Name System) eller genom att leta efter IP:n i cacheminnet. IP-adressen leder din webbläsare till webbservern.
- Efter att ha upprättat anslutningen kommer webbläsaren att begära webbsidan från webbservern med hjälp av en HTTP-förfrågan.
- Så snart webbservern tar emot denna begäran svarar den omedelbart genom att skicka tillbaka den begärda sidan eller filen till webbläsaren HTTP.
- Om webbsidan som begärs av webbläsaren inte finns eller om det uppstår något fel i processen kommer webbservern att returnera ett felmeddelande.
- Om det inte uppstår något fel kommer webbläsaren att visa webbsidan.

![Bild-16-PHP](/images/BE/wserver.jpeg)

### Exempel på användning av webbserver

Webbservrar används mest för:

- skicka och ta emot e-postmeddelanden på Internet genom att använda SMTP (Simple Mail Transfer Protocol);
- hämta förfrågningar för File Transfer Protocol (FTP)-filer; och
- designa, utveckla och publicera webbplatser.

Många webbservrar, även den grundläggande, stöder också skripttekniken på serversidan. Server-side scripting är en webbutvecklingsmetod som används för att använda skript på en webbserver som producerar ett anpassat svar för varje användare. Denna teknik fungerar på servermaskinen och består av en omfattande funktionsuppsättning, inklusive databasåtkomst. Skriptprocessen på serversidan kommer att ha olika skriptspråk som [ASP,](https://dotnet.microsoft.com/en-us/apps/aspnet) [PHP,](https://www.php.net/) [Java,](https://www.java.com/sv/) [JavaScript,](https://www.javascript.com/) [Python,](https://www.python.org/) [ruby](https://www.ruby-lang.org/en/) och många fler. Denna teknik gör det också möjligt för HTML-filerna att skapas dynamiskt.

### Källor:

(OOP i PHP) https://medium.com/@imadevguyanand/php-what-is-oop-413b566f9a94 