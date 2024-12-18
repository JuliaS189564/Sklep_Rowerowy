# Sklep_Rowerowy
Analiza danych dot.Sklepu Rowerowego 

Tytuł: Sklep Rowerowy
Autorzy: Julia Sulka, Julia Urban, Barbara Michalska
Opis projektu:
Projekt ma na celu eksplorację, czyszczenie, analizę i wizualizację danych zebranych od 1000 nabywców rowerów. Dane te zawierają szczegółowe informacje o użytkownikach, w tym dane demograficzne, takie jak wiek, dochód, stan cywilny, wykształcenie i inne zmienne. Celem jest zrozumienie, jakie czynniki mogą wpływać na decyzję o zakupie roweru i wykorzystanie algorytmów uczenia maszynowego do predykcji tej decyzji.

1. Zestaw Danych:
Zestaw danych zawiera informacje na temat 1000 nabywców rowerów. Zostały one zgromadzone, aby analizować, które zmienne mają wpływ na decyzję o zakupie roweru. Zawiera również dane brakujące (NA), które zostały poddane odpowiedniemu czyszczeniu i imputacji.

Zmienne:

ID – unikalny identyfikator nabywcy
Marital Status – status cywilny (np. „Married”/„Single”)
Gender – płeć (np. „Male”/„Female”)
Income – dochód
Children – liczba dzieci
Education – poziom wykształcenia (np. „Bachelors”, „Partial High School”)
Occupation – zawód (np. „Clerical”, „Professional”)
Home Owner – posiadanie domu (tak/nie)
Cars – liczba posiadanych samochodów
Commute Distance – odległość do pracy (np. „0-1 Miles”, „5-10 Miles”)
Region – region geograficzny (np. „Europe”, „Pacific”, „North America”)
Age – wiek
Purchased Bike – zakup roweru (tak/nie) – zmienna wyjściowa


2. Cel Projektu:
Celem projektu jest:

Eksploracja danych – identyfikacja wzorców, analizowanie związku pomiędzy różnymi zmiennymi.
Czyszczenie danych – usuwanie lub imputacja brakujących wartości (NA).
Analiza i wizualizacja – tworzenie wykresów i analiz statystycznych w celu lepszego zrozumienia danych.
Modelowanie predykcyjne – budowanie modeli predykcyjnych do przewidywania decyzji o zakupie roweru.


3. Proces Analizy Danych:
Projekt wykorzystuje następujące techniki:

Czyszczenie danych – usuwanie i imputacja brakujących wartości przy pomocy różnych metod, takich jak hotdeck (uzupełnianie braków).
Wizualizacja brakujących danych – użycie wykresów (np. vis_miss, gg_miss_upset,ggplot) do wizualizacji rozkładu brakujących danych.
Tworzenie reguł edytowania danych – stosowanie reguł do oceny poprawności danych, np. „dochód > 0”, „wiek <= 120”.
Analiza statystyczna – ocena zgodności danych z założonymi regułami oraz analiza naruszeń reguł.

4. Użyte Technologie i Biblioteki:
Projekt korzysta z następujących technologii i bibliotek:

R – język programowania i środowisko do analizy danych.
Biblioteki R:
readr – do wczytywania plików CSV.
naniar – do analizy brakujących danych.
ggplot2 – do tworzenia wykresów.
dlookr – do imputacji brakujących danych.
editrules – do definiowania reguł dla danych.
validate – do oceny poprawności danych na podstawie reguł.

5. Instrukcja Uruchamiania:
Załaduj dane: Użyj funkcji read_csv do wczytania danych z pliku sklep_rowerowy.csv.

Eksploracja danych:

Zbadaj strukturę danych przy pomocy head(data), aby sprawdzić pierwsze kilka wierszy.
Zidentyfikuj brakujące dane używając funkcji n_miss(data) oraz wizualizując je za pomocą vis_miss.
Czyszczenie danych:

Uzupełnij brakujące dane za pomocą funkcji hotdeck z pakietu dlookr.
Analiza danych:

Przeprowadź analizę naruszeń reguł edytowania danych (np. „Marital.Status %in% c('Married', 'Single')”).
Zastosuj reguły edytowania przy użyciu pakietu editrules i sprawdź, czy dane spełniają te reguły.
Wizualizacja wyników:

Twórz wykresy pokazujące brakujące dane, relacje pomiędzy zmiennymi i inne interesujące zależności w danych.