# 🚀 Jak opublikować ten projekt na GitHub

Wszystko jest gotowe! Projekt jest już skonfigurowany i commitnięty lokalnie.

## Krok 1: Utwórz repozytorium na GitHub

1. Przejdź do: **https://github.com/new**
2. Wypełnij formularz:
   - **Repository name**: `AlpacaTutorial`
   - **Description**: Tutorial 11: Bracket Orders with Stop-Loss and Take-Profit
   - **Public** lub **Private** (wybierz według preferencji)
   - ❌ **NIE zaznaczaj** "Initialize this repository with a README"
   - ❌ **NIE dodawaj** .gitignore ani licencji
3. Kliknij **"Create repository"**

## Krok 2: Wypchnij kod na GitHub

Po utworzeniu repozytorium, wykonaj tę komendę w terminalu:

```bash
git push -u origin main
```

To wszystko! Twój kod zostanie opublikowany na GitHub.

## Co zostanie opublikowane ✅

- ✅ `bracket_bot.py` - główny bot z bracket orders
- ✅ `config.example.py` - przykład konfiguracji
- ✅ `README.md` - dokumentacja
- ✅ `requirements.txt` - zależności
- ✅ `instructions.md` - instrukcje tutoriala
- ✅ `.gitignore` - ochrona plików

## Co NIE zostanie opublikowane ❌

- ❌ `config.py` - Twoje klucze API (chronione przez .gitignore)
- ❌ `.cursorrules` - konfiguracja IDE (chroniona przez .gitignore)
- ❌ `__pycache__/` - cache Pythona (chroniony przez .gitignore)

## Sprawdzenie

Po wykonaniu `git push`, możesz sprawdzić swoje repozytorium:

**https://github.com/TomaszCieslar/AlpacaTutorial**

---

## 🔐 WAŻNE: Bezpieczeństwo

Plik `config.py` z Twoimi prawdziwymi kluczami API **NIGDY** nie zostanie wysłany na GitHub, ponieważ jest w `.gitignore`.

Jeśli kiedykolwiek przypadkowo commitujesz klucze API:
1. Natychmiast usuń je z repozytorium
2. **Wygeneruj nowe klucze** w panelu Alpaca
3. Zaktualizuj lokalny plik `config.py`

---

## Testowanie po sklonowaniu

Gdy ktoś sklonuje Twoje repozytorium, musi:

```bash
git clone https://github.com/TomaszCieslar/AlpacaTutorial.git
cd AlpacaTutorial
pip install -r requirements.txt
copy config.example.py config.py
# Następnie edytować config.py i dodać swoje klucze API
python bracket_bot.py
```

Powodzenia! 🎉

