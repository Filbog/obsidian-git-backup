04-10-2026
# prowadzący - Tomasz Tyksinski
- tomasz.tyksinski@cdv.pl
- dyzury: wtorki 9:30-11:00 (online) po wczesniejszym potwierdzeniu, indywidualnie po wczesjniejszym ustaleniu temrinu
# zaliczenie - test
- nie na ocene
- robimy na blackboard
- dlugosc: 5-10min
## wiodacy jezyk programowania - C/C++

# PP1
## pojecia
### informatyka - nauka zajmująca się przetwarzaniem informacji
### algorytm - jakis proces gdzie mamy dane wejsciowe i wyjsciowe
- sluzy do rozwiazywania problemu;
- schemat, przepis jak rozwiazać zadanie wg określonych reguł
- Essentialy: **wejście - sposób - wyjście**
- wiele definicji; nie ma jednej, absolutej definicji algorytmu
### jak ulozyc algorytm do rozwiązania problemu? step by step
1. Scisłe sformułowania zadania
2. zdefiniowanie danych wejściowych
3. określenie rozwiązania problemu; co chcielibyśmy, żeby było wynikiem
4. poszukiwanie metody rozwiązania, algorytmu - rozkminy
5. zapisanie algorytmu w formie opisowej
6. przelozenie opisu na schemat blokowy
7. wytworzenie konkretnej listy krokow algorytmu; pseudokod
8. zapisanie algorytmu w wybranym jezyku programowania
9. sprawdzanie poprawności otrzymanego wyniku dla różnych danych wejściowych; testowanie
10. optymalizacja - klejenie blędów, poprawanie pod edge case'y, poszukiwanie lepszych rozwiązan
### poboczne pojecia
#### bit
- najmniejsza jednostka wykorzystywana w informatyce; 0 lub 1
- jeden bit jest w stanie przekazac 2 informacje, 2 bity - 4 informacje; z dolozeniem kazdego bitu liczba informacji zwieksza sie dwukrotnie, czyli bit to 8 bajtow obok siebie, wiec $2^8$ informacji
#### bajt - 8 bitow
#### schemat blokowy 
- skrzynka rozpoczynająca i konczaca, strzałki
- skrzynka łącznikowa
#### kod maszynowy
- nawet jezyk programowania jest tlumaczony wlasnie na jezyk maszynowy - **kompilacja**. Wtedy zazwyczaj przechodzi przez **język pośredni**
#### program - zapis algorytmu w wybranym jezyku programowania

# AiSD1
Za najstarszy algorytm uznaje się sposób na obliczenie NWD dwóch liczb naturalnych **a** i **b** przez Euklidesa


# PP2 (18-10)
## Budowa programu c.d.
- w C, C++ zawsze musi byc funkcja main
	- Program musi też zwracać jakiś wynik; return konczy też działanie funkcji (w main konczy program)
	- **#include** \<nazwa biblioteki> do importu bibliotek
- Zmienne - sluzą do przechowywania i przetwarzania danych
	- **Deklaracja zmiennej** - alokujemy w pamięci jakiś obszar dla zmiennej; w zależności od typu, oczywiście tez wartości
		- W C, C++ mamy dużo kontroli w kontekście zarządzania pamięcią. Np. Możemy „zmniejszyć” rozmiar danej typu *int* za pomocą keyworda *short*, „wydłużyć” za pomocą *long*
	- Przechowywane w pamięci
		- Języki C, C++ przy samej deklaracji zmiennej (bez przypisanai wartości) nie „czyszczą” przypisanego im obszaru - jak np. Napiszemy „int x;” to jeśli próbowalibyśmy ją wywołać, mogłyby jakieś dziwne nieprzewidziane wyniki
- #### kodowanie - przypisanie jakieś wartości pewnego znaku liczbowego
	- np. Oznaczanie znaków, liter; ASCII
- C/C++ są **case-sensitive**

# AiSD2 18-10
### rekurencja
- funkcja wywoluje sama siebie do pewnego momentu, za każdym razem ze zmienioną wartością
- Musi być warunek który ją zatrzyma w pewnym momencie; jeśli nie to zapcha się pamięć, **stack overflow**
#### rekurencja VS pętla
- zazwyczaj „lepsze” są pętle, ale w niektórych przypadkach potrafią być bardzo nieczytelne, bloated. Np przy jakichś grafach, drzewach
### podstawowe paradygmaty tworzenia algorytmów komputerowych
1. Divide and conquer - dzielimy problem na kilka mniejszych a te znowu dzielimy aż ich rozwiązania taną się oczywiste
2. Programowanie dynamiczne - problem dzielimy na kilka i hierarchizujemy je względem ważności; 
3. Zachłanne - wybieramy arbitralnie jedną metodę ktora jest najbardziej obiecująca
4. Programowanie liniowe
5. Poszukiwanie i wyliczanie
6. Algorytm probabilistyczny
7. Heurystyka - jak nic praktycznie nie wiemy i próbujemy znaleźć coś najbardziej podobnego, i na tej zasadzie kombinujemy
### techniki implementacji algorytmów
1. Proceduralność - algo dzielimy na szereg podstawowych procedur; wiele algorytmów współdzieli biblioteki takich standardowych procedur, z których są one wywoływane bez potrzeby
2. Praca sekwencyjna - jednowątkoa; wyoknywanie kolejnych procedur algorytmu
3. Praca wielowątkowa - procedury wykonywanie sekwencyjnie, lecz kolejność ich wykonania jest trudna/niemożliwa do przewidzenia dla programisty
4. Praca równoległa - wiele procedur wykonywanych jest w tym samym czasie, wymieniają się one danymi
5. Rekurencja - procedura/funkcja wywołuje sama siebie aż do uzyskania wyniku lub błędu
6. obiektowość - procedury i dane łączymy w pewne klasy reprezentujace najwaniejsze elementy algorytmu oraz stan wewnętrzny wykonującego je urządzenia

### formy prezentacji algorytmu
- opis słowny (język naturalny)
- Pseudokod - taki nieformalny język służący do przedstawienia logiki
- Język programowanie
- Notacje graficzne:
	- Schematy blokowe
	- Drzewa decyzyjne - jak z memów, że w zależności od opcji strzalki kierują nas w konkretne dymki
	- Diagramy UML - graficzny model, zwłaszcza do pełnoprawnych projektów. Jak backend laczy się z frontendem, co może robić uzytkownik itp
### Hashtags:
#cdv #education #coding 

### References (source material, similar notes):
