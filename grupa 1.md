### Zadania terminalowe (50% punktów)

Zapisz komendy dla poszczególnych operacji z wiersza poleceń. Dołącz do rozwiązania utworzone pliki.

1. Przejdź do katalogu domowego
2. Utwórz katalog `egzamin`
3. Zabierz innym użytkownikom wszystkie prawa do katalogu `egzamin`, pozostawiając je tylko właścicielowi
4. Przejdź do katalogu `egzamin`
5. Utwórz plik `pracownicy.csv`
6. Dodaj nagłówek: `id,imię,nazwisko,stanowisko`
7. Dodaj dane czterech pracowników (w tym siebie jako pierwszego)
8. Wyświetl zawartość pliku
9. Utwórz ukryty plik `.backup.csv`
10. Wyświetl wszystkie pliki w katalogu, w tym ukryte
11. Znajdź wszystkie pliki w `/var` zawierające w nazwie `log`
12. Wyszukaj w całym systemie katalogi zawierające `lib` i zapisz je do `libs.txt`
13. Skopiuj dane z `pracownicy.csv` (bez nagłówka) do `.backup.csv`, posortuj alfabetycznie po nazwisku i dodaj numerację. Zapisz do pliku `.backup2.csv`
14. Porównaj `.backup.csv` i `.backup2.csv`
15. Zastąp przecinki w `.backup.csv` średnikami
16. Użyj `sed`, aby wyświetlić tylko te osoby, których stanowisko zawiera słowo „inżynier”
17. Użyj `awk`, aby podsumować zajętość wszystkich punktów montowania (kolumny `Used` i `Available`) z polecenia `df`

---

### Projekt – IPC, Make, GIT (do 50%)

1. Stwórz projekt z plikami:

   * `manager.h` i `manager.c` – zarządzanie zespołem
   * `worker.h` i `worker.c` – implementacja zadań pracowników
   * `main.c` – punkt startowy programu
   * `readme.md` – Twoje imię i nazwisko

2. Napisz `Makefile`, który:

   * Kompiluje `manager.c` do biblioteki `libmanager.a`
   * Kompiluje `worker.c` do biblioteki `libworker.a`
   * Łączy `main.c` w program `projekt`
   * Zawiera cele: `manager`, `worker`, `main`, `all`, `clean`

3. Inicjalizuj GIT, dodaj pliki, wykonaj commit

4. Funkcjonalność:

   * Proces główny tworzy 4 procesy z nazwami „Alice”, „Bob”, „Eve”, „Tom”
   * Każdy wyświetla po uruchomieniu: `"Imię: Gotowy do pracy"`
   * Komunikacja przez pipe – na komendę „Podaj imię” wyświetla: `"My name is Imię"`
   * Komenda „PID?” – `"Imię: My PID is ..."`

5. Obsługa sygnałów w dzieciach:

   * `SIGHUP`: `"Imię: Odpoczywam"`
   * `SIGUSR1`: `"Imię: Startuję!"`
   * `SIGINT`: `"Imię: Kończę"` i zakończenie procesu

6. Wykonaj commit z komentarzem „Ukończono projekt”, wypchnij na GitHub

7. Prześlij link do publicznego repozytorium