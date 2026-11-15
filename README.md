# Integrator TomarLublin – wydania programu na Windows

Publiczne repozytorium z gotowymi wersjami programu **Synchronizacja** (Windows). Kodu źródłowego tu nie ma (jest
w prywatnym repozytorium `Integrator-TomarLublin-Zrodlo`, folder `desktop/`). Pliki są w zakładce
**[Releases](../../releases)**.

- Tagi: `v2.3.0` (oficjalne), `v2.2.5.4` (czwarty człon = wersja testowa/beta, oznaczona jako pre-release).
- Każde wydanie: `Synchronizacja-X.zip`, `wersja.json` (numer, suma kontrolna, ewentualny podpis), `opis.md`.
- Publikuje automat **Windows: wydanie** z repozytorium kodu.

## Jak program się aktualizuje

Program pobiera listę wydań tego repozytorium i wybiera najwyższą wersję z tagiem `v…` i plikiem `wersja.json`
(wersje testowe tylko na komputerach z włączonym kanałem beta). Starsze wersje programu (przed 2.3.0) biorą
najnowsze wydanie (`/releases/latest`), dlatego oficjalne wydania mają flagę „najnowsze”.

## Instalacja

Pobierz `Synchronizacja-X.zip` z [najnowszego wydania](../../releases/latest), rozpakuj i uruchom
`Synchronizacja.exe`. Kolejne wersje program zainstaluje sam.

## Historia

Do 15.11.2026 repozytorium nazywało się `synchronizacja-wydania`, a potem przez chwilę `Integrator-TomarLublin-Wydania`
(wspólne z Androidem). GitHub przekierowuje stare nazwy, więc starsze wersje programu dalej znajdują aktualizacje.
Wydania aplikacji na Androida są w `Integrator-TomarLublin-Wydania-Android`.
