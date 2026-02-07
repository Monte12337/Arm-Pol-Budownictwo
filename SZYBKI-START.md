# 🚀 SZYBKI START - Panel v3.0

## 📥 INSTALACJA (2 minuty)

### Krok 1: Rozpakuj
```bash
unzip armpol-V3-FINAL.zip
```

### Krok 2: Wgraj na hosting
Skopiuj wszystko do `public_html/` lub `/var/www/html/`

### Krok 3: Ustaw uprawnienia
```bash
chmod 755 *.html
chmod 755 *.js
chmod 755 uploads/
chmod 644 uploads/.htaccess
```

## ✅ GOTOWE! Możesz korzystać z panelu

---

## 🔑 PIERWSZE LOGOWANIE

1. Wejdź na: **https://armpolbudownictwo.pl/admin-v3.html**

2. Zaloguj się:
   - **Login:** armpoldev1
   - **Hasło:** haslotestowe123

3. Wybierz zakładkę **🏗️ Realizacje**

4. Zobacz 6 przykładowych projektów

---

## ✏️ PIERWSZA EDYCJA (30 sekund)

### Zmień tytuł strony głównej:

1. Kliknij zakładkę **🏠 Strona Główna**
2. Kliknij przycisk **✏️ Włącz edycję**
3. Kliknij w tytuł (duży nagłówek)
4. Wpisz nowy tekst, np. "ARM-POL - Lider w inwestycjach medycznych"
5. Kliknij **💾 Zapisz Zmiany**

**GOTOWE!** Twoja zmiana została zapisana.

---

## 🖼️ PIERWSZE ZDJĘCIE (1 minuta)

### Wgraj zdjęcie do galerii:

1. Kliknij zakładkę **🖼️ Galeria Zdjęć**
2. Przeciągnij zdjęcie JPG/PNG na obszar **📤 Wgraj nowe zdjęcia**
3. Zdjęcie pojawi się w galerii

### Zmień zdjęcie tła:

1. Kliknij zakładkę **🏠 Strona Główna**
2. Kliknij przycisk **🖼️ Zmień zdjęcie** przy zdjęciu tła
3. Wybierz zdjęcie z galerii
4. Kliknij **💾 Zapisz Zmiany**

---

## 🏗️ DODAJ PROJEKT (2 minuty)

1. Kliknij zakładkę **🏗️ Realizacje**
2. Kliknij **➕ Dodaj nową realizację**
3. Wypełnij formularz:
   - Tytuł: "Szpital Wojewódzki Kraków"
   - Rok: 2024
   - Budżet: 15 000 000 PLN
   - Powierzchnia: 4500 m²
   - Opis: Krótki opis projektu
4. Wgraj 1-6 zdjęć
5. Kliknij **💾 Zapisz projekt**

---

## 📄 INTEGRACJA ZE STRONĄ

Dodaj do `<head>` w `index.html`:

```html
<script src="content-loader.js"></script>
```

**To wszystko!** Zmiany z panelu będą automatycznie widoczne na stronie.

---

## 🔧 ROZWIĄZYWANIE PROBLEMÓW

### Nie widzę zmian na stronie?
→ Dodaj `<script src="content-loader.js"></script>` do `index.html`  
→ Wyczyść cache (Ctrl+Shift+R)

### Zniknęły dane?
→ Otwórz ostatni pobrany plik `content.json`  
→ Użyj instrukcji z PANEL-V3-DOKUMENTACJA.md

### Panel nie działa?
→ Sprawdź czy plik `admin-v3.html` jest na serwerze  
→ Sprawdź uprawnienia: `chmod 755 admin-v3.html`

---

## 📚 PEŁNA DOKUMENTACJA

Otwórz plik: **PANEL-V3-DOKUMENTACJA.md**

Znajdziesz tam:
- ✅ Szczegółowy opis każdej funkcji
- ✅ Instrukcje backup i przywracania
- ✅ Zaawansowane opcje
- ✅ FAQ i troubleshooting

---

## 🎯 PODSTAWOWE FUNKCJE

| Funkcja | Gdzie | Jak |
|---------|-------|-----|
| Edycja tekstu | Dowolna zakładka | Włącz edycję → Kliknij tekst |
| Zmiana zdjęcia | Dowolna zakładka | Kliknij 🖼️ Zmień zdjęcie |
| Dodaj projekt | Realizacje | Kliknij ➕ Dodaj |
| Usuń projekt | Realizacje | Kliknij 🗑️ Usuń |
| Wgraj zdjęcia | Galeria | Przeciągnij pliki |
| Zapisz zmiany | Zawsze | Kliknij 💾 Zapisz |

---

## ✅ CHECKLIST WDROŻENIA

- [ ] Rozpakować ZIP
- [ ] Wgrać na hosting
- [ ] Ustawić uprawnienia
- [ ] Zalogować się do panelu
- [ ] Przetestować edycję
- [ ] Dodać `content-loader.js` do `index.html`
- [ ] Wyczyść cache
- [ ] Sprawdzić czy zmiany widoczne na stronie

---

## 📞 WSPARCIE

**Dokumentacja:** PANEL-V3-DOKUMENTACJA.md  
**Panel:** https://armpolbudownictwo.pl/admin-v3.html  
**Login:** armpoldev1  
**Hasło:** haslotestowe123

---

**Wersja:** 3.0  
**Data:** 6 lutego 2026  
**Status:** ✅ GOTOWY DO UŻYCIA

---

**Miłego korzystania z panelu ARM-POL! 🚀**
