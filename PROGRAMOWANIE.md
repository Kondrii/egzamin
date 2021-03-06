# Programowanie

1. [Budowa języków programowania i ich podział.](#budowa-języków-programowania)
2. [Podstawowe typy danych, typy podzielne, literały.](#podstawowe-typy-danych)
3. [Metoda siłowa. Zgadnij i sprawdź. Przeszukiwanie wyczerpujące.](#metoda-siłowa)
4. [Modularyzacja programu: podprogramy. Funkcje oraz procedury. Deklaracja i definicja funkcji. Zasady wywoływania funkcji. Komunikacja z innymi podprogramami.](#modularyzacja)
5. [Dekompozycja i abstrakcja. Parametry formalne i argumenty. Parametry domyślne.](#dekompozycja)
6. [Zasięg i jego funkcja. Zmienne lokalne i globalne.](#zasięg) 
7. [Stos i jego funkcja.](#stos)
8. [Programowanie defensywne. Wyjątki.](#programowanie-defensywne)
10. [Testowanie oprogramowania. Testy strukturalne i funkcjonalne.](#testowanie)
11. [Błędy i ich podział.](#błędy)
12. [Dziel i zwyciężaj. Rekurencja. Przypadek podstawowy i część indukcyjna. Przykłady.](#dziel-i-zwyciężaj)
13. [Programowanie zorientowane obiektowo. Obiekty i ich identyfikatory, typy, tożsamość, stan. Instancje. Funkcje klas i metody instancji. Klasy abstrakcyjne.](#programowanie-zorientowane-obiektowo)
14. [Dziedziczenie. Hierarchia klas, klasy bazowe i pochodne.](#dziedziczenie) 
15. [Debugowanie, usuwanie błędów.](#debugowanie)
16. [Polimorfizm. Przeciążanie operatorów. Rzutowanie.](#polimorfizm)

## Budowa języków programowania

Budowa:
- Składnia - Aby dany ciąg znaków mógł być rozpoznany jako program napisany w danym języku, musi spełniać pewne reguły, zwane składnią
- Semantyka - definiuje precyzyjnie znaczenie poszczególnych symboli oraz ich funkcję w programie
- Typy danych
- Biblioteki standardowe

Podział:
- programowanie proceduralne
- programowanie strukturalne
- programowanie funkcyjne
- programowanie imperatywne
- programowanie obiektowe
- programowanie deklaratywne - W przeciwieństwie do programów napisanych imperatywnie, programista opisuje warunki, jakie musi spełniać końcowe rozwiązanie (co chcemy osiągnąć), a nie szczegółową sekwencję kroków, które do niego prowadzą
- programowanie modularne

## Podstawowe typy danych

![LEL](./Images/lel.jpeg)

## Metoda siłowa

__Wyszukiwanie wyczerpujące (ang. exhaustive search), metoda siłowa (ang. brute force)__ - metoda polegająca na analizie wszystkich potencjalnych rozwiązań zadania w celu wybrania tego, które spełnia warunki zadania

## Modularyzacja

![LEL](./Images/lel.jpeg)

## Dekompozycja

__Abstrakcja__ - pewnego rodzaju uproszczenie rozpatrywanego problemu, polegające na ograniczeniu zakresu cech manipulowanych obiektów wyłącznie do cech kluczowych dla algorytmu, a jednocześnie niezależnych od implementacji

__Dekompozycja__ - rozkład problemu na mniejsze pod-problemy

__Parametry__ - są nazwami obiektów przekazywanych do funkcji wraz z podaniem ich typów.

__Argumenty__ - konkretne zmienne lub wartości przekazywane do funkcji 

## Zasięg

![LEL](./Images/lel.jpeg)

## Stos

![LEL](./Images/lel.jpeg)

## Programowanie defensywne

![LEL](./Images/lel.jpeg)

## Testowanie

IMO:

![LEL](./Images/lel.jpeg)

Ale jak ktoś potrzebuje:

__Testy strukturalne__ - znane są także jako testy białej lub szklanej skrzynki. Polegają na testowaniu programu poprzez podawanie na wejściu takich danych, aby program przeszedł przez każdą zaimplementowaną ścieżkę

__Testy funkcjonalne__ - znane są także jako testy czarnej skrzynki, ponieważ osoba testująca nie ma dostępu do informacji na temat budowy programu, który testuje

## Błędy

__Błędy składniowe__ - nie pozwalają na kompilację programu, jak np. literówka w wywołaniu zmiennej. Są one najczęściej dość łatwe do usunięcia, zazwyczaj wynikają z drobnych pomyłek programisty.

__Błędy semantyczne__ - część błędów semantycznych można wychwycić już w momencie kompilacji, np. próbę odwołania się do nieistniejącej funkcji, lecz inne mogą ujawnić się dopiero w trakcie wykonywania.

__Błędy logiczne__

## Dziel i zwyciężaj

__Dziel i zwyciężaj__ - wyszukiwanie binarne, mergesort, quicksort
__Rekurencja__ - algorytm Euklidesa, ciąg Fibonacciego
__Przypadek podstawowy__ - Przy redukcji problemu  wymagany  jest wyraźnie  określony  warunek  zakończenia
__Część indukcyjna__ - Wykonywanie kolejnych kroków (kroki indukcyjne)

## Programowanie zorientowane obiektowo

![LEL](./Images/lel.jpeg)

## Dziedziczenie

![LEL](./Images/lel.jpeg)

## Debugowanie

![LEL](./Images/lel.jpeg)

## Polimorfizm

__Polimorfizm__ - cecha dzięki której jeden interfejs może być stosowany do wykonania różnych zadań 

__Przeciążanie operatorów__ - nadanie nowej funkcji operatorom takim jak + - / itd.

__Rzutowanie__ - konwersja typu, konstrukcja programistyczna umożliwiająca traktowanie danej pewnego, konkretnego typu, jak daną innego typu
