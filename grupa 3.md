### Zadania terminalowe (50% punktów)

Zapisz komendy dla poszczególnych operacji z wiersza poleceń. Dołącz do rozwiązania utworzone pliki.

1. Przejdź do katalogu domowego
2. Utwórz katalog `raporty`
3. Ustaw prawa dostępu do katalogu `raporty`, tak aby inni użytkownicy nie mieli żadnych uprawnień
4. Przejdź do katalogu `raporty`
5. Utwórz plik `statystyki.csv`
6. Dodaj nagłówek: `miasto,populacja,rok`
7. Dodaj dane dla czterech miast (w tym jedno z Twojego regionu), rozdzielone przecinkami
8. Wyświetl zawartość pliku
9. Utwórz ukryty plik `.archiwum_statystyk.csv`
10. Pokaż zawartość katalogu, w tym ukryte pliki
11. Wyszukaj w katalogu `/etc` pliki zawierające `net` w nazwie
12. Znajdź katalogi w `/` zawierające `log` w nazwie i zapisz wynik do pliku `logdirs.txt`
13. Skopiuj dane z `statystyki.csv` (bez nagłówka) do `.archiwum_statystyk.csv`, posortuj alfabetycznie po nazwie miasta, dodaj numerację i zapisz jako `.archiwum_statystyk2.csv`
14. Porównaj oba pliki `.archiwum_statystyk*`
15. Zamień w `.archiwum_statystyk.csv` przecinki na spacje
16. `sed`: wypisz tylko miasta, których populacja zawiera cyfrę `8`
17. `awk`: wypisz punkty montowania i pokaż dostępne oraz zajęte miejsce, w ostatnim wierszu pokaż sumy

---

### Projekt – Make, IPC, sygnały, GIT (max. 50%)

1. Stwórz projekt z plikami:

   * `coordinator.h`, `coordinator.c` – logika koordynatora
   * `agent.h`, `agent.c` – logika agentów
   * `main.c` – uruchomienie procesu
   * `readme.md` – Twoje imię i nazwisko

2. Zbuduj `Makefile` z celami:

   * `coordinator` – biblioteka z `coordinator.c`
   * `agent` – biblioteka z `agent.c`
   * `main` – kompilacja `main.c` i utworzenie programu `koordynator`
   * `all` – buduje wszystko
   * `clean` – usuwa pliki binarne i obiekty

3. Zainicjuj repozytorium GIT, dodaj pliki, wykonaj pierwszy commit

4. Funkcjonalność programu:

   * Koordynator tworzy 4 agentów: „Gamma”, „Beta”, „Alpha”, „Delta”
   * Każdy agent wyświetla po uruchomieniu: `"Imię agenta: Gotowy do misji"`
   * Nienazwany potok:

     * Na „Identify!” agent odpowiada: `"My codename is Imię"`
     * Na „Status?” agent odpowiada: `"Imię: My PID is: ..." `

5. Obsługa sygnałów:

   * `SIGUSR1`: `"Imię: Czekam na rozkazy"`
   * `SIGUSR2`: `"Imię: Rozpoczynam misję"`
   * `SIGTERM`: `"Imię: Misja zakończona"` i zakończenie procesu

6. Wykonaj commit z komunikatem: `Projekt zakończony`, wypchnij repozytorium na GitHub

7. Prześlij link do repozytorium publicznego
