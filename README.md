# SnakeGame (C# Console)

Projekt zespołowy – implementacja klasycznej gry Snake w konsoli (C#) z wykorzystaniem GitHub (branching, Pull Requests, Issues).

Repozytorium pokazuje pełny proces pracy zespołowej: podział zadań, osobne gałęzie, code review, merge oraz synchronizację forków.

---

## Funkcje gry

- Klasyczna mechanika Snake:
  - brak przechodzenia przez ściany,
  - kolizja ze ścianą lub wężem kończy grę.
- Jedzenie (`*`):
  - po zjedzeniu wąż rośnie,
  - zwiększany jest wynik (score).
- Tryb dwóch graczy (symulacja współpracy na konsoli):
  - Wąż 1 sterowany strzałkami (`O`),
  - Wąż 2 sterowany klawiszami WASD (`X`),
  - kolizje między wężami powodują zakończenie gry.
- Pauza gry:
  - klawisz `P` zatrzymuje i wznawia rozgrywkę,
  - podczas pauzy wyświetlany jest napis `PAUSED`.

---

## Sterowanie

### Gracz 1
- ↑ ↓ ← → (strzałki)

### Gracz 2
- W – góra  
- S – dół  
- A – lewo  
- D – prawo  

### Dodatkowe
- P – pauza / wznowienie gry

---

## Uruchomienie projektu

1. Sklonuj repozytorium:

2. Otwórz plik:

w Visual Studio.

3. Uruchom projekt:
- klawisz **F5**  
lub  
- przycisk **Run**

---

## Współpraca zespołowa (GitHub workflow)

Projekt realizowany był z wykorzystaniem standardowego workflow GitHub:

### Zasady pracy

- Każda nowa funkcjonalność była tworzona w osobnej gałęzi:
  - `feature/...` – nowe funkcje
  - `fix/...` – poprawki błędów
- Zmiany były wprowadzane do gałęzi `main` wyłącznie przez **Pull Request**.
- Kod był przeglądany w zakładce **Files changed** przed scaleniem.
- Po merge wykonywana była synchronizacja forków (**Sync fork / Pull origin**).

---

## Przykładowe gałęzie użyte w projekcie

- `feature/core-snake`  
  → ruch węża + kolizje ze ścianami  

- `feature/food-score`  
  → jedzenie, wzrost węża, system punktacji  

- `feature/multi-snake`  
  → drugi wąż (WASD), kolizje między wężami  

- `fix/multi-snake-growth`  
  → poprawka błędu wzrostu węży  

- `fix/pause-game`  
  → dodanie pauzy gry  

- `docs/readme`  
  → dokumentacja projektu  

---

## Issues (zarządzanie problemami)

Problemy i nowe funkcje były zgłaszane poprzez system **GitHub Issues**.

Przykłady:

- Bug: oba węże rosły po zjedzeniu jedzenia przez jednego gracza  
- Feature: dodanie pauzy gry  

Każde Issue było rozwiązywane poprzez:

1. Utworzenie osobnej gałęzi  
2. Implementację poprawki  
3. Pull Request  
4. Review  
5. Merge do main  

---

## Technologie

- Język: **C#**
- Typ aplikacji: **Console Application**
- System kontroli wersji: **Git**
- Platforma współpracy: **GitHub**

---

## Autorzy (symulacja zespołu)

Projekt realizowany z użyciem dwóch kont GitHub w celu symulacji pracy zespołowej:

- Konto główne (repozytorium): `chx101878` (sokrum20)
- Konto współpracownika (fork + PR): `bartosz.wiecek` (sokrum)

---

## Status projektu

Projekt ukończony zgodnie z wymaganiami zadania:

- gra Snake działa poprawnie,
- zaimplementowano tryb dwóch graczy,
- zastosowano workflow GitHub (branch + PR + Issues),
- dodano dokumentację.
