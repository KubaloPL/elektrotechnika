**1. Dwójnik Szeregowy RLC (Slajdy 21, 22)**

*   **Co to jest?** Wyobraź sobie obwód elektryczny, w którym masz połączone jeden za drugim (szeregowo) trzy elementy: rezystor (R), cewkę (L) i kondensator (C). Taki zestaw nazywamy dwójnikiem szeregowym RLC. Podłączamy go do źródła napięcia przemiennego (sinusoidalnego).
*   **Jak płynie prąd?** Przez wszystkie te trzy elementy płynie ten sam prąd przemienny (sinusoidalny). Dla uproszczenia zakłada się, że na początku (w chwili t=0) prąd jest równy zero i zaczyna rosnąć (faza początkowa prądu jest zero).
*   **Napięcia na elementach:**
    *   **Rezystor (R):** Napięcie na rezystorze (UR) jest "zgodne w fazie" z prądem. Oznacza to, że gdy prąd osiąga szczyt, napięcie na rezystorze też osiąga szczyt. Jest proporcjonalne do prądu (UR = R * I).
    *   **Cewka (L):** Napięcie na cewce (UL) "wyprzedza" prąd o 90 stopni (π/2). Oznacza to, że napięcie osiąga szczyt, zanim zrobi to prąd. Cewka "nie lubi" zmian prądu i reaguje na nie napięciem. Wielkość tego napięcia zależy od tzw. reaktancji indukcyjnej (XL = ωL), gdzie ω to pulsacja (związana z częstotliwością). UL = XL * I.
    *   **Kondensator (C):** Napięcie na kondensatorze (UC) "opóźnia się" względem prądu o 90 stopni (π/2). Oznacza to, że prąd osiąga szczyt, zanim zrobi to napięcie. Kondensator "nie lubi" zmian napięcia. Wielkość tego napięcia zależy od tzw. reaktancji pojemnościowej (XC = 1/ωC). UC = XC * I.
*   **Napięcie całkowite (U):** Całkowite napięcie źródła (U) musi pokonać napięcia na wszystkich elementach. Ale nie możemy ich po prostu dodać jak zwykłe liczby, bo mają różne fazy (przesunięcia w czasie). Dodajemy je "wektorowo". Napięcie UR jest w fazie z prądem, UL wyprzedza prąd o 90°, a UC opóźnia się o 90°.
*   **Wykresy wektorowe:**
    *   Na wykresach (b, c, d) prąd (I) jest wektorem skierowanym w prawo (nasza referencja).
    *   Wektor UR też jest w prawo.
    *   Wektor UL jest skierowany w górę (wyprzedza o 90°).
    *   Wektor UC jest skierowany w dół (opóźnia się o 90°).
    *   Całkowite napięcie U to suma tych wektorów. Najpierw "odejmujemy" wektory UL i UC (bo są przeciwnie skierowane), a potem dodajemy wynik (UL - UC) do UR za pomocą twierdzenia Pitagorasa.
*   **Impedancja (Z):** To jest całkowity "opór" obwodu RLC dla prądu przemiennego. Składa się z rezystancji (R) i całkowitej reaktancji (X = XL - XC). Obliczamy ją wzorem: Z = √(R² + (XL - XC)²). Jednostką impedancji jest Om (Ω).
*   **Prawo Ohma dla AC:** Podobnie jak w obwodach prądu stałego (U=RI), tutaj mamy U = Z * I (gdzie U i I to wartości skuteczne napięcia i prądu).
*   **Charakter obwodu:**
    *   Jeśli XL > XC (cewka "dominuje"), obwód ma charakter **indukcyjny**. Napięcie całkowite U wyprzedza prąd.
    *   Jeśli XL < XC (kondensator "dominuje"), obwód ma charakter **pojemnościowy**. Napięcie całkowite U opóźnia się względem prądu.
    *   Jeśli XL = XC, reaktancje się znoszą (X=0). Obwód ma charakter **rezystancyjny**. Impedancja jest minimalna (Z=R). Napięcie U jest w fazie z prądem. Nazywamy to **rezonansem napięć**. Wtedy prąd w obwodzie jest największy.
*   **Trójkąty napięć:** W przypadkach indukcyjnym i pojemnościowym, wektory UR, (UL-UC) i U tworzą trójkąt prostokątny, nazywany trójkątem napięć.

**2. Dwójnik Równoległy RLC (Slajdy 23, 24)**

*   **Co to jest?** Teraz te same trzy elementy (R, L, C) łączymy "obok siebie", czyli równolegle. Wszystkie są podłączone do tego samego źródła napięcia przemiennego (u = Um sin ωt).
*   **Jak płynie prąd?** Napięcie na każdym elemencie jest takie samo i równe napięciu źródła (U). Ale prąd całkowity ze źródła (i) rozdziela się na prądy płynące przez poszczególne gałęzie: IR (przez rezystor), IL (przez cewkę), IC (przez kondensator). Całkowity prąd i = IR + IL + IC (dodawanie chwilowe).
*   **Prądy w gałęziach:**
    *   **Rezystor (R):** Prąd IR jest w fazie z napięciem U. IR = U / R = G * U (G = 1/R to konduktancja - "łatwość przewodzenia").
    *   **Cewka (L):** Prąd IL opóźnia się względem napięcia U o 90 stopni (π/2). IL = U / XL = BL * U (BL = 1/XL to susceptancja indukcyjna - "podatność" na przepływ prądu).
    *   **Kondensator (C):** Prąd IC wyprzedza napięcie U o 90 stopni (π/2). IC = U / XC = BC * U (BC = 1/XC to susceptancja pojemnościowa).
*   **Prąd całkowity (I):** Podobnie jak poprzednio, prądów nie dodajemy algebraicznie, tylko wektorowo, bo mają różne fazy. Napięcie U jest teraz naszą referencją (skierowane w prawo).
*   **Wykresy wektorowe:**
    *   Wektor U jest w prawo.
    *   Wektor IR jest w prawo (w fazie z U).
    *   Wektor IL jest w dół (opóźnia się o 90°).
    *   Wektor IC jest w górę (wyprzedza o 90°).
    *   Całkowity prąd I to suma wektorowa IR, IL, IC. Najpierw "odejmujemy" wektory IC i IL, a potem dodajemy wynik (IC - IL) do IR za pomocą Pitagorasa.
*   **Admitancja (Y):** To jest odwrotność impedancji (Y=1/Z), czyli miara "łatwości", z jaką obwód przewodzi prąd przemienny. Składa się z konduktancji (G) i całkowitej susceptancji (B = BC - BL). Obliczamy ją wzorem: Y = √(G² + (BC - BL)²). Jednostką admitancji jest Siemens (S).
*   **Prawo Ohma (postać admitancyjna):** I = Y * U.
*   **Charakter obwodu:**
    *   Jeśli BC > BL (kondensator "dominuje" pod względem prądu), obwód ma charakter **pojemnościowy**. Prąd całkowity I wyprzedza napięcie U. (Uwaga: W tekście jest błąd, powinno być "pojemnościowy charakter obwodu", a nie "indukcyjny").
    *   Jeśli BC < BL (cewka "dominuje" pod względem prądu), obwód ma charakter **indukcyjny**. Prąd całkowity I opóźnia się względem napięcia U.
    *   Jeśli BC = BL, susceptancje się znoszą (B=0). Obwód ma charakter **rezystancyjny**. Admitancja jest minimalna (Y=G). Prąd I jest w fazie z napięciem U. Nazywamy to **rezonansem prądów**. Wtedy prąd pobierany ze źródła jest najmniejszy.
*   **Trójkąty prądów/admitancji:** W przypadkach indukcyjnym i pojemnościowym, wektory IR, (IC-IL) i I tworzą trójkąt prostokątny (trójkąt prądów). Podobnie wektory G, (BC-BL) i Y tworzą trójkąt admitancji.

**3. Budowa, Symbole, Charakterystyki Tranzystora Bipolarnego (Slajdy 9, 10, 15, 16)**

*   **Co to jest tranzystor bipolarny (BJT)?** To element elektroniczny zbudowany z trzech warstw półprzewodnika (typu N i P), ułożonych jako N-P-N lub P-N-P. Ma trzy wyprowadzenia: Emiter (E), Bazę (B) i Kolektor (C). Słowo "bipolarny" oznacza, że w jego działaniu biorą udział dwa rodzaje nośników ładunku: elektrony i dziury.
*   **Jak działa (w uproszczeniu)?** Działa jak sterowany "zawór" lub "kran" dla prądu elektrycznego. Mały prąd wpływający do Bazy (IB) kontroluje znacznie większy prąd płynący między Kolektorem a Emiterem (IC).
    *   **Emiter (E):** Emituje (wstrzykuje) nośniki ładunku (elektrony w NPN, dziury w PNP) do bazy.
    *   **Baza (B):** Cienka warstwa środkowa, która kontroluje przepływ nośników z emitera do kolektora.
    *   **Kolektor (C):** Zbiera (kolekcjonuje) nośniki, które przeszły przez bazę.
*   **Typy NPN i PNP:** Różnią się kolejnością warstw i kierunkiem przepływu prądu oraz polaryzacją napięć potrzebnych do działania. Na symbolach strzałka na emiterze pokazuje kierunek przepływu prądu (zgodnie z konwencją, od + do -):
    *   **NPN:** Strzałka "Nie Wskazuje do środka" (wychodzi z emitera). Prąd płynie od kolektora do emitera (IC), sterowany prądem wpływającym do bazy (IB). Potrzebuje dodatnich napięć na bazie i kolektorze względem emitera.
    *   **PNP:** Strzałka "Wskazuje do środka" (wchodzi do emitera). Prąd płynie od emitera do kolektora, sterowany prądem wypływającym z bazy. Potrzebuje ujemnych napięć na bazie i kolektorze względem emitera.
*   **Model diodowy:** Można myśleć o tranzystorze jak o dwóch diodach połączonych "plecami" (PNP) lub "przodami" (NPN) ze wspólną warstwą. Jednak sam model diodowy nie wyjaśnia w pełni działania tranzystora (efektu wzmocnienia).
*   **Warunki pracy (stan aktywny - wzmacnianie):** Aby tranzystor działał jak wzmacniacz, muszą być spełnione warunki:
    *   Złącze Baza-Emiter (BE) musi być spolaryzowane **w kierunku przewodzenia** (jak włączona dioda, napięcie UBE ok. 0.6-0.7V dla krzemu).
    *   Złącze Kolektor-Baza (CB) musi być spolaryzowane **w kierunku zaporowym** (jak wyłączona dioda).
*   **Wzmocnienie prądowe (β):** Stosunek prądu kolektora (IC) do prądu bazy (IB) w stanie aktywnym. IC ≈ β * IB. Beta jest zwykle duża (np. 50-500), co oznacza, że mały prąd bazy kontroluje duży prąd kolektora.
*   **Charakterystyki statyczne:** To wykresy pokazujące zależności między prądami i napięciami tranzystora.
    *   **Charakterystyka wejściowa:** Pokazuje zależność prądu bazy (IB) od napięcia baza-emiter (UBE), przy stałym napięciu kolektor-emiter (UCE). Wygląda podobnie do charakterystyki diody.
    *   **Charakterystyka wyjściowa:** Pokazuje zależność prądu kolektora (IC) od napięcia kolektor-emiter (UCE), dla różnych ustalonych wartości prądu bazy (IB). Widać na niej, że IC zależy głównie od IB, a tylko nieznacznie od UCE (w obszarze aktywnym).
*   **Kluczowa zasada:** Tranzystor bipolarny jest sterowany **prądowo** - prądem bazy (IB). Mała zmiana prądu bazy powoduje dużą zmianę prądu kolektora.

**4. Układy Zasilania (Polaryzacji) Wzmacniacza na Tranzystorze Bipolarnym (Slajdy 23, 26, 27)**

*   **Po co polaryzacja?** Zanim podamy na wejście tranzystora sygnał, który ma być wzmocniony (np. słaby sygnał audio), musimy ustawić tranzystor w odpowiednim "punkcie pracy" (Q-point). Oznacza to zapewnienie stałych napięć i prądów (UBE, UCE, IB, IC) tak, aby tranzystor był w stanie aktywnym (gotowy do wzmacniania). Układy polaryzacji dostarczają te stałe napięcia/prądy ze źródła zasilania (np. Ucc).
*   **a) Układ z potencjometrycznym zasilaniem bazy (dzielnik napięcia) (Slajd 23)**
    *   **Jak działa?** Dwa rezystory (R1 i R2) podłączone do źródła Ucc tworzą dzielnik napięcia. Napięcie w punkcie między nimi ustala napięcie bazy (UB). To napięcie, pomniejszone o spadek na złączu BE (ok. 0.7V), daje napięcie emitera (UE). Prąd emitera (IE) płynie przez rezystor emiterowy (RE - nie pokazany na tym konkretnym schemacie, ale często obecny), a prąd kolektora (IC ≈ IE) przez rezystor kolektorowy (RC).
    *   **Zalety:** Jest to najpopularniejszy i najbardziej stabilny układ polaryzacji. Napięcie bazy jest dość "sztywno" ustalone przez dzielnik i mniej zależne od zmian parametru β tranzystora czy temperatury.
    *   **Obliczenia:** Używa się praw Kirchhoffa i prawa Ohma. Równanie `UCC = IC*RC + UCE` opisuje tzw. **prostą obciążenia** na charakterystyce wyjściowej. Punkt pracy (Q) to punkt przecięcia prostej obciążenia z odpowiednią krzywą charakterystyki (dla danego IB). Napięcie bazy można wyliczyć ze wzoru na dzielnik `UB = UCC * (R2 / (R1 + R2))`, a potem `UBE = UB - UE`. Znając punkt pracy (IC, UCE) i wymagane UBE, można dobrać wartości R1 i R2.
    *   **Wady:** Schemat na Rys. 13 (bez rezystora emiterowego RE) jest w rzeczywistości "najgorszym sposobem", jak wspomniano w tekście, bo jest bardzo wrażliwy na zmiany UBE i β. Stabilność uzyskuje się dopiero po dodaniu RE.
*   **b) Układ ze sprzężeniem kolektorowym (Slajd 26, 27)**
    *   **Jak działa?** Rezystor bazy (RB) jest podłączony nie bezpośrednio do zasilania Ucc, ale do **kolektora** tranzystora.
    *   **Sprzężenie zwrotne ujemne:** To jest kluczowa cecha tego układu. Wyobraźmy sobie, że z jakiegoś powodu (np. wzrost temperatury) prąd kolektora IC chce wzrosnąć. Wzrost IC powoduje większy spadek napięcia na RC (URC = (IC+IB)*RC), co oznacza, że napięcie na kolektorze (UCE) maleje. Ponieważ baza jest podłączona do kolektora przez RB, spadek UCE powoduje też spadek napięcia na RB, a tym samym zmniejszenie prądu bazy IB. Mniejszy IB prowadzi do zmniejszenia IC, przeciwdziałając pierwotnemu wzrostowi. Układ sam stabilizuje swój punkt pracy.
    *   **Zalety:** Dobra stabilność punktu pracy dzięki ujemnemu sprzężeniu zwrotnemu. Prostszy niż układ z dzielnikiem (mniej elementów).
    *   **Wady:** Sprzężenie zwrotne może wpływać na inne parametry wzmacniacza (np. wzmocnienie sygnału zmiennego).
    *   **Obliczenia:** Znów prawa Kirchhoffa. `UCE = IB*RB + UBE` oraz `UCC = (IC+IB)*RC + UCE`. Korzystając z `IC = β*IB`, można wyliczyć prądy i napięcia w punkcie pracy. Wzór `IC = (UCC - UBE) / (RC + RB/β)` pokazuje, że wpływ β na IC jest mniejszy niż w prostym układzie zasilania bazy (gdzie IC byłby wprost proporcjonalny do β).

**5. Funkcje Specjalne w LOGO! (Slajdy 11, ...)**

*   **Co to LOGO!?** To mały, programowalny sterownik logiczny (PLC), często używany w prostych zadaniach automatyki domowej lub przemysłowej. Programuje się go za pomocą bloczków funkcyjnych.
*   **Funkcje specjalne:** To gotowe bloczki realizujące bardziej złożone zadania niż proste bramki AND/OR/NOT, często związane z czasem.
*   **a) Opóźnione wyłączenie (Off-Delay)**
    *   **Symbol:** Bloczek z zegarem, wejście `Trg` (Trigger - wyzwalanie), `R` (Reset), wyjście `Q`.
    *   **Działanie:**
        1.  Gdy na wejście `Trg` podamy sygnał "1" (stan wysoki), wyjście `Q` natychmiast staje się "1".
        2.  Gdy sygnał na `Trg` znika (zmienia się z "1" na "0" - zbocze opadające), bloczek zaczyna odliczać zaprogramowany czas `Ta`.
        3.  Wyjście `Q` pozostaje w stanie "1" przez cały czas odliczania `Ta`.
        4.  Po upływie czasu `Ta`, wyjście `Q` staje się "0".
        5.  Każde kolejne zbocze opadające na `Trg` rozpoczyna odliczanie czasu `Ta` od nowa.
        6.  Podanie sygnału "1" na wejście `R` (Reset) natychmiast zeruje wyjście `Q` i zatrzymuje/zeruje odliczanie czasu `Ta`.
    *   **Przykład:** Światło na klatce schodowej, które gaśnie minutę po naciśnięciu przycisku.
*   **b) Podtrzymane opóźnione załączenie (Retentive On-Delay)**
    *   **Symbol:** Bloczek z zegarem, wejście `Trg`, `R`, wyjście `Q`.
    *   **Działanie:**
        1.  Gdy na wejście `Trg` pojawi się sygnał "1" (zbocze narastające, zmiana z 0 na 1), bloczek zaczyna odliczać zaprogramowany czas `T`.
        2.  Wyjście `Q` pozostaje w stanie "0" podczas odliczania.
        3.  Po upływie czasu `T`, wyjście `Q` staje się "1".
        4.  Co ważne (retentive/podtrzymane): Wyjście `Q` pozostaje w stanie "1" nawet jeśli sygnał na `Trg` zniknie!
        5.  Kolejne impulsy na `Trg` w trakcie odliczania czasu `T` są ignorowane (czas nie jest naliczany od początku).
        6.  Wyjście `Q` można wyłączyć (zrobić "0") tylko podając sygnał "1" na wejście `R` (Reset). Reset działa w każdej chwili (przed, w trakcie, lub po odliczeniu czasu).
    *   **Przykład:** System, który ma uruchomić pompę 30 sekund po naciśnięciu startu, a pompa ma pracować aż do naciśnięcia przycisku stop (Reset).
*   **c) AND z pamięcią stanu (zbocze) (AND with edge detection)**
    *   **Symbol:** Bramka AND ze strzałką w górę przy wejściach (`&↑`).
    *   **Działanie:** Wyjście `Q` staje się "1" tylko wtedy, gdy spełnione są **jednocześnie dwa warunki**:
        1.  Wszystkie wejścia (np. 1, 2, 3, 4) mają w **bieżącym cyklu** programu stan "1".
        2.  **Przynajmniej jedno** z wejść w **poprzednim cyklu** programu miało stan "0" (czyli nastąpiła zmiana z 0 na 1 na co najmniej jednym wejściu, przy jednoczesnym stanie "1" na pozostałych).
    *   **Inaczej mówiąc:** Bloczek ten wykrywa **jednoczesne pojawienie się stanu "1" na wszystkich wejściach**, reagując tylko na "zbocze narastające" tej sytuacji. Jeśli wszystkie wejścia były "1" już w poprzednim cyklu, wyjście pozostanie "0" (lub stanie się "0", jeśli było "1").
    *   **Przykład:** Wykrywanie momentu, gdy wszystkie czujniki bezpieczeństwa maszyny jednocześnie zgłoszą stan OK (przejdą z 0 na 1), aby umożliwić jej start.
