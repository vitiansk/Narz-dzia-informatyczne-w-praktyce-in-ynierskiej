# Zadanie 4

Zastosowanie poleceń GIT.

## 1 Konfiguracja Git

Ustawienie danych użytkownika w konfiguracji Gita

```bash
git config --global user.name Viktor Daliak
git config --global user.email viktor.daliak8652@student.po.edu.pl
```

## 2 Tworzenie i inicjowanie lokalnego repozytorium
```bash
gir mkdir nowy-repozytorium
cd nowy-repozytorium
git init
```

## 3 Dodanie plików do repozytorium

Tworzenie nowych plików dodawanie ich do repozytorium, dodawanie wartości w pliku

```bash
touch plik1.txt
touch plik2.txt
git add .
echo "Treść" > plik1.txt
```

## 4 commit

```bash
git commit -m "Pierwszy commit"
```

## 5 zmina na plikach i zatwierdzenie zmian

zmiana nazy pliku, usuwanie pliku, dodawanie nowego pliku

```bash
git mv plik1.txt nowy_plik1.txt
git commit -m "Zmiana nazwy plik1"
git rm --cached nowy_plik1.txt
git commit -m "Usuniecie nowy_plik1 z repozytorium"
touch plik3.txt
git add plik3.txt
git commit -m "Dodanie plik3"
```

## 6 .gitignore

```bash
git log --oneline
git diff c1ef7f4
```

## 7 Tworzenie i łączenie gałęzi

```bash
git branch nowa_galez
git checkout nowa_galez
touch plik5.txt
echo "Treść 5" > plik5.txt
git add plik5.txt
git commit -m "Zmiany na nowej gałęzi"
git checkout master
git merge nowa_galez
```

# Autor
[Viktor Daliak] (https://github.com/vitiansk)
