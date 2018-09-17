# Specyfikacja programu Neuro-Predictor

### 1. Wprowadzenie

Niniejszy dokument zawiera opis specyfikacji programu Neuro-Predictor, którego zadaniem będzie zbudowanie modelu pewnego zjawiska w oparciu o obserwowane zmiany w czasie pewnych mierzalnych wielkości opisujących ten proces. Do programu zaimplementowana zostanie architektura w postaci sztucznej sieci neuronowej, dzięki której system będzie uczył się schematów realizowanych przez dostarczony zbiór danych i na tej postawie będzie przewidywał przyszłe wartości zmiennych, które mogą dołączyć do zbioru.

### 2. Cel

Celem pracy jest zaprojektowanie systemu bazującego na architekturze rekurencyjnej sieci neuronowej, zdolnego do nauki na dostarczonym zbiorze danych poprzez przetwarzanie sygnałów w kolejnych warstwach elementów, zwanych sztucznymi neuronami. Zastosowania programu mogą być wszechstronne, ograniczone jednak do predykcji przyszłych wartości tylko takich zmiennych, które charakteryzuje pewien określony wzorzec.Ze względu na to program można wykorzystać do wszelkiego rodzaju prognoz, szczególnie finansowych szeregów czasowych (prognozy cen sprzedaży, prognozy giełdowe). Przykładowym zastosowaniem programu może być prognoza cen akcji w oparciu o dane historyczne pochodzące z serwisu Yahoo! Finance.

### 3. Wersja aplikacji 

Program zostanie przygotowany w formie skrytpu napisanego w języku programowania Python. Aplikacja będzie kompatybilna ze środowiskami Widows, Linux oraz MacOS wyposażnymi w iterpreter języka Python.

### 4. Metoda estymacji

Program będzie działał w oparciu o architekturę rekurencyjnej sieci neuronowej (recurrent neural network- RNN)czyli takiej sztucznej sieci neuronów, która tworzy graf cykliczny, dzięki czemu istnieją w nim sprzężenia zwrotne między wejściem a wyjściem a zmiana stanu jednego neuronu przenosi się na całą sieć.
Zbiorem testowym, na podstawie którego system będzie uczył się szacowania ceny giełdowej będą dane pobrane z serwisu Yahoo! Finance w formacie .csv przedstawiające ceny otwarcia akcji firmy Google w kolejnych dniach w latach 2012 - 2016.
System złożony będzie z wydzielonych warstw:
-	Warstwa wejściowa - przechowywać będzie dane dostarczone do sieci.
-	Warstwa ukryta - jej celem będzie przetwarzanie informacji.
-	Warstwa wyjściowa - przechowywać będzie wyniki sieci.
Poprzez naukę systemu rozumie się dostosowywanie wag poszczególnych synaps w sieci, w taki sposób aby minimalizować błędy popełniane przez sieć metodami gradientowymi optymalizacji statycznej, co pozwoli na otrzymanie wyników podanych w przykładach. 

### 5. Interfejs oraz wymagania użytkownika 

Ze względu na charakter działania programu, którego zadaniem jest przede wszystkim analiza dostarczonych danych oraz prezentacja wyników, aplikacja zostanie wyposażona w bardzo ograniczony interfejs graficzny. Będzie się na niego składać główne okno programu umożliwiające wczytanie pliku zawierającego niezbędne dane do „trenowania” systemu oraz podgląd tabeli z danymi. Po zaakceptowaniu wprowadzonych danych, wyniki będą prezentowane w formie wykresu na dodatkowym panelu z opcją zapisania ich do plików tekstowych (dane) oraz rozszerzeń .jpg, .pdf (wykresy).

### 6. Licencja 

Program zostanie udostępniony naprawach licencji GNU General Public License. Oznacza to, że użytkownik będzie miał prawo do uruchamiania programu w dowolnym celu, dostosowywania programu do swoich potrzeb, rozpowszechniania niezmodyfikowanej kopii programu a także do udoskonalania i publicznego rozpowszechniania własnych rozszerzeń w społeczności.
