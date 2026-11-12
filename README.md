# Sprawa Tupeene'a

Gra na telefony do **Wykładu 5 „Modele warstwowe i protokoły”** z przedmiotu *Architektura systemów telekomunikacyjnych*.

James Bond, Arsène Lupin i Herlock Sholmes raz już zesłali łotra Tupeene'a na bezludną wyspę na Pacyfiku. Teraz Tupeene znalazł tam terminal satelitarny i nęka świat przez sieć. Gracze ścigają go przez kolejne warstwy modelu OSI i zbierają za to **rekomendacje zawodowe**.

## Dla studentów

1. Proszę otworzyć grę w przeglądarce telefonu (adres i kod QR są na ekranie w sali).
2. Proszę wpisać imię lub pseudonim — pojawi się na certyfikacie.
3. Gra ma sześć rozdziałów i 25 zadań. Kolejny rozdział otwiera się po rozwiązaniu wszystkich zadań poprzedniego.
4. Punktacja: poprawna odpowiedź za pierwszym razem — 10 rekomendacji, za drugim — 5, za trzecim — 2. Po trzech błędach Sholmes zdradza odpowiedź.
5. Po ostatnim rozdziale pojawia się **certyfikat rekomendacji** z liczbą punktów i kodem weryfikacyjnym. **Proszę zrobić zrzut ekranu całego certyfikatu** i przekazać go prowadzącemu.

Wolno naradzać się z sąsiadem. Słowniczek pojęć jest pod przyciskiem „Słowniczek”.

Postęp zapisuje się w przeglądarce telefonu, więc po przypadkowym zamknięciu karty można wrócić do gry. W trybie prywatnym przeglądarki postęp może przepaść po zamknięciu karty.

| Rozdział | Temat | Minuty |
|:---|:---|:---:|
| Prolog · Pub nad Tamizą | warstwy, protokół i usługa | 0–3 |
| W7 · Książę z Pacyfiku | warstwa aplikacji: DNS, HTTP, TLS, porty | 3–6 |
| W4 · Uścisk dłoni | warstwa transportowa: TCP, UDP, RTT | 6–9 |
| W3 · Odciski palców w nagłówku | warstwa sieciowa: nagłówek IPv4, TTL, fragmentacja | 9–13 |
| W2 · Fałszywy lokaj | warstwa łącza danych: MAC, ARP, urządzenia | 13–16 |
| Finał · Wyspa w sieci | enkapsulacja, narzut, płaszczyzny, GTP-U | 16–20 |

## Dla prowadzącego

### Tryb rzutnika

Adres gry z dopiskiem `#rzutnik`, np.:

```
https://maciej-janowicz.github.io/sprawa-tupeene/#rzutnik
```

Ten widok pokazuje duży zegar odliczający 20 minut (przycisk **Start śledztwa**), plan rozdziałów z podświetleniem bieżącego oraz sprawdzarkę kodów.

### Sprawdzanie wyników ze zrzutów ekranu

1. W trybie rzutnika, w ramce **Sprawdzenie kodu z certyfikatu**, wpisać **imię** i **liczbę rekomendacji** dokładnie tak, jak widnieją na zrzucie (wielkość liter i spacje na początku i końcu nie mają znaczenia).
2. Porównać wyświetlony kod z kodem na zrzucie.
   - Kody **zgodne** — wynik prawdziwy.
   - Kody **różne** — imię lub liczba punktów na zrzucie zostały zmienione albo przepisane z błędem.

Kod chroni przed poprawieniem liczby na obrazku. Nie jest zabezpieczeniem kryptograficznym: ktoś, kto przeczyta kod źródłowy strony, mógłby go wyliczyć samodzielnie.

### Rangi na certyfikacie

| Wynik | Ranga |
|:---:|:---|
| ≥ 90% | Agent 0x07 z licencją na dekapsulację |
| ≥ 75% | Dżentelmen-włamywacz warstw |
| ≥ 50% | Detektyw nagłówków |
| < 50% | Praktykant Scotland Yardu |

Maksymalnie: **250 rekomendacji**.

## Publikacja na GitHub Pages

1. Utworzyć publiczne repozytorium, np. `sprawa-tupeene`.
2. Wgrać do niego plik `index.html` (i ten `README.md`).
3. **Settings → Pages → Build and deployment:** *Source: Deploy from a branch*, *Branch: main*, folder */ (root)* → **Save**.
4. Po 1–2 minutach gra jest dostępna pod adresem `https://<nazwa-użytkownika>.github.io/sprawa-tupeene/`.

Gra to jeden samodzielny plik HTML. Nie wymaga serwera ani instalacji; z zewnątrz pobiera tylko kroje pisma z Google Fonts (bez nich użyje czcionek systemowych).

## Prywatność

Gra niczego nie wysyła. Imię i postęp są zapisywane wyłącznie w pamięci przeglądarki na urządzeniu gracza (`localStorage`). Prowadzący poznaje wynik tylko wtedy, gdy student sam przekaże zrzut ekranu.

## Autorstwo

Fabuła na motywach opowiadania „Lupin, Bond, and Sholmes debate” z cyklu *Bizarre Stories* Macieja Janowicza. Postać Tupeene'a wymyślił autor opowiadania. Arsène Lupin i Herlock Sholmes to postacie Maurice'a Leblanca, James Bond — Iana Fleminga; występują tu w roli parodystycznej. Treści dydaktyczne odpowiadają wykładowi 5 przedmiotu *Architektura systemów telekomunikacyjnych*.
