# 🚀 PANEL v4.0 - LIVE EDITOR

**REWOLUCYJNA ZMIANA:** Teraz widzisz stronę 1:1 i edytujesz bezpośrednio na niej!

---

## 🎯 CO TO JEST?

**Panel v4.0 Live Editor** to:
- ✅ **Wyświetla prawdziwą stronę** w iframe
- ✅ **Klikasz bezpośrednio w elementy** aby je edytować
- ✅ **Pomarańczowe ramki** pokazują co można edytować
- ✅ **Quick Edit** - szybka edycja w okienku
- ✅ **Bez opisów** - widzisz to co edytujesz!

---

## 🔑 LOGOWANIE

**URL:** https://armpolbudownictwo.pl/admin-v4.html

**Login:** armpoldev1  
**Hasło:** haslotestowe123

---

## 🎮 JAK UŻYWAĆ?

### Krok 1: Zaloguj się
Wpisz login i hasło

### Krok 2: Włącz tryb edycji
Kliknij przycisk **✏️ Włącz Edycję** (góra, środek)

### Krok 3: Zobaczysz pomarańczowe ramki
Wszystkie edytowalne elementy będą podświetlone

### Krok 4: Kliknij w element
- Kliknij w tekst/nagłówek → otworzy się okienko
- Wpisz nową wartość
- Kliknij **💾 Zapisz**

### Krok 5: Zapisz zmiany
Kliknij **💾 Zapisz Zmiany** (prawy górny róg)

---

## 🖼️ ZMIANA ZDJĘĆ

1. Włącz tryb edycji
2. Kliknij w zdjęcie (pomarańczowa ramka)
3. Otworzy się okienko z podglądem
4. Kliknij **🖼️ Zmień zdjęcie**
5. Wybierz z galerii lub wgraj nowe
6. Kliknij **💾 Zapisz Zmiany**

---

## 📱 RESPONSIVE PREVIEW

W prawym górnym rogu masz przyciski:
- **🖥️ Desktop** - widok na komputerze
- **📱 Tablet** - widok na tablecie
- **📱 Mobile** - widok na telefonie

Możesz zobaczyć jak strona wygląda na różnych urządzeniach!

---

## 📄 ZMIANA STRONY

Górny pasek → lista rozwijana:
- 🏠 Strona Główna
- ℹ️ O Nas
- 📋 Oferta
- 🏗️ Realizacje
- 🤝 Partnerzy
- 📞 Kontakt

Wybierz stronę którą chcesz edytować!

---

## ✨ CO MOŻESZ EDYTOWAĆ?

### Na stronie głównej:
- ✅ Tytuł główny (duży napis)
- ✅ Podtytuł
- ✅ Tekst przycisku
- ✅ Zdjęcie tła
- ✅ Wszystkie nagłówki (h1, h2, h3)
- ✅ Wszystkie paragrafy
- ✅ Wszystkie zdjęcia

### System automatycznie znajdzie:
- Wszystkie nagłówki
- Wszystkie teksty
- Wszystkie zdjęcia
- I podświetli je pomarańczowymi ramkami!

---

## 💾 ZAPISYWANIE

Po kliknięciu **💾 Zapisz Zmiany**:
1. Dane zapisują się do LocalStorage
2. Automatycznie pobierze się plik `content-v4.json`
3. Pojawi się komunikat: **✅ Zmiany zostały zapisane!**

**BACKUP:** Plik `content-v4.json` to Twój backup - zachowaj go!

---

## 🎨 INTERFEJS

### Górny pasek (niebieski):
- **Logo** - ARM-POL Live Editor v4.0
- **Selektor strony** - wybierz którą stronę edytujesz
- **Przycisk edycji** - włącz/wyłącz tryb edycji
- **Zapisz** - pojawia się gdy masz zmiany
- **Wyloguj** - wyjście z panelu

### Główny obszar:
- **Strona na żywo** - widzisz dokładnie to co będzie na stronie
- **Pomarańczowe ramki** - pokazują co możesz edytować (tylko w trybie edycji)
- **Etykiety** - nad każdą ramką jest opis co to jest

### Quick Edit (wyskakujące okienko):
- Tytuł (np. "Tytuł Hero")
- Pole tekstowe lub textarea
- Przyciski: **💾 Zapisz** i **✖️ Anuluj**

---

## 🖼️ GALERIA ZDJĘĆ

Kliknij **🖼️ Zmień zdjęcie**:

### Otworzy się modalne okno:
1. **Góra** - obszar wgrywania (przeciągnij pliki)
2. **Dół** - siatka dostępnych zdjęć

### Wgrywanie:
- Przeciągnij JPG/PNG na obszar **📤 Wgraj nowe zdjęcie**
- LUB kliknij i wybierz z dysku

### Wybieranie:
- Kliknij w zdjęcie z galerii
- Natychmiast zostanie zastosowane!

---

## 🔄 JAK TO DZIAŁA?

```
Ładowanie strony
    ↓
Strona wyświetla się w iframe (środek ekranu)
    ↓
JavaScript skanuje stronę i znajduje edytowalne elementy
    ↓
Włączasz tryb edycji
    ↓
Pomarańczowe ramki nakładają się na elementy
    ↓
Klikasz w element
    ↓
Otwiera się Quick Edit z aktualną wartością
    ↓
Edytujesz i klikasz Zapisz
    ↓
Element na stronie zmienia się natychmiast
    ↓
Klikasz "Zapisz Zmiany"
    ↓
Dane zapisują się do LocalStorage
    ↓
Pobiera się backup JSON
    ↓
GOTOWE!
```

---

## ⚡ KLUCZOWE ZALETY v4.0

| Funkcja | v3.0 | v4.0 |
|---------|------|------|
| Widok strony | ❌ Tylko opis | ✅ **Prawdziwa strona** |
| Edycja | ❌ Formularze | ✅ **Kliknij w element** |
| Podgląd | ❌ Tylko tekst | ✅ **Widzisz 1:1** |
| Intuicyjność | ⚠️ Średnia | ✅ **Bardzo łatwe** |
| Szybkość | ⚠️ Wolne | ✅ **Błyskawiczne** |

---

## 🎯 PRZYKŁAD UŻYCIA

### Chcesz zmienić główny tytuł na stronie:

**v3.0 (stary sposób):**
1. Wybierz "Strona Główna"
2. Poszukaj sekcji "Hero Section"
3. Znajdź pole "Tytuł H1"
4. Kliknij "Włącz edycję"
5. Kliknij w tekst
6. Wpisz nową wartość
7. Zapisz

**v4.0 (nowy sposób):**
1. Kliknij **✏️ Włącz Edycję**
2. Kliknij w duży tytuł (widzisz go!)
3. Wpisz nową wartość
4. Kliknij **💾 Zapisz**

**7 kroków → 4 kroki!** 🚀

---

## 📊 STATYSTYKI

- ✅ Automatycznie znajduje **wszystkie edytowalne elementy**
- ✅ Wyświetla **rzeczywistą stronę** (nie makietę)
- ✅ **Pomarańczowe ramki** pokazują co można kliknąć
- ✅ **Quick Edit** pojawia się natychmiast
- ✅ **Responsive preview** (Desktop/Tablet/Mobile)

---

## ⚠️ WAŻNE

### Co NIE DZIAŁA w LocalStorage:
- ❌ Synchronizacja między przeglądarkami
- ❌ Backup automatyczny na serwerze
- ❌ Historia zmian (undo)
- ❌ Współdzielenie z innymi użytkownikami

### Rozwiązanie:
**Zawsze pobieraj backup** (`content-v4.json`) po każdej sesji edycji!

---

## 🐛 ROZWIĄZYWANIE PROBLEMÓW

### Nie widzę pomarańczowych ramek?
→ Kliknij **✏️ Włącz Edycję**

### Ramki są w złym miejscu?
→ Zrestartuj tryb edycji (wyłącz i włącz ponownie)

### Nie mogę kliknąć w element?
→ Sprawdź czy jest pomarańczowa ramka (jeśli nie, element nie jest edytowalny)

### Zmiany zniknęły?
→ Sprawdź czy kliknąłeś **💾 Zapisz Zmiany** przed wylogowaniem

---

## 📚 PORÓWNANIE WERSJI

| Wersja | Opis | Główna cecha |
|--------|------|-------------|
| v1.0 | Podstawowy panel | Logowanie + lista realizacji |
| v2.0 | Rozszerzony | 6 zakładek edycji |
| v2.1 | Naprawa | Fix liczby projektów |
| v3.0 | System CMS | Edycja inline + galeria |
| **v4.0** | **LIVE EDITOR** | **Wyświetla stronę 1:1!** ⭐ |

---

## ✅ STATUS

**WERSJA 4.0 - GOTOWA DO UŻYCIA! 🚀**

- ✅ Logowanie
- ✅ Wyświetlanie strony w iframe
- ✅ Automatyczne wykrywanie elementów
- ✅ Pomarańczowe ramki
- ✅ Quick Edit
- ✅ Edycja tekstów
- ✅ Edycja zdjęć
- ✅ Galeria
- ✅ Responsive preview
- ✅ Zapisywanie zmian
- ✅ Backup JSON

---

## 🎉 PODSUMOWANIE

**Panel v4.0** to największa aktualizacja!

### Dlaczego jest lepszy?
1. **Widzisz co edytujesz** - nie musisz zgadywać
2. **Klikasz bezpośrednio** - nie szukasz w menu
3. **Pomarańczowe ramki** - wiesz co można zmieniać
4. **Quick Edit** - szybka edycja w miejscu
5. **Responsive** - sprawdzisz jak wygląda na telefonie

---

**Miłego korzystania z panelu v4.0! 🚀**

---

**Data:** 7 lutego 2026  
**Wersja:** 4.0  
**URL:** https://armpolbudownictwo.pl/admin-v4.html  
**Login:** armpoldev1  
**Hasło:** haslotestowe123
