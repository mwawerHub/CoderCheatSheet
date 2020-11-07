## Spis Treści
[TOC]

## SOLID
### S: Zasada pojedynczej odpowiedzialności

Każda klasa powinna być odpowiedzialna za jedną konkretną funkcjonalność. Jeżeli modyfikujesz klasę powinieneś mieć jeden konkretny powód tej zmiany.

### O: Otwarty(na rozszerzanie)/Zamknięty(na modyfikację)

Klasy powinny być pisane w taki sposób, aby dodawanie kolejnych funkcjonalności nie wymuszało zmian bezpośrednio w kodzie. Polimorfizm i dziedziczenie to ważne paradygmaty programowania obiektowego, pozwalające na zachowanie zasady otwarty/zamknięty.


### L: Zasada podstawienia Liskov

W miejsce klasy bazowej można zawsze użyć dowolnej kalsy pochodnej. Innymi słowy klasa pochodna powinna być substytutem dla klasy bazowej. Wszystkie funkcjonalności klasy bazowej powinny być wykorzystywane w klasie pochdnej. Nazwa zasady pochodzi od nazwiska amerykańskiej programistki Barbary Liskov. 

### I: Segregacja interfejsów

Projektuj interfejsy tak, aby nie wymuszać na klasie implementującej wprowadzania metod, których nie będzie używać. Twórz interfejsy mniejsze i bardziej skoncentrowane na podobnych metodach. Unikaj w swoich interfejsach deklaracji wielu metod różniących się funkcjonalnościami.

### D: (*Dependency Inversion*) Odwrócenie zależności

Buduj zależności między obiektami na podstawie abstrakcji, a nie konkretnych typów. Zamiast konkretnych typów używaj interfejsów przedstawiających daną abstrakcję. Dzięki temu zmniejszysz powiązania między klasami i umożliwisz wykorzystanie wzorca wstrzykiwania zależności.

## Źródła:

PL: https://www.p-programowanie.pl/paradygmaty-programowania/zasady-solid
ENG: https://www.digitalocean.com/community/conceptual_articles/s-o-l-i-d-the-first-five-principles-of-object-oriented-design

## Pozostałe Materiały:

https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882
