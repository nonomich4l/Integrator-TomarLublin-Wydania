# Wydania programów TomarLublin

Publiczne repozytorium z gotowymi do pobrania wersjami programów. Kodu źródłowego tu nie ma (jest w prywatnych
repozytoriach). Pliki są w zakładce **[Releases](../../releases)**.

| Program | Tagi wydań | Plik | Pobieranie |
|---|---|---|---|
| **Synchronizacja** (Windows) | `v2.2.4`, `v2.2.5.4` (czwarty człon = wersja testowa/beta) | `Synchronizacja-X.zip` + `wersja.json` | [najnowsza](../../releases/latest) |
| **Integrator** (Android 8.0+) | `android-v1.0.1` | `Integrator-TomarLublin-X.apk` | lista [Releases](../../releases), szukaj „Android” |

## Jak programy się aktualizują

- **Program na Windows** pyta GitHuba o *najnowsze wydanie* tego repozytorium (`/releases/latest`) i pobiera z niego
  `wersja.json` i paczkę `.zip`. Komputery z włączonym kanałem beta biorą najnowsze wydanie z plikiem `wersja.json`,
  także testowe.
- **Aplikacja na Androida** szuka najnowszego wydania z tagiem `android-v…` i pobiera plik `.apk`.

**Ważne:** wydania Androida muszą być publikowane z flagą „nie najnowsze” (`make_latest: false` /
`--latest=false`). Inaczej program na Windows uzna wydanie z Androida za swoje najnowsze i przestanie widzieć
aktualizacje. Automat `.github/workflows/przenies-android.yml` sprawdza to i w razie czego przywraca poprawne wydanie.

## Historia

Do listopada 2026 wydania Androida były w osobnym repozytorium `integrator-android-wydania`. Zostały tu przeniesione
z tymi samymi plikami (sprawdzone sumy kontrolne). Stare repozytorium zostaje, dopóki wszystkie telefony nie
zaktualizują się do wersji, która szuka wydań tutaj.

## Instalacja

**Windows:** pobierz `Synchronizacja-X.zip` z [najnowszego wydania](../../releases/latest), rozpakuj i uruchom
`Synchronizacja.exe`. Kolejne wersje program zainstaluje sam.

**Android:** na telefonie otwórz wydanie `android-v…`, pobierz plik `.apk` i otwórz go. Android zapyta o zgodę na
instalowanie z przeglądarki. Aktualizację instaluj na poprzednią wersję, bez odinstalowywania: ustawienia i hasła
zostaną.
