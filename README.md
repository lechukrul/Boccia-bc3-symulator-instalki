# Symulator bocci BC3

## Pobieranie

**[➜ Pobierz najnowszą wersję](https://github.com/lechukrul/Boccia-bc3-symulator-instalki/releases/latest)** — na stronie wydania, w sekcji „Assets”, wybierz plik dla swojego systemu:

| System | Plik |
|---|---|
| Windows | `Symulator-bocci-BC3-…-win-x64.exe` |
| macOS | `Symulator-bocci-BC3-…-mac-universal.dmg` |
| Ubuntu, Debian, Mint | `Symulator-bocci-BC3-…-linux-amd64.deb` |
| inne Linuxy | `Symulator-bocci-BC3-…-linux-x86_64.AppImage` |

Symulator 3D do treningu bocci w kategorii BC3 (gra z rampą). Nie wyrzuca się bili
ręką: ustawia się rampę i puszcza bilę z wybranej wysokości rynny, a dalej bila
toczy się po parkiecie i zderza z innymi bilami według fizyki.

Program działa bez internetu i bez zakładania konta. Wszystkie ustawienia
(zestaw bil, pomiary kalibracji, wyniki ćwiczeń) zapisują się na Twoim komputerze.

## Instalacja

Program nie ma płatnego podpisu cyfrowego, więc system przy pierwszym
uruchomieniu ostrzeże, że aplikacja pochodzi od nieznanego wydawcy. To normalne.

### Windows

1. Uruchom plik `Symulator-bocci-BC3-…-win-x64.exe`.
2. Jeśli pojawi się niebieskie okno „System Windows ochronił ten komputer”,
   kliknij **Więcej informacji** → **Uruchom mimo to**.
3. Przejdź przez instalator. Symulator uruchomisz skrótem na pulpicie
   „Symulator bocci BC3”.

### macOS

1. Otwórz plik `Symulator-bocci-BC3-…-mac-universal.dmg` i przeciągnij ikonę
   symulatora do folderu **Aplikacje**.
2. Uruchom symulator z Aplikacji. System go zablokuje — kliknij **Gotowe**.
3. Wejdź w **Ustawienia systemowe → Prywatność i ochrona**, przewiń w dół
   i przy komunikacie o symulatorze kliknij **Otwórz mimo to**, potem potwierdź.
   Od tej pory program uruchamia się normalnie.

Jeśli macOS pisze, że aplikacja „jest uszkodzona”, otwórz Terminal i wpisz:

    xattr -cr "/Applications/Symulator bocci BC3.app"

### Linux

- **Ubuntu, Debian, Mint:** zainstaluj plik `.deb` (dwuklik albo
  `sudo apt install ./Symulator-bocci-BC3-…-linux-amd64.deb`). Symulator pojawi
  się w menu aplikacji.
- **Inne dystrybucje:** pobierz plik `.AppImage`, nadaj mu prawo uruchamiania
  (Właściwości → „Pozwól na uruchamianie jako program” albo
  `chmod +x Symulator-bocci-BC3-*.AppImage`) i uruchom go.

## Jak działa symulator

Cały program obsługuje się **przyciskami na pasku na dole ekranu** — wystarczy
myszka (zawodnik, dla którego powstał, steruje myszką za pomocą głowy).
Klawiatura nie jest potrzebna.

**Rzut**

1. **Ustaw rampę w polu wyrzutu** — „pozycja statywu” (strzałki) przesuwa
   rampę, „obrót statywu” obraca całą rampę, a „obrót dzioba” kręci samą rynną
   (podstawa stoi, wylot zatacza łuk). Kliknięcie to mały krok, przytrzymanie
   przycisku — ruch ciągły, który powoli przyspiesza.
2. **Wybierz dostawki** (1–3) — im dłuższa rampa, tym mocniej można rzucić.
3. **Wybierz punkt puszczenia** — oznaczenia na rynnie (dziób 1–10, A–D,
   „prawie góra”, „góra”, na dostawce 1–9, A–C). Wyżej = szybciej i dalej.
4. **Wybierz bilę** — kolor (czerwona / niebieska / jack) i konkretną bilę
   z zestawu. Bile różnią się twardością (od super miękkiej do super twardej),
   co zmienia toczenie i zderzenia — miękką bilę mocny rzut potrafi przeskoczyć.
5. Kliknij czerwony przycisk **PUŚĆ BILĘ**.

Panel po prawej pokazuje ustawienie rampy, wybraną bilę i odległości bil
od jacka.

**Kamera** — „zza rampy” (jak widzi zawodnik), „z góry” albo „swobodna”;
strzałki przesuwają widok, „+” i „−” przybliżają. „Podgląd jacka” po rzucie
pokazuje w rogu ekranu okolicę jacka z góry.

**Tryby gry**

- **Trening** (start programu) — rzucasz dowolnie wiele bil; „cofnij bilę”
  zdejmuje ostatnią, „wyczyść” — wszystkie.
- **Mecz** — 4 endy, dwie rampy (czerwona i niebieska), jedna osoba rzuca za
  obie strony. Program pilnuje kolejki (rzuca strona dalsza od jacka) i po
  każdym rzucie pokazuje, jaki byłby wynik endu.
- **Perfekty** — ćwiczenie: jack i jedna bila, celem jest położyć ją tuż przy
  jacku tak, żeby zasłonić go przeciwnikowi. Każdy rzut dostaje ocenę w %.

**Zestaw bil i kalibracja**

- „Zestaw bil” — tu nadajesz nazwy swoim 13 bilom i ustawiasz ich twardość.
- „Kalibracja” — dla symulowania własnych bil: rzucasz prawdziwą bilą
  z danego punktu rampy i wskazujesz w programie, gdzie się zatrzymała.
  Symulator dopasowuje do tego toczenie tej bili. Bez kalibracji działają
  ustawienia domyślne.
- Zestaw, pomiary i wyniki ćwiczeń można zapisać do pliku i wczytać na innym
  komputerze.
