# Stopy i ławy

[Wideo](#wideo) | [Instrukcja](#instrukcja) | [Moduły do ABC](https://pkpkbud.github.io/)

Moduł do szybkiego projektowania fundamentów bezpośrednich zgodnie z Eurokodami w
programach **ABC** firmy [PRO-SOFT](https://www.pro-soft.gliwice.pl/). Przed zakupem
działa w trybie DEMO, gdzie nie można zmieniać parametrów podłoża.

<script>
  if (["#zakup", "#instalacja", "#kontakt"].includes(location.hash))
    location.replace("https://pkpkbud.github.io/" + location.hash);
</script>

## Wideo

<iframe width="560" height="315" src="https://www.youtube.com/embed/T7rEyB1jpJs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/MAA1BrUQ1LE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/dykUG6P5lk0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Instrukcja

Podczas korzystania z modułu, można uzyskać wskazówki dotyczące danej funkcji po
najechaniu na opis kursorem myszy. Jednostki, w jakich podane są wartości są po
lewej stronie każdego pola. Wartości można zmieniać, wpisując na klawiaturze i
zatwierdzając klawiszem `Enter`, klikając na znaki `góra`-`dół` po prawej stronie
pola lub wciskając klawisze strzałek `↑`-`↓` na klawiaturze.

### Uruchomienie

Moduł można uruchomić samodzielnie w trybie kalkulatora. W tym celu należy uruchomić
skrót z pulpitu albo odpowiedni plik `stopa.exe` lub `lawa.exe` z lokalizacji instalacji
(np. *C:\ABC6\EXE*). **Pierwsze uruchomienie należy wykonać z poziomu programu ABC.**

![image](https://github.com/user-attachments/assets/2f8600b2-e011-4c78-8b2b-64817a7e84dd)

W każdym typie zadania, w którym wprowadzono podpory węzłowe lub typu `Słup` można
zaprojektować stopę fundamentową. W programach **ABC** dla podpór liniowych lub typu
`Ściana` oraz prętów na podłożu można zaprojektować ławę fundamentową.
W wynikach zadania w menu `Wymiar` dostępne są opcje `Projektowanie stopy` oraz
`Projektowanie ławy`. W przypadku, gdy ta możliwość nie jest dostępna należy
zaktualizować program **ABC** do wersji 6.23, włączyć pełny zakres menu w **ABC**
przyciskiem "M" lub wybrać z menu opcję `Pokaż → Wybór wymiarowania`.

![image](https://github.com/pkpkbud/fundamenty/assets/55211992/775bd5e1-657d-4b8f-a272-fb3ec5c52b8e)

### Obciążenia

Po uruchomieniu pokaże się pytanie o obciążenia. W przypadku wariantu będzie można
zmienić mnożnik obciążenia, podpowiadany z opisu obciążeń przyjmowanych do obwiedni.
Obwiednia generalnie będzie obliczana jako `Automat EN`, chyba, że są zdefiniowane
własne kombinacje wg PN-EN, to wtedy będzie można je wybrać. Jeśli projektowanie
fundamentów było poprzedzone wymiarowaniem żelbetu, to nie będzie pytania o obciążenia,
ponieważ fundamenty będą projektowane na te same obciążenia co użyte w żelbecie. Jest
również możliwość dodania ciężaru własnego ścian i słupów do obciążeń po włączeniu
opcji `Dodaj ciężar ściany`. Przycisk `Usuń` usuwa wcześniej zadane miejsca.

![image](https://github.com/user-attachments/assets/5f267596-8f0e-45a1-aec4-1f9389700013)

### Wybór miejsca

Po zatwierdzeniu obciążeń plansza zostanie zamknięta i pokaże się rysunek modelu. W
przypadku opcji `Projektowanie stopy` pojawią się podpory skupione (słupy) z zaznaczonym
miejscem o największej reakcji pionowej, należy wybrać projektowane miejsce. W przypadku
opcji `Projektowanie ławy` pojawią się podpory liniowe typu `Ściana`, należy wybrać dwa
skrajne węzły projektowanego miejsca. Istnieje możliwość dodania długości ściany.
Jej dodanie rozkłada obciążenie na większej długości.

### Podłoże

![Okno Podłoże](podloze.png)

W oknie można zdefiniować `Głębokość posadowienia`, którą należy liczyć od najniższego
poziomu naziomu. Pole zmienia kolor na pomarańczowy, gdy głębokość jest mniejsza niż
zalecane 0,5 m (p. 2.2.2 normy *PN-81 B-03020*), bo takie zagłębienie wymaga uzasadnienia.
W celu uwzględnienia sił wyporu spowodowanych wodą gruntową należy określić
`Poziom wody gruntowej`.

Opcja `Sprawdź podłoże na innej głębokości` służy do uwzględnienia sytuacji, gdy
warstwa o niższych parametrach geotechnicznych zalega na głębokości mniejszej niż 2B
poniżej poziomu posadowienia fundamentu według metody fundamentu zastępczego normy
*PN-81 B-03020*. Należy zdefiniować, na jakiej głębokości od naziomu znajduje się strop
warstwy gruntu oraz jaki jest rodzaj gruntu bezpośrednio pod podstawą fundamentu.
Parametr ten służy do ustalenia zasięgu poszerzania podstawy fundamentu zastępczego.
Po zatwierdzeniu przyciskiem `OK` sprawdzenie podłoża odbywa się na nowej głębokości.
W celu sprawdzenia kolejnej warstwy gruntu, można skopiować listę z wynikami
`Do schowka` lub `Do Worda` i wprowadzić nową głębokość oraz parametry geotechniczne.

![Rysunek ławy ze sprawdzeniem podłoża na innej głębokości](rysunek_lawa.png)

W celu definicji podłoża należy podać charakterystyczne wartości parametrów
geotechnicznych na podstawie badań geologicznych gruntu lub z normowych tablic. Przycisk
`Metoda B normy PN-81 B-03020` umożliwia wprowadzenie parametrów geotechnicznych na
podstawie zależności korelacyjnych z normy `PN-81 B-03020` oraz zalecane dopuszczalne
naprężenia według tabeli 12-2 książki *Zarys geotechniki* Zenona Wiłuna (2013 wyd. 10).
Po wyborze z menu rodzaju gruntu należy podać jego charakterystyczny parametr jak:
stopień zagęszczenia i wilgotność (grunty niespoiste) lub stopień plastyczności
i typ konsolidacji (grunty spoiste). Po zatwierdzeniu przyciskiem `Zastosuj` wartości
parametrów w oknie `Podłoże` są aktualizowane oraz blokowane. W celu ich zmiany należy
odznaczyć opcję `Metoda B normy PN-81 B-03020`. Dodatkowo, w celach informacyjnych,
podawane są współczynnik Poissona, moduł odkształcenia pierwotnego `E0` oraz wskaźnik
skonsolidowania gruntu `β` według tablicy 3 normy.

![Okno Metoda B normy PN-81 B-03020](metoda_b.png)

W celu sprawdzenia warunku naprężeń krawędziowych należy włączyć i podać
`Dopuszczalne naprężenia`. W celu sprawdzenia osiadania należy włączyć
`Sprawdź osiadanie` i podać `M0`, edometryczny moduł ściśliwości pierwotnej gruntu.
`Graniczna wartość osiadania` oraz `Graniczna wartość różnicy osiadań`
definiowana jest w oknie `Ustawienia`.

Przycisk `Budowla wysoka lub hala z suwnicą` zmienia parametry wymiarowania nie
dopuszczając, aby siła wypadkowa wychodziła poza rdzeń podstawy oraz aby nie było za
dużej dysproporcji pomiędzy minimalnymi i maksymalnymi naprężeniami krawędziowymi.

### Projektowanie

Po wprowadzeniu danych na pierwszej planszy można przyciskiem `OK` przejść do planszy
głównej modułu. Na niej przeprowadzane jest całe projektowanie. Składa się z opisanych
poniżej elementów.

![Plansza projektowania stopy](plansza.png)

**Ramka z danymi po lewej stronie**, gdzie podobnie jak na pierwszej planszy należy
podać wartości, tym razem dotyczące przyjętych wymiarów, materiałów, otuliny oraz
zbrojenia. Kierunek X i Y jest zgodny z układem osi przyjętym w programach **ABC**.
`Opis` można dowolnie modyfikować, domyślnie wpisany jest numer węzła. Zaznaczenie opcji
`Okrągła` pozwala na projektowanie niezbrojonych, pionowo obciążonych stóp o podstawie
kołowej o promieniu R według normy *PN-81 B-03020*, gdzie przyjmuje się B = L = 1,77 R.
Przycisk `Obróć` umożliwia obracanie stopy o 90 stopni, podmieniana jest wartość X z Y.
`Wysokość` fundamentu to wartość od poziomu posadowienia (głębokości wykopu) w górę.
Przycisk `Centruj` umożliwia zerowanie mimośrodów, czyli centralne ustawienie środka
słupa względem środka fundamentu. Ponowne wciśnięcie przywraca wartości przed centrowaniem.
W celu policzenia ławy jako fundamentu pasmowego o nieskończonej długości należy
odznaczyć opcję `Długość`. Wymiary słupa, ściany oraz dane fundamentu są pobierane
z opisu podpory z wyjątkiem słupów okrągłych. Aby je zadać, należy zaznaczyć opcję
`Okrągły`. W innych przypadkach są przyjmowane wartości domyślne.

![image](https://github.com/pkpkbud/fundamenty/assets/55211992/7c280982-7f00-4da0-ae3f-20141f9460d6)

**Ramka z wynikami u dołu**, która aktualizuje się po zmianie wartości parametrów
lub po naciśnięciu przycisku `Oblicz`. Każda linijka zawiera opis sprawdzanego warunku,
wzór oraz stopień wytężenia podany w procentach. Stopień wytężenia większy niż 999%
podawany jest jako `> 999%`. W przypadku, gdy któryś warunek nie jest spełniony, kolor
tekstu zmienia się na czerwony. Nie są również pokazywane sprawdzenia wyników o zerowym
wytężeniu. Zachowanie to można zmienić w oknie `Ustawienia`. W przypadku wymiarowania na
obwiednię sił, na końcu każdego wzoru w nawiasie kwadratowym podany jest decydujący
przypadek. Po najechaniu na niego kursorem myszy wyświetlone zostaną wartości sił pobrane
z programu **ABC**. Nazwa przypadku oznacza wiodące obciążenie dla warunku.

Sprawdzane są następujące warunki nośności podłoża zgodnie z normą *PN-EN 1997-1*:
- Opór pionowy podłoża (wyparcie) obliczony metodą analityczną według załącznika D.
- Nośność na przesunięcie poziome (poślizg) obliczona zgodnie z punktem 6.5.3. Gdy pod
podstawą powstaje szczelina, a podłoże jest spoiste lub pracuje bez odpływu, opór
ogranicza się do 0,4 Vd według punktu 6.5.3(12)P.
- Sprawdzenie, czy siła wypadkowa znajduje się w rdzeniu podstawy. W przypadku
większych wartości mimośrodów (> 1/6) pojawiają się naprężenia rozciągające w kontakcie
grunt-fundament, czego konsekwencją jest powstanie szczeliny, tzw. odrywanie. Można
dopuścić przyciskiem `ODRYWANIE` w przypadku, gdy obiekt budowlany nie ma wysoko
umiejscowionego środka ciężkości. Zaleca się, aby były to szczególne i wyjątkowe
sytuacje.
- Gdy włączono opcję `ODRYWANIE`, to znaczy, że sprawdzany jest poszerzony rdzeń podstawy
fundamentu (w przybliżeniu dwa razy większy od rdzenia właściwego). Sprawdzenie zasięgu
szczeliny między podłożem i podstawą fundamentu jest przeprowadzone według normy
*PN-81 B-03020* (p. 2.3 c), gdzie wymagane jest, aby zasięg szczeliny był mniejszy niż
połowa odległości między narożem, w którym występuje odrywanie, a prostą równoległą do
osi obojętnej przeprowadzonej przez środek fundamentu.
- Dopuszczalne naprężenia krawędziowe, które są porównywane z wartością graniczną podaną
na pierwszej planszy modułu [Podłoże](#podłoże).
- Osiadania średnie, obliczone metodą sumowania odkształceń warstw podłoża według punktu
F.1 normy. Metoda ta jest analogiczna do zalecanych zasad normy *PN-81 B-03020*.
- Różnica osiadań, obliczona w sposób analogiczny do osiadań średnich, zamiast naprężeń
średnich uwzględnia się maksymalne i minimalne. Warunek można interpretować jako
ograniczenie obrotu fundamentu wywołane nierównomiernym osiadaniem naroży od
mimośrodowego obciążenia.
- Stosunek nacisków na podłoże, który jest zaleceniem z doświadczeń praktyki projektowej
w celu ograniczenia nierównomiernego osiadania fundamentu. Sprawdzany jest poprzez
porównanie ilorazu maksymalnych i minimalnych naprężeń krawędziowych z wartościami
dopuszczalnymi z normy *PN-93 B-03201* lub z książki dr inż. Olgierda Puły
*Projektowanie fundamentów bezpośrednich według Eurokodu 7*.

![Wyniki sprawdzenia podłoża](wyniki_podloze.png)

Moduł sprawdza, czy element można zaprojektować jako niezbrojony zgodnie z
p. 12.9.3 normy *PN-EN 1992-1-1*. Wynik koloru pomarańczowego oznacza, że wysokość
fundamentu jest mniejsza niż zalecany podwójny wysięg odsadzki.

![Wynik stopy niezbrojonej](wyniki_niezbrojony.png)

Jeżeli nie jest spełniony warunek to zbrojenie jest wymiarowane na zginanie zgodnie
z normą *PN-EN 1992-1-1* w przekroju cofniętym od krawędzi na odległość 0,15 wymiaru
słupa lub ściany. Podane wartości powierzchni zbrojenia wymaganego `As,req`
oraz założonego `As,prov` dotyczą zbrojenia na całej długości krawędzi fundamentu.
W przypadku ław fundamentowych nie uwzględniono konstrukcyjnego zbrojenia podłużnego.
W przypadku stóp fundamentowych momenty gnące są wyznaczane domyślnie
*metodą wydzielonych wsporników prostokątnych*, alternatywnie można wybrać
*metodę wydzielonych wsporników trapezowych* w oknie `Ustawienia`.
Przyjęto, że zbrojenie w kierunku dłuższego boku stopy jest układane dołem
(kierunek Y w przypadku stopy kwadratowej).

Nośność fundamentu na przebicie (przez ścinanie) jest sprawdzana: dla stopy na
obwodach kontrolnych leżących w odległości od 0,5d do 2d (co 0,1) od skraju słupa w
myśl p. 6.4.2 (2) *PN-EN 1992-1-1*, a dla ławy w odległości 1d od skraju ściany.
Odległość krytyczna podana jest w opisie warunku. W przypadku, gdy obwód kontrolny
wykracza poza obręb powierzchni stopy nie zachodzi mechanizm przebicia.

![Wyniki wymiarowania zbrojenia](wyniki_zbrojenie.png)

**Rysunek w centralnej części** przedstawia geometrię fundamentu w rzucie z góry w
przypadku stopy lub przekrój poprzeczny w przypadku ławy, wraz z przebiegiem i
wartościami naprężeń maksymalnych i minimalnych na każdej krawędzi. Dodatkowo na
rysunku jest układ osi, schematyczne zbrojenie oraz poziomy w przypadku ławy.
Rysunek można przybliżać za pomocą pokrętła myszy oraz przesuwać trzymając lewy
przycisk myszy. Przydaje się to w przypadku, gdy opisy są blisko siebie i są trudne
do odczytania. Optymalne położenie rysunku w oknie najłatwiej uzyskać akceptując
ponownie dowolny parametr klawiszem `Enter` lub przyciskiem `Oblicz`.

![Rysunek stopy](rysunek.png)

**Ramka przycisków po prawej** stronie zawierająca następujące funkcje:
- Przycisk `Oblicz` aktualizuje rysunek i część z wynikami dla zadanych wartości.
- Przycisk `Dobierz` w sposób iteracyjny szuka geometrii fundamentu, która spełnia
wszystkie warunki sprawdzenia podłoża (nie dopuszcza odrywania). Jako kryterium
optymalnej geometrii przyjęto najmniejszą powierzchnię podstawy. W przypadku stopy
fundamentowej maksymalną proporcję długości do szerokości można zmienić w oknie
`Ustawienia`. Obliczenia są przeprowadzane w tle i przy obwiedni sił,
dużych wartościach sił lub słabym podłożu mogą trwać dłuższą chwilę.
- Przycisk `Podłoże` otwiera ponownie wcześniej opisane okno [Podłoże](#podłoże).
- Przycisk `Obciążenia` otwiera okno z wartościami obliczeniowych sił skupionych i
rozłożonych. Po włączeniu opcji `Własne` wszystkie wartości obciążeń można
dowolnie modyfikować oraz można wybrać wariant z obwiedni sił. Przycisk `Zeruj`
zeruje wszystkie obciążenia. Ponowne wciśnięcie przywraca wartości przed zerowaniem.
Przycisk `Y ⟺ Z` zamienia wartości sił w kierunku Y z wartościami w kierunku Z.
Można go użyć w zadaniach, w których oś pionowa to Y (domyślnie Z w górę).
- Przycisk `Ustawienia` zawiera dodatkowe opcje obliczeniowe oraz konfigurację wartości
parametrów takich jak dane materiałowe i częściowe współczynniki bezpieczeństwa (które
można przywrócić do wartości normowych przyciskiem `NA.2`). W dodatkowych opcjach
obliczeniowych można wybrać, czy podłoże sprawdzane jest w warunkach pracy
`z odpływem` czy `bez odpływu`. W przypadku wybrania opcji `bez odpływu` należy podać
wartość wytrzymałości gruntu na ścinanie. `Metoda wydzielonych wsporników` dotyczy
sposobu wyznaczania momentów gnących do wymiarowania zbrojenia stopy. Włączenie opcji
`Pokazuj sprawdzenie zerowych warunków i minimalne zbrojenie` powoduje, że w ramce z
wynikami są pokazywane również warunki, gdy stopień wytężenia wynosi 0% oraz sprawia,
że fundament jest liczony jako żelbetowy. Osiadanie jest porównywane z wartością
podaną w `Graniczna wartość osiadania`. Różnica osiadań jest porównywana z wartością
podaną w `Graniczna wartość różnicy osiadań`. `Maksymalna proporcja L:B w "Dobierz"`
służy do wybrania maksymalnej proporcji długości do szerokości stopy fundamentowej
szukanej funkcją `Dobierz`. Wybranie `1:1` sprawia, że stopa w rzucie jest kwadratowa.
- Przycisk `Wczytaj` umożliwia otwarcie pliku zadania z końcówką *.STO* w celu wczytania
wcześniej zapisanych danych.
- Przycisk `Zapisz` pozwala na zapisanie danych do pliku z końcówką *.STO* w wybranej
lokalizacji na dysku.
- Przycisk `Folder` pozwala określić domyślny folder do wczytywania i zapisywania
plików z danymi.
- Przycisk `Do schowka` kopiuje listę z notką obliczeniową do schowka. Po zamknięciu
modułu schowek zostaje wyczyszczony.
- Przycisk `Do Worda` otwiera nowy dokument zawierający notkę obliczeniową z rysunkiem.
Ponowne naciśnięcie przycisku powoduje dopisanie wyników do otwartego dokumentu.
W przypadku posiadania innego pakietu niż *Microsoft Office*, jest tworzony i otwierany
nowy plik *Nazwa_zadania.STO.DOCX* w lokalizacji zadania.
- Przycisk `Aktualizuj` sprawdza, czy jest uruchomiona aktualna wersja pakietu oraz w
razie potrzeby umożliwia pobranie i aktualizację do najnowszej wersji. Plik instalacyjny
jest pobierany w tle, trzeba poczekać na jego pobranie. Następnie moduł jest wyłączany
i uruchamia się instalacja. Zaleca się zamknięcie programu **ABC** przed instalacją.
Pomarańczowy kolor czcionki przycisku sygnalizuje, że jest dostępna aktualizacja.
- Przycisk `Instrukcja` otwiera niniejszą stronę internetową z instrukcją modułu.
- Przycisk `Zamknij` zapisuje wyniki i zamyka moduł, skąd można przejść do wyboru
kolejnego miejsca. W przypadku stóp fundamentowych miejsca zaprojektowane będą opisane
*Stopa*, a podpowiadane będzie kolejne miejsce z największą reakcją pionową.
- Przełączanie opcji `Zawsze na wierzchu` powoduje przypięcie lub odpięcie modułu ponad
innymi oknami (domyślnie włączony przy uruchamianiu z programu **ABC**).
- Zaznaczenie opcji `Domyślne` powoduje, że po zamknięciu modułu bieżące ustawienia
zostają zapisane jako domyślne do wymiarowania kolejnych miejsc.

![image](https://github.com/pkpkbud/fundamenty/assets/55211992/e88f781a-19ab-42cf-b5f1-507f2f21484c)

