# Git Cheat Sheet

## Konfiguracja i tworzenie

| Komenda | Opis |
|---------|------|
| `git config --global user.name "Name"` | Ustaw nazwę użytkownika |
| `git config --global user.email "email"` | Ustaw email |
| `git init` | Utwórz nowe repozytorium |
| `git clone <url>` | Sklonuj istniejące repozytorium |

## Podstawowe operacje

| Komenda | Opis |
|---------|------|
| `git status` | Sprawdź status plików |
| `git add <file>` | Dodaj plik do staging |
| `git add .` | Dodaj wszystkie zmienione pliki |
| `git commit -m "message"` | Utwórz commit |
| `git commit -am "message"` | Add + commit (tylko zmienione) |
| `git commit --amend` | Popraw ostatni commit |

## Gałęzie (Branches)

| Komenda | Opis |
|---------|------|
| `git branch` | Lista gałęzi |
| `git branch <name>` | Utwórz nową gałąź |
| `git switch <branch>` | Przełącz się na gałąź |
| `git switch -c <branch>` | Utwórz i przełącz na gałąź |
| `git merge <branch>` | Scal gałąź z bieżącą |
| `git branch -d <branch>` | Usuń gałąź |

## Historia i różnice

| Komenda | Opis |
|---------|------|
| `git log` | Pokaż historię commitów |
| `git log --oneline --graph` | Kompaktowy log z grafem |
| `git show <commit>` | Pokaż szczegóły commita |
| `git diff` | Różnice w working directory |
| `git diff --staged` | Różnice w staging area |
| `git diff <commit1> <commit2>` | Różnice między commitami |

## Zdalne repozytoria

| Komenda | Opis |
|---------|------|
| `git remote add origin <url>` | Dodaj zdalne repo |
| `git remote -v` | Lista zdalnych repo |
| `git push origin <branch>` | Wyślij zmiany na remote |
| `git push -u origin <branch>` | Push z ustawieniem tracking |
| `git fetch` | Pobierz zmiany (bez merge) |
| `git pull` | Pobierz i scal zmiany |

## Cofanie i naprawianie

| Komenda | Opis |
|---------|------|
| `git restore <file>` | Cofnij zmiany w pliku |
| `git restore --staged <file>` | Usuń plik ze staging |
| `git reset HEAD~1` | Cofnij ostatni commit (zachowaj zmiany) |
| `git reset --hard HEAD~1` | Cofnij commit i usuń zmiany |
| `git revert <commit>` | Cofnij commit (nowy commit) |
| `git reflog` | Historia wszystkich operacji |

## .gitignore

| Komenda | Opis |
|---------|------|
| `echo "*.log" >> .gitignore` | Ignoruj pliki .log |
| `echo "node_modules/" >> .gitignore` | Ignoruj katalog |
| `echo ".env" >> .gitignore` | Ignoruj pliki z sekretami |

## SSH i bezpieczeństwo

| Komenda | Opis |
|---------|------|
| `ssh-keygen -t ed25519 -C "email"` | Generuj klucz SSH |
| `cat ~/.ssh/id_ed25519.pub` | Wyświetl klucz publiczny |
| `ssh-add ~/.ssh/id_ed25519` | Dodaj klucz do agenta SSH |

## Przydatne dodatki

| Komenda | Opis |
|---------|------|
| `git stash` | Schowaj zmiany tymczasowo |
| `git stash push -m "message"` | Schowaj z nazwą |
| `git stash list` | Lista schowanych zmian |
| `git stash apply stash@{0}` | Przywróć konkretny stash |
| `git stash pop` | Przywróć ostatnie zmiany |
| `git tag <name>` | Utwórz tag |
| `git tag -a <name> -m "msg"` | Utwórz annotated tag |
| `git cherry-pick <commit>` | Przenieś konkretny commit |
| `git blame <file>` | Kto zmienił każdą linię |
| `git rm <file>` | Usuń plik z repo i dysku |
| `git rm --cached <file>` | Usuń z repo (zachowaj na dysku) |

## Aliasy i konfiguracja

| Komenda | Opis |
|---------|------|
| `git config --global alias.st status` | Utwórz alias (git st) |
| `git config --global alias.co checkout` | Alias dla checkout |
| `git config --global alias.br branch` | Alias dla branch |
| `git config --global alias.cm "commit -m"` | Alias dla commit -m |

---

## Przydatne linki

- [Oficjalna dokumentacja Git](https://git-scm.com/doc)
- [Learn Git Branching (interaktywny tutorial)](https://learngitbranching.js.org/)
- [Conventional Commits](https://www.conventionalcommits.org/)
- [gitignore.io](https://gitignore.io)
