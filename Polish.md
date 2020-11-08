## Spis Treści
- [Spis Treści](#spis-treści)
- [Programowanie Obiektowe (Object oriented programming - OOP)](#programowanie-obiektowe-object-oriented-programming---oop)
  - [Klasy:](#klasy)
  - [Obiekt](#obiekt)
- [SOLID](#solid)
  - [S: (*Single responsibility principle*)Zasada pojedynczej odpowiedzialności](#s-single-responsibility-principlezasada-pojedynczej-odpowiedzialności)
  - [O: (*Open/closed principle*)Otwarty(na rozszerzanie)/Zamknięty(na modyfikację)](#o-openclosed-principleotwartyna-rozszerzaniezamkniętyna-modyfikację)
  - [L: (*Liskov substitution*)Zasada podstawienia Liskov](#l-liskov-substitutionzasada-podstawienia-liskov)
  - [I: (*Interface segregation*)Segregacja interfejsów](#i-interface-segregationsegregacja-interfejsów)
  - [D: (*Dependency Inversion*) Odwrócenie zależności](#d-dependency-inversion-odwrócenie-zależności)


***

## Programowanie Obiektowe (Object oriented programming - OOP)

Programowanie obiektowe to koncepcja, w której logika programu przedstawiana jest za pomocą klas oraz ich wzajemnych zależności. W tej koncepcji rozszerzamy funkcjonalności aplikacji przez wprowadzanie kolejnych klas przedstawiających daną abstrakcję i odpowiedzialnych za konkretne funkcjonalności. Obiekty, czyli instancje zdefiniowanych klas posiadają różne stany oraz implementują metody.

### Klasy:

Klasy to elementy języków obiektowych, które służą do przedstawiania konkretnych abstrakcji lub, innymi słowy, elementów logiki programu. Klasy mogą zawierać w sobie elementy takie jak:

* pola
* konstruktory
* właściwości
* funkcje
* zdarzenia

Klasa jest definicją tego, jak będzie wyglądał obiekt.

### Obiekt
Obiekt to instancja klasy, czyli jej konkretny egzemplarz. Obiekty tworzymy za pomocą słowa kluczowego new:
*var classInstance = new Class();*
Takie wyrażenie powoduje wywołanie konstruktora klasy. Jeżeli konstruktor nie został zaimplementowany własnoręcznie, wywołany zostanie konstruktor domyślny.

Źródła:

PL/ENG: https://docs.microsoft.com/pl-pl/dotnet/csharp/programming-guide/classes-and-structs/classes
PL/ENG: https://docs.microsoft.com/pl-pl/dotnet/csharp/tutorials/intro-to-csharp/object-oriented-programming
PL: https://cezarywalenciuk.pl/blog/programing/kurs-obiektowosc-w-c-klasa-i-obiekty-01


Other Resources:

http://www.albahari.com/nutshell/

***
## SOLID
### S: (*Single responsibility principle*)Zasada pojedynczej odpowiedzialności

Każda klasa powinna być odpowiedzialna za jedną konkretną funkcjonalność. Jeżeli modyfikujesz klasę powinieneś mieć jeden konkretny powód tej zmiany.


### O: (*Open/closed principle*)Otwarty(na rozszerzanie)/Zamknięty(na modyfikację)

Klasy powinny być pisane w taki sposób, aby dodawanie kolejnych funkcjonalności nie wymuszało zmian bezpośrednio w kodzie. Polimorfizm i dziedziczenie to ważne paradygmaty programowania obiektowego, pozwalające na zachowanie zasady otwarty/zamknięty.


### L: (*Liskov substitution*)Zasada podstawienia Liskov

W miejsce klasy bazowej można zawsze użyć dowolnej kalsy pochodnej. Innymi słowy klasa pochodna powinna być substytutem dla klasy bazowej. Wszystkie funkcjonalności klasy bazowej powinny być wykorzystywane w klasie pochdnej. Nazwa zasady pochodzi od nazwiska amerykańskiej programistki Barbary Liskov. 


### I: (*Interface segregation*)Segregacja interfejsów

Projektuj interfejsy tak, aby nie wymuszać na klasie implementującej wprowadzania metod, których nie będzie używać. Twórz interfejsy mniejsze i bardziej skoncentrowane na podobnych metodach. Unikaj w swoich interfejsach deklaracji wielu metod różniących się funkcjonalnościami.


### D: (*Dependency Inversion*) Odwrócenie zależności

Buduj zależności między obiektami na podstawie abstrakcji, a nie konkretnych typów. Zamiast konkretnych typów używaj interfejsów przedstawiających daną abstrakcję. Dzięki temu zmniejszysz powiązania między klasami i umożliwisz wykorzystanie wzorca wstrzykiwania zależności.

Źródła:

PL: https://www.p-programowanie.pl/paradygmaty-programowania/zasady-solid
<br>
ENG: https://www.digitalocean.com/community/conceptual_articles/s-o-l-i-d-the-first-five-principles-of-object-oriented-design

Pozostałe Materiały:

https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882
