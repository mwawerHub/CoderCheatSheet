## Spis Treści
- [Spis Treści](#spis-treści)
- [Programowanie Obiektowe (Object oriented programming - OOP)](#programowanie-obiektowe-object-oriented-programming---oop)
  - [Klasy:](#klasy)
  - [Obiekt](#obiekt)
  - [Atrybuty](#atrybuty)
- [SOLID](#solid)
  - [S: (*Single responsibility principle*)Zasada pojedynczej odpowiedzialności](#s-single-responsibility-principlezasada-pojedynczej-odpowiedzialności)
  - [O: (*Open/closed principle*)Otwarty(na rozszerzanie)/Zamknięty(na modyfikację)](#o-openclosed-principleotwartyna-rozszerzaniezamkniętyna-modyfikację)
  - [L: (*Liskov substitution*)Zasada podstawienia Liskov](#l-liskov-substitutionzasada-podstawienia-liskov)
  - [I: (*Interface segregation*)Segregacja interfejsów](#i-interface-segregationsegregacja-interfejsów)
  - [D: (*Dependency Inversion*) Odwrócenie zależności](#d-dependency-inversion-odwrócenie-zależności)
- [Złożoność obliczeniowa](#złożoność-obliczeniowa)
  - [Złożoność obliczeniowa](#złożoność-obliczeniowa-1)
  - [Złożoność pamięciowa](#złożoność-pamięciowa)
  - [Typy notacji](#typy-notacji)
  - [Typy oszacowań:](#typy-oszacowań)


***

## Programowanie Obiektowe (Object oriented programming - OOP)

Programowanie obiektowe to koncepcja, w której logika programu przedstawiana jest za pomocą klas oraz ich wzajemnych zależności. W tej koncepcji rozszerzamy funkcjonalności aplikacji przez wprowadzanie kolejnych klas przedstawiających daną abstrakcję i odpowiedzialnych za konkretne funkcjonalności. Klasa jest reużywalnym fragmentem kodu, który definiuje stan obiektu poprzez atrybuty oraz jego zachowanie poprzez metody. Obiekty, czyli instancje zdefiniowanych klas posiadają konkretne wartości swoich atrybutów oraz umożliwiają wywołanie zaimplementowanych przez klasę metod.

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

### Atrybuty

Atrybuty są informacjami, które definiują stan obiektu. Przykładowo, klasa *Budynek* może zawierać pola oraz/lub właściwości takie jak wysokość, szerokość, powierzchnia, liczba pięter, rodzaj zadaszenia itp.
Konkretne egzemplarze klasy to na przykład: *Dom* i *DrapaczChmur*. Każdy z tych obiektów będzie miał różne wartości dla zdefiniowanych przez klasę *Budynek* pół i właściwości. Tym samym obiekty będą miały różne atrybuty. 

Źródła:

* ENG: https://www.educative.io/blog/object-oriented-programming
* PL: https://cezarywalenciuk.pl/blog/programing/kurs-obiektowosc-w-c-klasa-i-obiekty-01
* PL/ENG: https://docs.microsoft.com/pl-pl/dotnet/csharp/programming-guide/classes-and-structs/classes
* PL/ENG: https://docs.microsoft.com/pl-pl/dotnet/csharp/tutorials/intro-to-csharp/object-oriented-programming

Other Resources:

* http://www.albahari.com/nutshell/

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

* PL: https://www.p-programowanie.pl/paradygmaty-programowania/zasady-solid
* ENG: https://www.digitalocean.com/community/conceptual_articles/s-o-l-i-d-the-first-five-principles-of-object-oriented-design
* ENG: https://www.educative.io/blog/solid-principles-oop-c-sharp

Pozostałe Materiały:

* https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882

***

## Złożoność obliczeniowa

Powszechnym sposobem przedstawiania złożoności obliczeniowej algorytmu jest oszacowanie.

### Złożoność obliczeniowa

Złożoność obliczeniowa to ilość operacji, jaka niezbędna jest do wykonania algorytmu.

### Złożoność pamięciowa

Złożoność pamięciowa to ilość pamięci, jaką musi wykorzystać algorytm.

### Typy notacji

<b>Notacja dużego O (*Big-O notation*):</b>

Najczęściej spotykany rodzaj oszacowania. Wyrażony jest za pomocą funkcji *g(n)* dla której spełniona jest następująca zależność:<br> *∀n⩾n0:f(n)⩽c∗g(n)*<br>
Od pewnych wartości n (*n0*) jeśli przemnożymy funkcję *g(n)* przez pewną stałą *c*, funkcja *g(n)* będzie zawsze większa od funkcji opisującej ten algorytm. Nazywamy to oszacowaniem z góry.

<b>Notacja Ω:</b>

Jest to odwrotność notacji dużego O. Oszacowanie to opisane jest funkcją, która spełnia właściwość:<br>
*∀n⩾n0:f(n)⩾c∗g(n).*<br>
Od pewnych wartości n (*n0*) jeśli przemnożymy funkcję *g(n)* przez pewną stałą *c*, funkcja *g(n)* będzie zawsze większa od funkcji opisującej ten algorytm. Nazywamy to oszacowaniem z góry.

### Typy oszacowań:

* Ο(*1*) - Złożoność stała. Stała liczba operacji.
* O(*log n*) - Złożoność logarytmiczna. Czas wykonania zależny będzie od wyniku funkcji *log n*. Najczęściej spotykana w algorytmach, które przy każdej iteracji dzielą zbiór danych na pół.
* O(*n*) - Złożoność liniowa. Liczba operacji zależna od ilości danych.
* O(*n2*) - Złożoność kwadratowa. Jest to szczególny przypadek złożoności wielomianowej. Liczba operacji może sięgnąć do wyniku funkcji n^2.

Źródła:

* ENG: https://codility.com/media/train/1-TimeComplexity.pdf
* ENG: https://cs.stackexchange.com/questions/16461/memory-complexity
* PL: http://cpp0x.pl/kursy/Teoria-w-Informatyce/424
* PL: https://www.samouczekprogramisty.pl/podstawy-zlozonosci-obliczeniowej/