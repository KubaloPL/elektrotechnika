**Sterownik Programowalny LOGO! - Uniwersalny mózg dla Twoich urządzeń**

LOGO! to taki uniwersalny "mózg" elektroniczny, stworzony przez firmę Siemens.  Wyobraź sobie, że masz klocki LEGO, ale zamiast budować z nich zamki, budujesz układy sterujące różnymi urządzeniami. LOGO! jest właśnie takim "klockiem" -  ma w sobie wszystko, co potrzebne, żeby sterować prostymi rzeczami w domu, jak i bardziej skomplikowanymi w przemyśle.

**Co LOGO! ma w sobie?**

LOGO! to taki mały komputer, który łączy w sobie różne elementy:

*   **Elementy sterowania:** To po prostu przyciski, przełączniki, które pozwalają Tobie "mówić" LOGO!, co ma robić.
*   **Panel sterowniczy z ekranem:**  Wyświetlacz, na którym LOGO! pokazuje, co robi, i gdzie Ty możesz go programować. Niektóre modele LOGO! nie mają ekranu, ale większość ma.
*   **Zasilacz:**  Czyli to, co daje LOGO! energię do działania, tak jak bateria dla zabawki.
*   **Interfejsy do modułów zewnętrznych:**  Dzięki temu możesz do LOGO! podłączyć dodatkowe "klocki", które rozszerzają jego możliwości, np. więcej wejść i wyjść.
*   **Interfejs do karty pamięci i komputera:**  Możesz użyć karty pamięci, żeby zapisywać programy w LOGO!, a kabel pozwala połączyć LOGO! z komputerem, żeby go programować.
*   **Wbudowane funkcje:**  LOGO! ma już w sobie "wgrane" podstawowe umiejętności, takie jak:
    *   **Opóźnione załączanie/wyłączanie:**  Żeby coś włączyło się lub wyłączyło z opóźnieniem.
    *   **Przekaźnik impulsowy:**  Żeby wysłać krótki impuls sygnału.
    *   **Przełącznik programowalny:**  Żeby LOGO! samo przełączało coś w zależności od programu.
    *   **Timer (zegar):** Żeby LOGO! liczył czas.
*   **Znaczniki stanu (binarne i analogowe):**  To takie "lampki kontrolne" w LOGO!, które pokazują, co się dzieje w programie, czy coś jest włączone, wyłączone, lub jaką ma wartość.
*   **Wejścia i wyjścia:**  To "drzwi i okna" LOGO!. Wejścia to miejsca, gdzie LOGO! "słucha" sygnałów z zewnątrz (np. z czujników, przycisków). Wyjścia to miejsca, gdzie LOGO! "mówi" do urządzeń zewnętrznych (np. włącza światło, steruje silnikiem). Liczba wejść i wyjść zależy od modelu LOGO!.

**Gdzie LOGO! znajdzie swoje miejsce?**

LOGO! jest bardzo wszechstronny i można go używać w wielu miejscach:

*   **Urządzenia domowe:**  Możesz go użyć do sterowania oświetleniem na klatce schodowej, oświetleniem ogrodu, markizami, żaluzjami, oświetleniem wystaw sklepowych - wszędzie tam, gdzie chcesz automatyzacji w domu.
*   **Instalacje elektryczne:**  LOGO! może zastąpić tradycyjne szafki rozdzielcze, upraszczając instalację.
*   **Sterowanie urządzeniami mechanicznymi:**  Możesz go użyć do sterowania bramą wjazdową, klimatyzacją, pompą do wody deszczowej - urządzeniami, które działają mechanicznie.
*   **Specjalistyczne systemy:**  LOGO! jest też używany w szklarniach i cieplarniach do sterowania temperaturą, wilgotnością, oświetleniem.
*   **Przemysł:**  Można go łączyć z modułami komunikacyjnymi (np. ASi), żeby sterować maszynami i procesami w fabrykach, zwłaszcza tam, gdzie sterowanie jest rozproszone, czyli nie wszystko dzieje się w jednym miejscu.

**Wejścia i wyjścia w LOGO! - szczegóły techniczne**

Niezależnie od tego, ile dodatkowych modułów podłączysz, w programie LOGO! zawsze masz do dyspozycji:

*   **Wejścia binarne (I):** Od I1 do I24. Wejścia binarne przyjmują tylko dwa stany: włączone lub wyłączone (prawda lub fałsz). Myśl o nich jak o przyciskach - naciśnięty (1) lub nie naciśnięty (0).
*   **Wejścia analogowe (AI):** Od AI1 do AI8. Wejścia analogowe mogą przyjmować wartości z zakresu, np. temperaturę, napięcie. Myśl o nich jak o pokrętle, które możesz ustawić na różnych wartościach.
*   **Wyjścia binarne (Q):** Od Q1 do Q16. Wyjścia binarne sterują urządzeniami, które też mają tylko dwa stany: włączone lub wyłączone (np. światło, przekaźnik).
*   **Wyjścia analogowe (AQ):** AQ1 i AQ2.  Wyjścia analogowe mogą "wypuszczać" sygnały o zmiennej wartości, np. sterować jasnością światła, prędkością silnika.
*   **Bity rejestru przesuwnego (S):** Od S1 do S8. To taka wewnętrzna "pamięć" w LOGO!, gdzie możesz przechowywać informacje w postaci bitów, które można przesuwać.
*   **Klawisze kursora (4):**  Na panelu LOGO! masz 4 strzałki, które pomagają Ci poruszać się po menu i programować.
*   **Wyjścia wirtualne (X):** Od X1 do X16. To takie "wyjścia" tylko w programie, nie ma ich fizycznie na LOGO!. Możesz ich używać w programie, żeby organizować logikę, ale nie sterują one bezpośrednio urządzeniami.
*   **Bloki znaczników binarnych stanu (M):** Od M1 do M24.  Kolejne "lampki kontrolne" w programie, binarne, czyli włączone/wyłączone.
*   **Bloki znaczników analogowych stanu (AM):** Od AM1 do AM6. Analogiczne "lampki kontrolne", ale pokazujące wartości analogowe.

**Tryby Pracy LOGO! - STOP i RUN**

LOGO! ma dwa główne tryby pracy:

*   **STOP:**
    *   Na ekranie (jeśli jest) wyświetla się "No program" (jeśli nie ma programu) lub coś innego, w zależności od modelu.
    *   LOGO! jest w trybie programowania - możesz go programować, zmieniać ustawienia.
    *   Lampka na LOGO! (dioda) świeci na czerwono (tylko w modelach bez ekranu).
    *   **Działanie LOGO! w trybie STOP:**
        *   Nie odczytuje stanów wejść - ignoruje to, co się dzieje na wejściach.
        *   Program nie jest wykonywany - LOGO! nic nie robi, tylko czeka na programowanie.
        *   Przekaźniki wewnątrz LOGO! są rozwarte (wyłączone), a tranzystory wyjściowe są wyłączone - nic nie jest sterowane na wyjściach.

*   **RUN:**
    *   Na ekranie wyświetla się monitor stanów wejść i wyjść oraz różne komunikaty z menu.
    *   LOGO! jest w trybie modyfikacji parametrów - możesz zmieniać niektóre ustawienia programu.
    *   Lampka na LOGO! świeci na zielono (tylko w modelach bez ekranu).
    *   **Działanie LOGO! w trybie RUN:**
        *   Odczytuje stany wejść - LOGO! "słucha" tego, co dzieje się na wejściach.
        *   Wykonuje program i oblicza stany wyjść - LOGO! robi to, co mu zaprogramowałeś.
        *   Włącza lub wyłącza wyjściowe przekaźniki lub tranzystory - steruje urządzeniami podłączonymi do wyjść, zgodnie z programem.

**Konektory LOGO! - jak podłączyć sygnały**

"Konektor" to takie ogólne słowo na wszystkie połączenia i miejsca, gdzie podłączasz sygnały w LOGO!.  Stan logiczny wejścia/wyjścia jest opisany jako 0 lub 1:

*   **Stan 0:**  Brak napięcia na danym wejściu. LOGO! rozumie to jako "wyłączone", "nieaktywne", "fałsz".
*   **Stan 1:**  Jest napięcie na danym wejściu. LOGO! rozumie to jako "włączone", "aktywne", "prawda".

**Oznaczenia "hi" i "lo"**

Żeby programowanie było łatwiejsze, konektory są oznaczane jako "hi" i "lo":

*   **"hi" (high - wysoki poziom napięcia):** Odpowiada stanowi logicznemu **1**. Czyli "jest napięcie", "włączone".
*   **"lo" (low - niski poziom napięcia):** Odpowiada stanowi logicznemu **0**. Czyli "brak napięcia", "wyłączone".

Nie musisz zawsze używać wszystkich konektorów w bloku funkcyjnym.  Jeśli jakiegoś konektora nie użyjesz, program LOGO! sam ustawi mu taki stan (0 lub 1), żeby blok działał poprawnie.

**Bloki w LOGO! - podstawowe funkcje**

"Blok" w LOGO! to taka podstawowa funkcja, która przetwarza sygnał wejściowy na wyjściowy.  Bez LOGO!, żeby zrobić to samo, musiałbyś łączyć kable w szafce sterowniczej. LOGO! ułatwia to, bo programujesz przez łączenie bloków na ekranie.

Programowanie LOGO! polega na łączeniu bloków ze sobą. Wybierasz połączenie z menu "Co" (od "Connector").

**Podstawowe bloki logiczne (funkcje podstawowe):**

*   **AND (I):**  "I" logiczne. Wyjście bloku będzie "1" (prawda) tylko wtedy, gdy **wszystkie** wejścia są "1" (prawda). Jakbyś miał kilka wyłączników światła połączonych szeregowo - światło zaświeci się tylko wtedy, gdy wszystkie są włączone.
*   **OR (LUB):** "LUB" logiczne. Wyjście bloku będzie "1" (prawda), gdy **przynajmniej jedno** wejście jest "1" (prawda).  Jakbyś miał kilka wyłączników światła połączonych równolegle - światło zaświeci się, gdy włączysz którykolwiek z nich.
*   **itp.:**  Jest więcej podstawowych funkcji logicznych, np. NAND, NOR, XOR, NOT (o nich za chwilę).

**Przykład bloku OR:**

Na rysunku masz blok OR (≥1). Wejścia I1 i I2 są podłączone do bloku. Pozostałe dwa wejścia (oznaczone "x") są nieużywane i LOGO! ustawi dla nich taki stan, żeby nie przeszkadzały w działaniu bloku OR.

**Funkcje specjalne - więcej możliwości!**

Oprócz podstawowych bloków logicznych, LOGO! ma też bardziej zaawansowane funkcje specjalne:

*   **Przerzutnik bistabilny:**  Zapamiętuje stan (włączony/wyłączony) nawet po zaniku sygnału.
*   **Licznik wzrastający/malejący:**  Liczy impulsy, może liczyć w górę lub w dół.
*   **Włącznik czasowy:**  Włącza coś na określony czas.
*   **Przełącznik wciskowy:**  Działa jak przycisk - włącza coś tylko na czas wciśnięcia.
*   **Przełącznik wielofunkcyjny:**  Może działać na różne sposoby, w zależności od ustawień.
*   **Generator losowy:**  Generuje losowe sygnały.
*   **Opóźnione wyłączenie:**  Wyłącza coś z opóźnieniem.
*   **Podtrzymane opóźnione załączenie:**  Włącza coś z opóźnieniem, ale "pamięta" impuls wejściowy.

**Wyświetlanie bloków w LOGO!**

Ekran LOGO! pokazuje bloki graficznie.  Na ekranie widzisz typowy widok bloku, z wejściami po lewej, wyjściem po prawej i symbolem funkcji w środku.

Jednocześnie na ekranie może być wyświetlony tylko jeden blok.  Dlatego bloki są numerowane, żeby łatwiej było budować program i wiedzieć, jak są połączone.

**Numeracja bloków - porządek w programie**

Kiedy dodajesz nowy blok do programu, LOGO! automatycznie nadaje mu numer. Te numery pokazują, jak bloki są połączone ze sobą. Dzięki numerom łatwiej jest kontrolować program i wiedzieć, co jest z czym połączone.

**Przykład numeracji:**

Na rysunku widzisz trzy widoki ekranu LOGO!, które razem tworzą jeden program.  Bloki są ponumerowane (B1, B2, B3). Strzałki i numery bloków pokazują, że wyjście bloku B1 jest połączone z wejściem bloku B3.  Dzięki numeracji łatwo śledzić połączenia, nawet jeśli program jest rozbudowany.

**Reprezentacja obwodu na schemacie połączeń**

Możesz przedstawić obwód sterowania na tradycyjnym schemacie elektrycznym, a potem przenieść go na program w LOGO! za pomocą bloków i konektorów.

**Przykład - obwód światła sterowanego przełącznikami:**

Na schemacie masz obciążenie E1 (np. lampę), które jest włączane/wyłączane przez układ przełączników S1, S2 i S3.  Lampa zaświeci się, jeśli (S1 LUB S2) I S3 jest zamknięte.

**Realizacja schematu w LOGO!:**

W LOGO! projektujesz program, łącząc bloki i konektory, tak jakbyś budował obwód elektryczny.

**Program działania LOGO! dla tego przykładu:**

Na rysunku widzisz program w LOGO!, który realizuje ten sam obwód co na schemacie elektrycznym.  Użyto bloków OR (≥1) i AND (&). Wejścia I1 i I2 odpowiadają przełącznikom S1 i S2, wejście I3 odpowiada przełącznikowi S3, a wyjście Q1 steruje przekaźnikiem, który włącza lampę.

**Wskazówka programowania:**

W programowaniu LOGO! najlepiej zacząć od wyjścia - czyli od tego, co chcesz sterować (np. lampa, przekaźnik). Potem "cofaj się" w programie, dodając bloki i wejścia, które sterują tym wyjściem.

**Listy funkcji LOGO! - porządek w funkcjach**

W programowaniu LOGO! masz dostęp do różnych elementów i funkcji, które są ułożone w listy:

*   **↓Co - lista konektorów (Connector):**  Lista wejść, wyjść, znaczników stanu, itp. - czyli wszystkich "punktów" do podłączania sygnałów.
*   **↓GF - lista funkcji podstawowych (Grundfunktionen - Basic Functions):** Lista podstawowych bloków logicznych: AND, OR, NAND, NOR, XOR, NOT.
*   **↓SF - lista funkcji specjalnych (Sonderfunktionen - Special Functions):** Lista bardziej zaawansowanych funkcji: timery, liczniki, przerzutniki, itp.
*   **↓BN - lista bloków użytych w programie (Block Number):** Lista bloków, które już dodałeś do programu.

**Lista funkcji podstawowych (GF) - szczegółowo**

Funkcje podstawowe to proste operacje logiczne, tak jak w algebrze Boole'a.

**Możliwość negacji sygnału:**  Możesz "zanegować" sygnał na wejściu bloku specjalnego.  Wtedy, jeśli na wejście przyjdzie "1", blok potraktuje to jako "0", i odwrotnie.

**Funkcje podstawowe - tabela:**

Tabela pokazuje symbole funkcji podstawowych na schematach elektrycznych i w LOGO!, oraz ich nazwy:

*   **AND:**  Szeregowe połączenie styków zwiernych.
*   **AND z pamięcią stanu (zbocze):** Specjalna wersja AND, która reaguje na zmianę stanu wejścia.
*   **NAND (NOT AND):** Negacja funkcji AND.
*   **NAND (NOT AND) z pamięcią stanu (zbocze):** Negacja AND z pamięcią stanu.
*   **OR:** Równoległe połączenie styków zwiernych.
*   **NOR (NOT OR):** Negacja funkcji OR.
*   **XOR (nierównoważność):** Wyjście "1", gdy wejścia są różne.
*   **NOT (Negacja, Inwerter):**  Odwraca stan wejścia - "1" zamienia na "0", "0" na "1".
*   **Podwójny styk przełączny:** Specjalny styk, który ma dwa wyjścia.
*   **Styk rozwierny:**  Działa odwrotnie niż styk zwierny - normalnie jest zamknięty, a otwiera się po zadziałaniu.

**AND z pamięcią stanu (zbocze) - przykład i wykres**

Funkcja "AND z pamięcią stanu (zbocze)" jest trochę bardziej skomplikowana.  Reaguje ona na zbocze narastające (zmianę stanu z 0 na 1) na wejściu.

**Wykres czasowy:**

Wykres pokazuje, jak sygnały na wejściach (1, 2, 3, 4) i wyjściu (Q) bloku AND z pamięcią stanu zmieniają się w czasie.

**Działanie:**

Wyjście bloku AND z pamięcią stanu przyjmuje stan "1", jeśli:
1.  Stany na **wszystkich** wejściach (1, 2, 3, 4) są "1".
2.  **Przynajmniej jedno** wejście w poprzednim cyklu miało stan "0".

Czyli, żeby wyjście było "1", wszystkie wejścia muszą być "1", a dodatkowo blok "pamięta", że wcześniej na jakimś wejściu był stan "0". To jest funkcja, która reaguje na zmianę stanu wejść, a nie tylko na ich aktualny stan.

**Bloki funkcji specjalnych (SF) - funkcje czasowe**

Funkcje specjalne to bardziej zaawansowane bloki, np. timery, liczniki.  Wykład skupia się na funkcjach czasowych.

**Tabela funkcji czasowych:**

Tabela pokazuje funkcje czasowe dostępne w LOGO!, ich oznaczenia w LOGO!, nazwy i oznaczenie "REM" (prawdopodobnie od "REMote" - zdalne sterowanie/monitorowanie, ale nie jest to wprost wyjaśnione w tekście).

*   **Opóźnione włączenie (Opóźnienie włączenia):** Włącza wyjście z opóźnieniem.
*   **Opóźnione wyłączenie (Opóźnienie wyłączenia):** Wyłącza wyjście z opóźnieniem.
*   **Opóźnione włącz/wyłącz (Opóźnione załącz/wyłącz):**  Może działać jako opóźnione włączanie lub wyłączanie, w zależności od ustawień.
*   **Opóźnienie z podtrzymaniem (Opóźnienie z podtrzymaniem):**  Włącza z opóźnieniem, ale "pamięta" impuls wejściowy i trzyma wyjście włączone, dopóki nie pojawi się sygnał resetu.
*   **Przekaźnik czasowy z wyjściem impulsowym (Przekaźnik czasowy z wyjściem impulsowym):** Generuje impuls na wyjściu o określonym czasie trwania.

**Opóźnione włączenie - szczegółowo**

**Działanie:** Wyjście bloku staje się "1" dopiero po upływie zadanego czasu.

**Opis konektorów:**

*   **Trg (Trigger):**  Wejście wyzwalające. Odliczanie czasu zaczyna się, gdy na wejściu Trg pojawi się zbocze narastające (zmiana stanu z 0 na 1).
*   **Par (Parameter):**  Parametr czasu. Ustawiasz czas (T), po którym wyjście ma się włączyć.
*   **Q (Output):** Wyjście. Stan wyjścia zmienia się z 0 na 1 po upływie czasu T, jeśli na wejściu Trg nadal jest "1".

**Wykres czasowy:**

Wykres pokazuje, jak sygnały na wejściu Trg i wyjściu Q zmieniają się w czasie.  Pogrubiony fragment wykresu jest też pokazany na symbolu bloku w LOGO!.

**Zmiana stanu na wejściu Trg:**  Zmiana stanu Trg z 0 na 1 rozpoczyna odliczanie czasu Ta (czas roboczy LOGO!).

**Warunek włączenia wyjścia:** Jeśli na wejściu Trg stan "1" trwa wystarczająco długo (przynajmniej tyle, ile wynosi zadany czas T), to po upływie czasu T wyjście Q staje się "1".

**Przerwanie odliczania:** Jeśli wejście Trg wróci do stanu "0" zanim upłynie czas T, odliczanie czasu jest przerwane.

**Zerowanie wyjścia:** Wyjście Q wraca do "0", gdy wejście Trg wróci do stanu "0".

**Brak podtrzymania pamięci:**  Jeśli nie jest włączona opcja podtrzymania pamięci, przerwa w zasilaniu LOGO! spowoduje wyzerowanie wyjścia Q i reszty odliczanego czasu.

**Opóźnione wyłączenie - szczegółowo**

**Działanie:** Wyjście bloku staje się "0" po upływie zadanego czasu.

**Opis konektorów:**

*   **Trg (Trigger):** Wejście wyzwalające. Pojawienie się stanu wysokiego (zmiana z 0 na 1) na wejściu Trg powoduje wzbudzenie wyjścia Q (wyjście staje się "1").
*   **R (Reset):** Wejście zerujące. Zeruje wyjście Q i czas Ta.
*   **Q (Output):** Wyjście.

**Wykres czasowy:**

Wykres pokazuje, jak sygnały na wejściach Trg, R i wyjściu Q zmieniają się w czasie.

**Zmiana stanu na wejściu Trg:** Zmiana stanu Trg z 1 na 0 powoduje rozpoczęcie odliczania czasu Ta. Wyjście Q pozostaje "1" w czasie odliczania.

**Wyzerowanie wyjścia:** Gdy czas Ta osiągnie wartość T (ustawioną), wyjście Q staje się "0".

**Zbocze opadające na Trg:** Każde zbocze opadające (zmiana z 1 na 0) na wejściu Trg powoduje ponowne rozpoczęcie odliczania czasu od początku.

**Wejście zerujące R:** Wejście R służy do natychmiastowego wyzerowania wyjścia Q i czasu Ta, nawet jeśli czas T jeszcze nie upłynął.

**Opóźnienie z podtrzymaniem - szczegółowo**

**Działanie:** Impuls na wejściu Trg rozpoczyna odliczanie czasu. Wyjście włącza się po upływie zadanego czasu i pozostaje włączone, dopóki nie zostanie zresetowane.

**Opis konektorów:**

*   **Trg (Trigger):** Wejście wyzwalające. Impuls na wejściu Trg rozpoczyna odliczanie czasu.
*   **R (Reset):** Wejście resetujące. Zeruje wyjście Q i czas Ta.
*   **Q (Output):** Wyjście.

**Wykres czasowy:**

Wykres pokazuje, jak sygnały na wejściach Trg, R i wyjściu Q zmieniają się w czasie.

**Zmiana stanu na wejściu Trg:** Zmiana stanu Trg z 0 na 1 powoduje rozpoczęcie odliczania czasu Ta. Po upływie czasu Ta=T, wyjście Q staje się "1". Dalsze zmiany stanu na wejściu Trg nie mają wpływu na odliczanie czasu Ta.

**Wyzerowanie wyjścia:** Wyjście Q i odliczany czas Ta są zerowane, gdy na wejściu R pojawi się sygnał "1".

**Przekaźnik czasowy z wyjściem impulsowym - szczegółowo**

**Działanie:** Sygnał na wejściu Trg generuje na wyjściu Q impuls o określonym czasie trwania.

**Opis konektorów:**

*   **Trg (Trigger):** Wejście wyzwalające. Sygnał na wejściu Trg generuje impuls na wyjściu.
*   **Par (Parameter):** Parametr czasu. Ustawiasz czas trwania impulsu (T).
*   **Q (Output):** Wyjście. Generuje impuls.

**Wykres czasowy:**

Wykres pokazuje, jak sygnały na wejściu Trg i wyjściu Q zmieniają się w czasie.

**Zmiana stanu na wejściu Trg:** Zmiana stanu Trg z 0 na 1 powoduje wzbudzenie wyjścia Q (staje się "1") i rozpoczęcie odliczania czasu Ta (czas trwania impulsu).

**Czas trwania impulsu:** Wyjście Q pozostaje "1" przez czas Ta. Gdy czas Ta osiągnie wartość T (zadaną długość impulsu), wyjście Q wraca do stanu "0".

**Przerwanie impulsu:** Jeśli przed upływem czasu T wejście Trg zmieni stan z 1 na 0, wyjście Q natychmiast wraca do stanu "0".

**Przykłady zastosowań LOGO! - Drzwi i Brama automatyczna**

Wykład kończy się dwoma przykładami zastosowań LOGO!: drzwi automatyczne i brama automatyczna.  Pokazane są schematy elektryczne tradycyjnych rozwiązań i schematy blokowe implementacji tych rozwiązań w LOGO!.

**Przykład 1: Drzwi automatyczne**

**Wymagania:**

*   Drzwi mają się otwierać automatycznie, gdy ktoś się zbliża.
*   Drzwi mają pozostać otwarte, dopóki ktoś jest w przejściu.
*   Drzwi mają się automatycznie zamknąć po krótkim czasie, gdy przejście jest puste.

**Rozwiązanie klasyczne (schemat elektryczny):**

Schemat pokazuje czujniki ruchu (B1, B2), przekaźniki (K1, K2, K3, K4) i obwody sterowania silnikiem drzwi.

**Schemat blokowy LOGO! - konwencjonalny i uproszczony:**

Pokazane są dwa schematy blokowe w LOGO! - jeden bardziej złożony, a drugi uproszczony, wykorzystujący funkcje specjalne (opóźnione wyłączenie).  Uproszczony schemat jest bardziej przejrzysty i efektywny.

**Przykład 2: Brama automatyczna**

**Schemat elektryczny i schemat blokowy LOGO!:**

Podobnie jak w przykładzie z drzwiami, pokazane są schematy elektryczne i blokowe LOGO! dla bramy automatycznej.  Schematy uwzględniają przyciski "otwieranie", "zamykanie", "stop", czujniki otwarcia i zamknięcia bramy, czujnik bezpieczeństwa i światło ostrzegawcze.

Schematy blokowe LOGO! pokazują, jak za pomocą bloków logicznych i czasowych można zrealizować sterowanie bramą, uwzględniając wszystkie wymagania bezpieczeństwa i funkcjonalności.

Mam nadzieję, że to streszczenie jest zrozumiałe i pomocne!
