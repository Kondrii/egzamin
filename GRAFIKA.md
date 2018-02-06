# Elementy Grafiki Komputerowej

- [Modele barw.](#modele-barw)
- [Metody kompresji obrazów.](#metody-kompresji-obrazów)
- Formaty plików graficznych.
- Rzutowanie.
- Rendering.
- Rasteryzacja, algorytmy rysowania prymitywów graficznych (w szczególności algorytm rysowania odcinka),  antyaliasing. 
- Generowanie sceny przy pomocy “śledzenia promieni”. 
- Algorytmy eliminowania powierzchni zasłoniętych.
- Modele oświetlenia. 
- Materiały, tekstury.


## Modele Barw

- Model barw jest to określony trójwymiarowy system współrzędnych
barw wraz z widzialnym podzbiorem, w którym leżą wszystkie barwy
z określonej gamy barw.
- Model barw ma umożliwiać wygodny wybór barw wewnątrz jakiejś
gamy barw.

#### RGB
- Stanowi najpopularniejszą reprezentację barw.
- Oparty na trójchromatycznej teorii percepcji barw.
- Barwy podstawowe R, G, B są __mieszane addytywnie__, tzn. indywidualne udziały każdej barwy podstawowej są sumowane (mieszane) w celu uzyskania wyniku.

##### Reprezentacja Graficzna

- Bryła modelu RGB jest sześcianem o boku 1. W wierzchołkach tego sześcianu znajdują się barwy podstawowe: 
  - czerwona (1, 0, 0), 
  - zielona (0, 1, 0), 
  - niebieska (0, 0, 1), 
- barwy dopełniające: 
  - żółta (1, 1, 0), 
  - cyjan (0, 1, 1), 
  - magenta (1, 0, 1),
  - biała (1, 1, 1),
  - czarna (0, 0, 0). 
  
- Główna przekątna sześcianu (łącząca wierzchołek barwy czarnej i białej), z równym udziałem barwy podstawowej, reprezentuje poziomy szarości.

![RGB Image](Images/RGB.png)

##### Wady i Zalety

Zalety:
- wygoda i szybkość obliczeń barw,
- odpowiada sposobom generowania barw na takich urządzeniach jak monitor i telewizor.

Wady:
- percepcyjna niejednorodność, tzn. słabe korelacje pomiędzy postrzeganą różnicą dwóch barw a ich euklidesową odległością w sześcianie RGB,
- nieintuicyjność posługiwania się składowymi, R, G, B w określaniu barwy – problem z wizualizacją barwy na podstawie znajomości składowych RGB,
- wrażliwość wartości składowych na zmiany poziomu oświetlenia (iluminacji) sceny,
- jednoczesne operacje wykonywane na wszystkich składowych mogą prowadzić do przekłamania kolorów (np. rozjaśnienie obrazu RGB wymaga ingerencji we wszystkie składowe obrazu).

#### CMY

- Barwy cyjan, magenta i żółta są barwami dopełniającymi odpowiednio dla barw: czerwonej, zielonej, niebieskiej.
- Podstawowe barwy subtraktywne to barwy filtrów używanych w celu odjęcia barwy od barwy światła białego.

##### Reprezentacja Graficzna

- Model CMY jest tak samo reprezentowany w układzie współrzędnych jak model RGB z tą różnicą, że barwa biała (pełne światło) znajduje się w początku układu współrzędnych (a nie barwa czarna - brak światła). Barwy są określane przez to co zostało usunięte albo odjęte od światła białego, a nie przez to co zostało dodane do czerni.

##### Wady i Zalety


## Metody Kompresji Obrazów