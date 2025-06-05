## Notatki na I Kolokwium z PEE

### 1. Dwójnik Szeregowy RLC

**Co to jest?**
Dwójnik szeregowy RLC to obwód elektryczny, w którym opornik (R), cewka (L) i kondensator (C) są połączone jeden za drugim (szeregowo) i zasilane prądem przemiennym (sinusoidalnym).

**Kluczowe informacje:**
*   **Prąd:** W połączeniu szeregowym przez wszystkie elementy płynie ten sam prąd `i(t)`. Jeśli `i(t) = Im sin(ωt)`, to napięcia na poszczególnych elementach będą miały różne fazy względem tego prądu.
*   **Napięcia na elementach:**
    *   **Rezystor (R):** Napięcie `uR` jest w fazie z prądem. `uR = R · Im sin(ωt)`.
    *   **Cewka (L):** Napięcie `uL` wyprzedza prąd o 90° (π/2). `uL = ωL · Im sin(ωt + π/2)`. `XL = ωL` to reaktancja indukcyjna (opór cewki dla prądu przemiennego).
    *   **Kondensator (C):** Napięcie `uC` opóźnia się względem prądu o 90° (π/2). `uC = (1/ωC) · Im sin(ωt - π/2)`. `XC = 1/ωC` to reaktancja pojemnościowa (opór kondensatora dla prądu przemiennego).
*   **Napięcie całkowite (źródła):** Jest sumą wektorową napięć na poszczególnych elementach: `U = √(UR² + (UL - UC)²)`.
*   **Impedancja (Z):** To całkowity opór obwodu dla prądu przemiennego. `Z = √(R² + (XL - XC)²)`. Jednostka: Om [Ω].
    *   `X = XL - XC` nazywamy reaktancją wypadkową obwodu.
*   **Prawo Ohma dla obwodu RLC:** `U = Z · I` (dla wartości skutecznych) lub `Um = Z · Im` (dla amplitud).
*   **Kąt przesunięcia fazowego (φ):** Kąt między napięciem całkowitym `U` a prądem `I`.
    *   Jeśli `XL > XC`, obwód ma charakter indukcyjny, napięcie wyprzedza prąd (φ > 0).
    *   Jeśli `XC > XL`, obwód ma charakter pojemnościowy, prąd wyprzedza napięcie (φ < 0).
    *   Jeśli `XL = XC`, obwód ma charakter rezystancyjny (φ = 0) – jest to **rezonans napięć**.
*   **Rezonans napięć:**
    *   Warunek: `XL = XC`, czyli `ωL = 1/ωC`.
    *   Częstotliwość rezonansowa: `fr = 1 / (2π√(LC))`.
    *   W rezonansie: `Z = R` (impedancja jest minimalna i równa rezystancji), prąd w obwodzie jest maksymalny, napięcie jest w fazie z prądem (φ = 0).
    *   Napięcia `UL` i `UC` mogą być znacznie większe od napięcia zasilającego, ale znoszą się wzajemnie.

**Co narysować?**
![alt text](https://files.catbox.moe/elz0l2.png)
---

### 2. Dwójnik Równoległy RLC

**Co to jest?**
Dwójnik równoległy RLC to obwód, w którym opornik (R), cewka (L) i kondensator (C) są połączone równolegle do tego samego źródła napięcia przemiennego (sinusoidalnego).

**Kluczowe informacje:**
*   **Napięcie:** W połączeniu równoległym na wszystkich elementach jest to samo napięcie `u(t)`. Jeśli `u(t) = Um sin(ωt)`.
*   **Prądy w gałęziach:**
    *   **Rezystor (R):** Prąd `iR` jest w fazie z napięciem. `iR = (Um/R) sin(ωt) = G · Um sin(ωt)`. `G = 1/R` to konduktancja (przewodność czynna).
    *   **Cewka (L):** Prąd `iL` opóźnia się względem napięcia o 90° (π/2). `iL = (Um/XL) sin(ωt - π/2) = BL · Um sin(ωt - π/2)`. `BL = 1/XL` to susceptancja indukcyjna (przewodność bierna indukcyjna).
    *   **Kondensator (C):** Prąd `iC` wyprzedza napięcie o 90° (π/2). `iC = (Um/XC) sin(ωt + π/2) = BC · Um sin(ωt + π/2)`. `BC = 1/XC` to susceptancja pojemnościowa (przewodność bierna pojemnościowa).
*   **Prąd całkowity (źródła):** Jest sumą wektorową prądów w poszczególnych gałęziach: `I = √(IR² + (IC - IL)²)`.
*   **Admitancja (Y):** To odwrotność impedancji, miara "łatwości" przepływu prądu. `Y = √(G² + (BC - BL)²)`. Jednostka: Siemens [S].
    *   `B = BC - BL` nazywamy susceptancją wypadkową obwodu.
*   **Prawo Ohma (postać admitancyjna):** `I = Y · U`.
*   **Kąt przesunięcia fazowego (φ):** Kąt między prądem całkowitym `I` a napięciem `U`.
    *   Jeśli `BC > BL`, obwód ma charakter pojemnościowy, prąd wyprzedza napięcie (φ > 0).
    *   Jeśli `BL > BC`, obwód ma charakter indukcyjny, napięcie wyprzedza prąd (φ < 0).
    *   Jeśli `BC = BL`, obwód ma charakter rezystancyjny (φ = 0) – jest to **rezonans prądów**.
*   **Rezonans prądów:**
    *   Warunek: `BC = BL`, czyli `ωC = 1/ωL`.
    *   Częstotliwość rezonansowa: `fr = 1 / (2π√(LC))` (taka sama jak dla rezonansu napięć).
    *   W rezonansie: `Y = G` (admitancja jest minimalna i równa konduktancji), prąd pobierany ze źródła jest minimalny, prąd jest w fazie z napięciem (φ = 0).
    *   Prądy `IL` i `IC` mogą być znacznie większe od prądu źródłowego, ale znoszą się wzajemnie (prąd krąży między cewką a kondensatorem).

**Co narysować?**

![alt text](https://files.catbox.moe/krwyjz.png)

---

### 3. Budowa Tranzystora Bipolarnego, Symbole, Charakterystyki Tranzystora

**Co to jest tranzystor bipolarny?**
Tranzystor bipolarny (BJT - Bipolar Junction Transistor) to element półprzewodnikowy zbudowany z trzech warstw półprzewodnika typu P i N, tworzących dwa złącza P-N. Służy głównie do wzmacniania sygnałów elektrycznych lub jako elektroniczny przełącznik. "Bipolarny" oznacza, że w jego działaniu biorą udział oba rodzaje nośników ładunku: elektrony i dziury.

**Budowa:**
*   **Warstwy:**
    *   **Emiter (E):** Silnie domieszkowany, emituje (wstrzykuje) nośniki ładunku do bazy.
    *   **Baza (B):** Cienka i słabo domieszkowana warstwa środkowa, steruje przepływem nośników między emiterem a kolektorem.
    *   **Kolektor (C):** Średnio domieszkowany, zbiera nośniki ładunku przepływające z emitera przez bazę.
*   **Typy:**
    *   **NPN:** Warstwy N - P - N (emiter N, baza P, kolektor N). Prąd płynie głównie dzięki elektronom.
    *   **PNP:** Warstwy P - N - P (emiter P, baza N, kolektor P). Prąd płynie głównie dzięki dziurom.

**Symbole:**
*   **NPN:** Strzałka na emiterze skierowana na zewnątrz (od bazy). "Nie Płynie do Niej" (strzałka).
*   **PNP:** Strzałka na emiterze skierowana do wewnątrz (do bazy). "Płynie ku Niej" (strzałka).
    (Slajd "TRANZYSTORY BIPOLARNE I UKŁADY WZMACNIACZY", str. 9, Rys. 2)

**Zasada działania (dla NPN w stanie aktywnym - wzmacniania):**
1.  **Polaryzacja:**
    *   Złącze Emiter-Baza (BE): spolaryzowane w kierunku przewodzenia (ok. +0,7V na bazie względem emitera dla krzemowego NPN).
    *   Złącze Kolektor-Baza (CB): spolaryzowane w kierunku zaporowym (kolektor ma wyższy potencjał dodatni niż baza).
2.  **Przepływ prądu:**
    *   Elektrony z emitera (N) są wstrzykiwane do bazy (P).
    *   Większość elektronów (ok. 95-99%) przechodzi przez cienką bazę do kolektora (N), przyciągana przez jego dodatni potencjał. Tworzy to prąd kolektora `IC`.
    *   Niewielka część elektronów rekombinuje z dziurami w bazie, tworząc mały prąd bazy `IB`.
    *   Prąd emitera `IE = IB + IC`.
3.  **Sterowanie:** Mała zmiana prądu bazy `IB` powoduje dużą zmianę prądu kolektora `IC`.
4.  **Wzmocnienie prądowe (β lub hFE):** Stosunek prądu kolektora do prądu bazy: `β = IC / IB`. Typowo wartości od kilkudziesięciu do kilkuset.

**Charakterystyki Tranzystora:** (Najczęściej dla konfiguracji Wspólnego Emitera - WE)
*   **Charakterystyka wejściowa:** Zależność prądu bazy `IB` od napięcia baza-emiter `UBE`, przy stałym napięciu kolektor-emiter `UCE`.
    *   Wygląda jak charakterystyka diody spolaryzowanej w kierunku przewodzenia. Prąd `IB` zaczyna znacząco płynąć, gdy `UBE` osiągnie ok. 0,6-0,7V (dla krzemu).
    (Slajd "TRANZYSTORY BIPOLARNE I UKŁADY WZMACNIACZY", str. 16, lewy wykres)
*   **Charakterystyka wyjściowa:** Zależność prądu kolektora `IC` od napięcia kolektor-emiter `UCE`, przy stałym prądzie bazy `IB` (rodzina charakterystyk dla różnych `IB`).
    *   **Obszar odcięcia (zatkania):** `IB` = 0, `IC` ≈ 0. Tranzystor nie przewodzi.
    *   **Obszar aktywny (liniowy):** `IC` jest proporcjonalne do `IB` (`IC = β·IB`) i prawie niezależne od `UCE`. Tranzystor działa jak wzmacniacz.
    *   **Obszar nasycenia:** `IC` przestaje rosnąć wraz ze wzrostem `IB` i jest ograniczone przez obwód zewnętrzny. `UCE` jest małe (ok. 0,2V). Tranzystor działa jak zamknięty przełącznik.
    (Slajd "TRANZYSTORY BIPOLARNE I UKŁADY WZMACNIACZY", str. 16, prawy wykres)
*   **Prosta obciążenia:** Linia na charakterystyce wyjściowej, reprezentująca zależność `IC` od `UCE` narzuconą przez zewnętrzny obwód (rezystor w kolektorze RC i napięcie zasilania UCC). Wyznacza możliwe punkty pracy tranzystora.
    (Slajd "TRANZYSTORY BIPOLARNE I UKŁADY WZMACNIACZY", str. 20, Rys. 11)
*   **Punkt pracy (Q):** Punkt przecięcia prostej obciążenia z charakterystyką wyjściową dla danego prądu bazy `IB`. Określa stałe wartości `ICQ` i `UCEQ` przy braku sygnału wejściowego.

**Co narysować?**

![alt text](https://files.catbox.moe/4t2lp6.png)
---

### 4. Układy Zasilania Wzmacniacza: Układ Potencjometryczny i Układ ze Sprzężeniem Kolektorowym

**Po co układy zasilania (polaryzacji)?**
Aby tranzystor pracował poprawnie jako wzmacniacz, musi być odpowiednio spolaryzowany, tzn. na jego złączach muszą panować odpowiednie napięcia stałe. To ustala tzw. **punkt pracy (Q)** w obszarze aktywnym charakterystyki. Punkt pracy powinien być stabilny, tzn. mało wrażliwy na zmiany temperatury i różnice w parametrach tranzystorów (np. β).

**A) Układ potencjometryczny (dzielnika napięcia)**
*   **Budowa:** Napięcie na bazę jest podawane z dzielnika napięcia utworzonego przez rezystory R1 (między UCC a bazą) i R2 (między bazą a masą). W obwodzie kolektora jest rezystor RC, a w obwodzie emitera często rezystor RE (dla stabilizacji).
    (Slajd "TRANZYSTORY BIPOLARNE I UKŁADY WZMACNIACZY", str. 23, Rys. 13)
*   **Działanie:** Rezystory R1 i R2 ustalają stałe napięcie na bazie `VB`. Napięcie na emiterze `VE = VB - UBE` (gdzie `UBE` ≈ 0,7V). Prąd emitera `IE = VE / RE`. Prąd kolektora `IC ≈ IE`.
*   **Zalety:** Zapewnia dobrą stabilizację punktu pracy, szczególnie jeśli prąd płynący przez dzielnik (R1, R2) jest znacznie większy niż prąd bazy `IB`, a rezystancja `RE` jest odpowiednio duża. Stosunkowo niezależny od β.
*   **Wady:** Wymaga więcej elementów. Potencjalne problemy, jeśli źle zaprojektowany (opisane na str. 24).

**B) Układ ze sprzężeniem kolektorowym (ujemnym sprzężeniem zwrotnym z kolektora)**
*   **Budowa:** Rezystor bazowy RB jest podłączony między kolektorem a bazą tranzystora (a nie bezpośrednio do UCC). W obwodzie kolektora jest rezystor RC.
    (Slajd "TRANZYSTORY BIPOLARNE I UKŁADY WZMACNIACZY", str. 26, Rys. 17)
*   **Działanie (stabilizacja):** Jest to przykład ujemnego sprzężenia zwrotnego.
    *   Jeśli z jakiegoś powodu prąd kolektora `IC` wzrośnie (np. przez wzrost temperatury lub β), to spadek napięcia na `RC` (`IC·RC`) również wzrośnie.
    *   To powoduje, że napięcie na kolektorze `VC = UCC - IC·RC` zmaleje.
    *   Ponieważ baza jest połączona z kolektorem przez `RB`, spadek `VC` powoduje spadek napięcia na bazie `VB`, a tym samym spadek prądu bazy `IB`.
    *   Mniejszy prąd `IB` powoduje zmniejszenie prądu `IC`, co przeciwdziała pierwotnemu wzrostowi `IC`.
*   **Zalety:** Lepsza stabilizacja punktu pracy niż w układzie z stałym prądem bazy (gdzie RB jest do UCC). Prostszy niż układ potencjometryczny. Zapobiega wejściu tranzystora w głębokie nasycenie.
*   **Wady:** Zależność `IC` od β, choć mniejsza niż w układzie z stałym prądem bazy, jest wciąż obecna. Wzór na `IC=(UCC- UBE)/(RC + RB/β)` pokazuje, że wpływ β jest mniejszy, jeśli `RB/β` jest małe w porównaniu do `RC`.

**Co narysować?**

![alt text](https://files.catbox.moe/5xpytq.png)

---

### 5. Funkcje Specjalne w LOGO: Symbole Graficzne i Przebiegi Czasowe

Sterownik LOGO! posiada wiele gotowych bloków funkcyjnych, które ułatwiają programowanie. Skupimy się na trzech wymienionych.

**A) Opóźnione wyłączenie (Off-Delay Timer)**
*   **Symbol graficzny:** Prostokątny blok z wejściem wyzwalającym `Trg` (Trigger), wejściem resetującym `R` (Reset), parametrem czasu `T` (lub Par) i wyjściem `Q`.
    (Slajd "STEROWNIK PROGRAMOWALNY LOGO", str. 11 - ogólna tabela, str. 13 - szczegółowy opis i symbol)
*   **Działanie:**
    1.  Gdy na wejściu `Trg` pojawi się sygnał wysoki (stan 1, zbocze narastające 0->1), wyjście `Q` natychmiast staje się aktywne (stan 1).
    2.  Gdy sygnał na `Trg` zaniknie (stan 0, zbocze opadające 1->0), rozpoczyna się odliczanie zadanego czasu `T`.
    3.  Wyjście `Q` pozostaje w stanie wysokim (1) przez cały czas odliczania `T`.
    4.  Po upływie czasu `T`, wyjście `Q` przechodzi w stan niski (0).
    5.  Jeśli podczas odliczania czasu `T` na wejściu `Trg` ponownie pojawi się stan wysoki, odliczanie jest przerywane, a wyjście `Q` pozostaje w stanie wysokim. Nowe odliczanie rozpocznie się po kolejnym zaniku sygnału na `Trg`.
    6.  Sygnał wysoki na wejściu `R` (Reset) natychmiast zeruje wyjście `Q` i zatrzymuje odliczanie czasu.
*   **Przebieg czasowy:**
    (Slajd "STEROWNIK PROGRAMOWALNY LOGO", str. 13 - Wykres czasowy)
    *   `Trg`: Impuls lub sygnał trwający pewien czas.
    *   `Q`: Aktywuje się wraz z `Trg`, a dezaktywuje po czasie `T` od momentu, gdy `Trg` przestaje być aktywny.
    *   `Ta`: Czas odmierzany przez timer.

**B) Podtrzymane opóźnione załączenie (Retentive On-Delay Timer / Opóźnienie z podtrzymaniem)**
*   **Symbol graficzny:** Prostokątny blok z wejściem wyzwalającym `Trg`, wejściem resetującym `R`, parametrem czasu `T` (Par) i wyjściem `Q`.
    (Slajd "STEROWNIK PROGRAMOWALNY LOGO", str. 11 - ogólna tabela, str. 14 - górny schemat "Opóźnienie z podtrzymaniem")
*   **Działanie:**
    1.  Gdy na wejściu `Trg` pojawi się sygnał wysoki (stan 1, zbocze narastające 0->1), rozpoczyna się odliczanie zadanego czasu `T`.
    2.  Jeśli sygnał na `Trg` zaniknie (stan 0) *zanim* upłynie czas `T`, odliczanie jest kontynuowane (podtrzymywane).
    3.  Po upływie skumulowanego czasu `T` (nawet jeśli `Trg` już nie jest aktywne), wyjście `Q` staje się aktywne (stan 1).
    4.  Wyjście `Q` pozostaje w stanie wysokim (1) niezależnie od dalszych zmian na `Trg`, aż do momentu pojawienia się sygnału wysokiego na wejściu `R` (Reset).
    5.  Sygnał wysoki na wejściu `R` natychmiast zeruje wyjście `Q` i czas skumulowany `Ta`.
*   **Przebieg czasowy:**
    (Slajd "STEROWNIK PROGRAMOWALNY LOGO", str. 14 - górny Wykres czasowy dla "Opóźnienie z podtrzymaniem")
    *   `Trg`: Może być krótkim impulsem.
    *   `Q`: Aktywuje się po czasie `T` od pierwszego zbocza narastającego na `Trg`, nawet jeśli `Trg` już opadło. Pozostaje aktywne do Resetu.
    *   `Ta`: Czas odmierzany przez timer, nie zeruje się po zaniku `Trg` (jeśli opcja podtrzymania jest aktywna).

**C) AND z pamięcią stanu (zbocze) (AND with edge detection / memory)**
*   **Symbol graficzny:** Blok funkcji AND (`&`) z dodatkowym symbolem strzałki w górę (`↑`) przy jednym lub wszystkich wejściach, wskazującym na detekcję zbocza narastającego, oraz wyjściem `Q`.
    (Slajd "STEROWNIK PROGRAMOWALNY LOGO", str. 10 - oznaczenie w LOGO!)
*   **Działanie:**
    1.  Wyjście `Q` bloku przyjmuje stan wysoki (1), jeśli:
        *   Wszystkie wejścia (np. 1, 2, 3, 4) są w stanie wysokim (1) ORAZ
        *   Przynajmniej jedno z wejść (to z detekcją zbocza) w poprzednim cyklu programu miało stan niski (0), a w obecnym cyklu przeszło w stan wysoki (1) (czyli nastąpiło zbocze narastające 0->1 na tym wejściu).
    2.  Po ustawieniu wyjścia `Q` na stan 1, może ono pozostać w tym stanie (efekt pamięci) nawet jeśli warunek zbocza już nie jest spełniony, dopóki wszystkie wejścia są wysokie. Jeśli którekolwiek wejście przejdzie w stan 0, wyjście `Q` również przejdzie w stan 0.
    *(Uwaga: Dokładne zachowanie "pamięci" może zależeć od konkretnej implementacji w LOGO! – czy jest to jednorazowe wykrycie zbocza przy spełnieniu warunku AND, czy też wyjście jest typu "Set". Slajd 10 sugeruje, że wyjście jest aktywne, gdy warunki są spełnione, a zbocze wystąpiło.)*
*   **Przebieg czasowy:**
    (Slajd "STEROWNIK PROGRAMOWALNY LOGO", str. 10 - Wykres czasowy sygnałów)
    *   Wejścia 1, 2, 3, 4: Różne kombinacje sygnałów.
    *   Wyjście Q: Staje się aktywne (1) tylko w tych cyklach (`Cycle`), gdzie wszystkie wejścia są 1, a na przynajmniej jednym z nich (np. wejście 1 na wykresie) właśnie nastąpiło przejście z 0 na 1. Widać, że w cyklu 1 Q=1, bo wszystkie In=1 i In1 zmieniło się z 0->1. W cyklu 2, mimo że In=1, Q=0, bo nie było nowego zbocza.

**Co narysować?**

![alt text](https://files.catbox.moe/zcltrc.png)
---

Powodzenia na kolokwium! Pamiętaj, aby dobrze zrozumieć zasadę działania każdego elementu i funkcji, a rysunki traktować jako pomoc wizualną.
