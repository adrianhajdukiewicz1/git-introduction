# Syllabus kursu Git

## Moduł 0: Wprowadzenie

- Problem, który Git rozwiązuje (praca na plikach, wersjonowanie, kolizje)
- Instalacja Git (Linux/Mac/Windows), konfiguracja globalna (user.name / user.email)
- SSH vs https

## Moduł 1: Podstawowy cykl pracy

- Tworzenie repo: `git init`, `git clone`
- Obszary: Working Directory / Staging Area / Local Repo / Remote
- `git status`, `git add`, `git commit`
- Komentarze commitów – konwencje conventional commits
- Praktyka: utworzenie prostego projektu (np. notatnik README + plik źródłowy)

## Moduł 2: Poruszanie się w historii

- `git log`, formatowanie logu (`--oneline --graph --decorate`)
- `git show`, `git diff` (między plikami, między commitami, staged vs working)
- Tagowanie wersji

## Moduł 3: .gitignore i ignorowanie plików

- Wzorce ignorowania (`*.log`, `node_modules/`, `.env`)
- Przypadki binarne i pliki IDE
- Generatory .gitignore (gitignore.io)
- Praktyka: .gitignore z credentials.json - **nigdy nie commituj plików z sekretami!**
- Ochrona wrażliwych danych (hasła, klucze API)

## Moduł 4: Praca z gałęziami

- Koncepcja branchy (odejście od głównej linii rozwoju)
- Tworzenie/zmiana/usuwanie: `git branch`, `git switch`, `git checkout -b`
- Scalanie: `git merge` (fast-forward vs true merge)
- Ćwiczenie: Feature branch + merge

## Moduł 5: Zdalne repozytoria i GitHub/GitLab

- Remote: `git remote add origin`, `git remote -v`
- Push/Pull: `git push`, `git fetch`, `git pull` (fetch + merge)
- Fork vs clone, kiedy który model
- Pull Request (PR) w GitHub / Merge Request w GitLab
  - Koncepcja, opis, code review, status checks
- Ustawienia ochrony gałęzi (Branch protection rules)
- Zakaz pushowania do main (branch protection)
- Pokaz dużego repozytorium i jak tam wyglądają PR/MR

## Moduł 6: Cofanie i naprawianie

- `git restore` / `git checkout HEAD` - cofanie zmian w plikach
- `git reset HEAD` - usuwanie ze staging area
- `git reset --hard` - cofanie commitów (**UWAGA: traci zmiany!**)
- Praktyka: staging area workflow z `git status`

## Moduł 7: Dodatkowo (jeśli starczy czasu)

- Pre-commit hooks (automatyczne sprawdzenia)
- Git submodules (alternatywa to instalowanie python packages)
- Git aliases (skróty dla często używanych komend)
- `git rm` (usuwanie plików z repo)
- `git stash` (schowek na zmiany)
- `git cherry-pick` (przenoszenie konkretnych commitów)
- `git blame` (historia zmian w pliku)
- Revert MR - w GitLab
