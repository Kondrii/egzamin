# Bazy Danych

1. [Relacyjny model danych](#relacyjny-model-danych...) i algebra relacji: atrybuty, dziedziny atrybutów, krotki i relacje; operacje na relacjach
2. [Język SQL](#język-sql) – zapytania, selekcja, sortowanie, grupowanie, funkcje agregujące, podzapytania.
3. [Instrukcje DML](#instrukcje-dml) – usuwanie, aktualizacja i dołączanie danych.
4. [Instrukcje DDL](#instrukcje-ddl) – tworzenie tabel, modyfikacje struktury tabel, usuwanie tabel.
5. Zależności funkcyjne. Aksjomaty Armstronga. Integralność danych (klucze, klucze obce). Opcje propagacji.
6. Postacie normalne: 1NF, 2NF, 3NF, BCNF, 4NF. Normalizacja.
7. Indeksy. Widoki. Procedury składowane. Wyzwalacze.
8. Modelowanie danych: model logiczny (diagram związków encji - ERD) i model relacyjny 
9. Systemy transakcyjne i analityczne - podstawowe różnice
10. Transakcje. Własności ACID. Poziomy izolacji.
11. Administrowanie użytkownikami bazy danych i ochrona danych.

## Relacyjny model danych...

Model organizacji danych bazujący na matematycznej teorii mnogości, w szczególności na pojęciu relacji.

W najprostszym ujęciu w modelu relacyjnym dane grupowane są w relacje, które reprezentowane są przez tablice. Relacje są pewnym zbiorem rekordów o identycznej strukturze wewnętrznie powiązanych za pomocą związków zachodzących pomiędzy danymi. Relacje zgrupowane są w tzw. schematy bazy danych. Relacją może być tabela zawierająca dane teleadresowe pracowników, zaś schemat może zawierać wszystkie dane dotyczące firmy.

### Relacje i reszta pojęć

Relacja - dowolny podzbiór iloczynu kartezjańskiego skończonej liczby zbiorów.

Krotka - struktura danych będąca odzwierciedleniem matematycznej n-ki, tj. uporządkowanego ciągu wartości

Zatem relacja r typu R to nic innego jak skończony zbiór krotek k typu R.

Atrybut - 'pole' encji (np. nazwa, data, wysokość itd...), kolumna krotki

### Algebra relacji

- Selekcja (wybór) 
  - (sigma){{warunek}}(R). 
  - Zgodnie z nazwą wybiera ona z relacji tylko te krotki, dla których jest spełniony podany warunek.
- Rzutowanie (projekcja)
  - (pi){{kolumna_{1},...,kolumna_{n}}}(R)
  - Z relacji wybieramy tylko podane kolumny.
- Złączenie
  - R{\theta}{\Join}S 
  - Podobne do iloczynu kartezjańskiego, ale łączy się ze sobą tylko pary wierszy spełniające podany warunek (theta).
  
## Język SQL

- SQL (Structured Query Language) – język zapytań dla relacyjnych baz danych;
- Język nieproceduralny – użytkownik wyszczególnia operacje co ma być zrobione, a nie w jaki sposób.
- SQL posiada optymalizator, który wybiera optymalną ścieżkę wykonywania zapytania.
- SQL ma kilka dialektów. Są nieznaczne różnice pomiędzy różnymi systemami baz danych.

            
- Selekcja:
  - SELECT * FROM Sells WHERE bar = ‘Tawerna’
- Sortowanie:
  - SELECT * FROM Sells ORDER BY Price (ASCENDING/DESCENDING)
- Agregacja:
  - SUM(Price)
  - COUNT(Price)
  - MAX(Price)
  - AVG(Price)
- Grupowanie:
  - SELECT Bar, AVG(Price) As AvgPrice FROM Sells GROUP BY Bar
- Podzapytania:
  - SELECT Lokalizacja FROM Lokalizacja WHERE Wydzial IN (SELECT Wydzial FROM Pracownik WHERE Nazwisko = 'Zaorski')

## Instrukcje DML

## Instrukcje DDL


