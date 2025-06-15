### Zadania terminalowe (50% punktów)

Zapisz komendy dla poszczególnych operacji z wiersza poleceń. Dołącz do rozwiązania utworzone pliki.

1. Przejdź do katalogu domowego
2. Utwórz katalog `zadanie`
3. Zmień prawa do katalogu `zadanie` tak, aby inni nie mogli go przeglądać
4. Przejdź do katalogu
5. Utwórz plik `produkty.csv`
6. Dodaj nagłówek: `nazwa,cena,ilość`
7. Dodaj dane 4 produktów
8. Wyświetl zawartość pliku
9. Utwórz plik `.archiwum.csv`
10. Pokaż zawartość katalogu, także ukryte pliki
11. Znajdź w `/usr` pliki zawierające `conf` w nazwie
12. Znajdź katalogi z `log` w nazwie w `/`, zapisz do `logs.txt`
13. Skopiuj dane z `produkty.csv` (bez nagłówka), posortuj wg ceny rosnąco, dodaj numerację, zapisz do `.archiwum2.csv`
14. Porównaj pliki `.archiwum.csv` i `.archiwum2.csv`
15. Zamień przecinki w `.archiwum.csv` na spacje
16. `sed`: wyświetl tylko produkty, których cena zawiera cyfrę 9
17. `awk`: wypisz punkty montowania i oblicz sumaryczne użycie i wolne miejsce

---

### Projekt – IPC, Make, GIT (do 50%)

1. Stwórz pliki:

   * `server.h`, `server.c` – logika zarządzania serwerem
   * `client.h`, `client.c` – logika klientów
   * `main.c` – uruchomienie serwera i klientów
   * `readme.md` – imię i nazwisko

2. Napisz `Makefile` z celami:

   * `server`, `client`, `main`, `all`, `clean`

3. Inicjalizuj GIT, dodaj pliki, wykonaj commit

4. Funkcjonalność:

   * Proces główny tworzy 4 klientów: „Anna”, „Paul”, „Rick”, „Nina”
   * Każdy wyświetla komunikat: `"Imię: Client initialized"`
   * Pipe – na „Hello clients! Who are you?” klient odpowiada: `"I am Imię"`
   * Na „Hello clients! Your PID?” odpowiada: `"Imię: PID is ..."`

5. Obsługa sygnałów:

   * `SIGTERM`: `"Imię: Terminating..."`
   * `SIGUSR2`: `"Imię: Acknowledged"`
   * `SIGINT`: `"Imię: Shutting down"` i zakończenie

6. Wykonaj commit: „Projekt gotowy”, wypchnij na GitHub

7. Prześlij link do repozytorium
