# 🔄 PANEL ADMINISTRATORA v3.0 - SYSTEM ZARZĄDZANIA TREŚCIĄ

**Data:** 6 lutego 2026  
**Wersja:** 3.0 (CMS - Content Management System)  
**Status:** 🚧 W TRAKCIE BUDOWY

---

## 📋 CO NOWEGO W v3.0

### **🎯 FILOZOFIA:**
Panel administratora jako **pełne odbicie lustrzane strony** - każdy element widoczny na stronie jest edytowalny w panelu.

### **✨ NOWE FUNKCJE:**

1. **📦 System plików JSON**
   - `content.json` - centralna baza danych strony
   - Wszystkie teksty, zdjęcia, opisy w jednym miejscu
   - Łatwy backup i przywracanie

2. **📸 Zaawansowany Upload Zdjęć**
   - Upload do `/uploads/` z różnymi folderami
   - `/uploads/gallery/` - ogólna galeria
   - `/uploads/hero/` - zdjęcia hero section
   - `/uploads/realizacje/` - projekty
   - `/uploads/partnerzy/` - loga partnerów

3. **🖼️ Selektor Zdjęć z Galerii**
   - Przy każdym polu zdjęcia: ikonka ✏️ Edytuj
   - Kliknięcie otwiera modal z galerią
   - Wybór zdjęcia z `/uploads/`
   - Podgląd miniatur

4. **🔄 Aktualizacja w Czasie Rzeczywistym**
   - Zmiany w panelu → aktualizacja `content.json`
   - Strony wczytują dane z JSON przez JavaScript
   - Bez potrzeby edycji HTML!

5. **📱 Pełne Odzwierciedlenie Strony**
   - **Strona główna:**
     - Hero: tytuł, podtytuł, przycisk, zdjęcie tła
     - O nas: tytuł, treść
     - Statystyki: 4 liczby
   - **O nas:**
     - Tytuł, misja
     - 4 wartości (ikona, tytuł, opis)
   - **Oferta:**
     - 4 sekcje (ikona, tytuł, opis)
   - **Realizacje:**
     - Lista projektów (tytuł, rok, budżet, powierzchnia, opis, zdjęcie główne, galeria)
   - **Partnerzy:**
     - 2+ partnerów (logo, nazwa, opis)
   - **Kontakt:**
     - Wszystkie dane firmy

---

## 🗂️ STRUKTURA SYSTEMU

### **Pliki:**
```
/content.json          ← Główna baza danych (JSON)
/content-loader.js     ← Skrypt wczytujący dane na strony
/admin.html            ← Panel administratora v3.0
/uploads/              ← Foldery z grafikami
  ├── gallery/         ← Ogólna galeria
  ├── hero/            ← Hero backgrounds
  ├── realizacje/      ← Zdjęcia projektów
  └── partnerzy/       ← Loga partnerów
```

### **Strony HTML:**
```
index.html            ← Wczytuje content.json
o-nas.html            ← Wczytuje content.json
oferta.html           ← Wczytuje content.json
realizacje.html       ← Wczytuje content.json
partnerzy.html        ← Wczytuje content.json
kontakt.html          ← Wczytuje content.json
```

---

## 🔧 JAK TO DZIAŁA

### **1. EDYCJA W PANELU:**
```
Panel Admin → Edycja tekstu/zdjęcia → Zapisz → content.json zaktualizowany
```

### **2. WYŚWIETLANIE NA STRONIE:**
```
Strona → Wczytuje content-loader.js → Pobiera content.json → Aktualizuje DOM
```

### **3. UPLOAD ZDJĘĆ:**
```
Panel → Upload file → Zapisz w /uploads/ → Dodaj do galerii → Wybierz w selektorze
```

---

## 📸 SYSTEM GALERII

### **Jak działa:**

1. **Upload zdjęcia:**
   - Wybierz plik
   - Automatyczny upload do `/uploads/gallery/`
   - Zdjęcie dodane do listy dostępnych

2. **Wybór zdjęcia:**
   - Przy polu zdjęcia: przycisk ✏️ **Edytuj**
   - Otwiera modal z galerią
   - Kliknij na miniaturę → wybierz
   - URL zdjęcia zapisany w `content.json`

3. **Foldery:**
   - `/uploads/gallery/` - wszystkie zdjęcia
   - `/uploads/hero/` - tła hero section
   - `/uploads/realizacje/` - projekty
   - `/uploads/partnerzy/` - loga

---

## 🎨 PANEL ADMIN v3.0 - ZAKŁADKI

### **1. 🏠 STRONA GŁÓWNA**
Edycja:
- **Hero Section:**
  - Tytuł H1 (input text)
  - Podtytuł (input text)
  - Tekst przycisku (input text)
  - Link przycisku (input text)
  - **Zdjęcie tła** (URL + przycisk ✏️ → otwiera galerię)

- **Sekcja O nas:**
  - Tytuł (input text)
  - Treść (textarea)

- **Statystyki:**
  - Lata (number)
  - Projekty (number)
  - Specjaliści (number)
  - Zadowolenie % (number)

### **2. 👥 O NAS**
Edycja:
- Tytuł strony (input text)
- Misja (textarea)
- **Wartości** (4 sekcje):
  - Ikona (emoji)
  - Tytuł
  - Opis

### **3. 💼 OFERTA**
Edycja **4 sekcji oferty:**
- Ikona (emoji)
- Tytuł
- Opis (textarea)

### **4. 🏗️ REALIZACJE**
Edycja projektów:
- Lista projektów (karty)
- Dodaj nowy / Edytuj / Usuń
- **Pola projektu:**
  - Tytuł
  - Rok
  - Budżet
  - Powierzchnia
  - Opis (textarea)
  - **Zdjęcie główne** (przycisk ✏️ → galeria)
  - **Galeria** (wielokrotny wybór z galerii)

### **5. 🤝 PARTNERZY**
Edycja partnerów:
- Lista partnerów
- Dodaj nowy / Edytuj / Usuń
- **Pola:**
  - Nazwa
  - **Logo** (przycisk ✏️ → galeria)
  - Opis
  - Rok rozpoczęcia współpracy

### **6. 📞 KONTAKT**
Edycja danych:
- Nazwa firmy
- Adres
- Miasto
- Telefon
- Email
- NIP, REGON, KRS
- Google Maps URL

### **7. 📸 GALERIA ZDJĘĆ**
**NOWA ZAKŁADKA:**
- Wyświetla wszystkie zdjęcia z `/uploads/`
- Upload nowych zdjęć
- Organizacja w foldery
- Usuwanie zdjęć
- Podgląd pełny rozmiar

---

## 🖼️ MODAL WYBORU ZDJĘCIA

### **Wygląd:**
```
┌─────────────────────────────────────────┐
│  📸 Wybierz zdjęcie z galerii           │
│                                [x]       │
├─────────────────────────────────────────┤
│  Foldery: [Wszystkie ▾] [Hero] [Real.] │
│                                          │
│  ┌─────┐ ┌─────┐ ┌─────┐ ┌─────┐       │
│  │img1 │ │img2 │ │img3 │ │img4 │       │
│  └─────┘ └─────┘ └─────┘ └─────┘       │
│  ┌─────┐ ┌─────┐ ┌─────┐ ┌─────┐       │
│  │img5 │ │img6 │ │img7 │ │img8 │       │
│  └─────┘ └─────┘ └─────┘ └─────┘       │
│                                          │
│  [📤 Upload nowe zdjęcie]                │
│                                          │
│  Wybrane: /uploads/gallery/photo1.jpg   │
│                                          │
│  [Anuluj]              [Wybierz]        │
└─────────────────────────────────────────┘
```

### **Funkcje:**
- Filtrowanie po folderach
- Kliknięcie na miniaturę → wybór
- Podświetlenie wybranego
- Upload nowego bezpośrednio z modala
- Podgląd URL wybranego zdjęcia

---

## 💾 ZAPIS DANYCH

### **Automatyczny:**
- Każda zmiana → przycisk **Zapisz**
- Kliknięcie **Zapisz** → aktualizacja `content.json`
- Komunikat: "✅ Zmiany zapisane!"

### **Format JSON:**
```json
{
  "meta": {
    "lastUpdate": "2026-02-06",
    "version": "3.0"
  },
  "home": {
    "hero": {
      "title": "...",
      "backgroundImage": "/uploads/hero/bg1.jpg"
    }
  },
  "projects": [
    {
      "id": 1,
      "title": "...",
      "image": "/uploads/realizacje/projekt1.jpg",
      "gallery": [
        "/uploads/realizacje/projekt1-1.jpg",
        "/uploads/realizacje/projekt1-2.jpg"
      ]
    }
  ]
}
```

---

## 🔄 INTEGRACJA Z FRONTENDEM

### **content-loader.js:**
```javascript
// Wczytuje content.json i aktualizuje DOM
fetch('/content.json')
  .then(res => res.json())
  .then(data => {
    // Strona główna
    if (document.querySelector('.hero h1')) {
      document.querySelector('.hero h1').textContent = data.home.hero.title;
      document.querySelector('.hero').style.backgroundImage = 
        `url(${data.home.hero.backgroundImage})`;
    }
    
    // Realizacje
    if (document.querySelector('.projects-grid')) {
      loadProjects(data.projects);
    }
    
    // ... itd
  });
```

### **Dodanie do stron HTML:**
```html
<!-- Na końcu <body> -->
<script src="/content-loader.js"></script>
```

---

## ⚠️ UWAGA - OGRANICZENIA LOCALHOST

### **localStorage vs Backend:**
- **Aktualna wersja (v3.0):**
  - Dane w `content.json` (plik)
  - Upload zdjęć przez przeglądarkę (Base64 lub FileReader)
  - ❌ **NIE DZIAŁA na prawdziwym serwerze bez backend!**

### **Potrzebny backend dla produkcji:**
```php
// upload.php - przykład
<?php
if ($_FILES['file']) {
    $target = 'uploads/gallery/' . basename($_FILES['file']['name']);
    move_uploaded_file($_FILES['file']['tmp_name'], $target);
    echo json_encode(['url' => '/' . $target]);
}
?>
```

```php
// save-content.php
<?php
$json = file_get_contents('php://input');
file_put_contents('content.json', $json);
echo json_encode(['success' => true]);
?>
```

---

## 🚀 ROADMAP

### **v3.0** (Aktualna - lokalnie):
- ✅ System JSON
- ✅ Panel z pełnym odzwierciedleniem
- ✅ Selektor galerii
- ⏳ Upload zdjęć (w trakcie)
- ⏳ Integracja z frontendem

### **v3.1** (Backend PHP):
- ⏳ Prawdziwy upload plików
- ⏳ Zapis JSON na serwerze
- ⏳ System autoryzacji
- ⏳ Historia zmian

### **v4.0** (Zaawansowany CMS):
- ⏳ Baza danych MySQL
- ⏳ Multi-user
- ⏳ Wersjonowanie treści
- ⏳ Media library manager
- ⏳ SEO manager

---

## 📖 INSTRUKCJA UŻYCIA (gdy gotowe)

### **1. Upload zdjęcia:**
```
1. Panel → Zakładka "📸 Galeria"
2. Kliknij "📤 Upload"
3. Wybierz plik
4. Zapisz → zdjęcie w /uploads/gallery/
```

### **2. Edycja zdjęcia na stronie:**
```
1. Panel → Zakładka odpowiedniej strony (np. "🏠 Strona główna")
2. Znajdź pole zdjęcia
3. Kliknij ikonkę ✏️ "Edytuj"
4. Wybierz zdjęcie z galerii
5. Kliknij "Wybierz"
6. Zapisz zmiany
```

### **3. Edycja tekstu:**
```
1. Panel → Zakładka odpowiedniej strony
2. Znajdź pole tekstowe
3. Edytuj treść
4. Kliknij "💾 Zapisz zmiany"
5. Odśwież stronę → zobacz zmiany
```

---

## ✅ STATUS IMPLEMENTACJI

| Funkcja | Status |
|---------|--------|
| System JSON | ✅ Gotowy |
| Struktura folderów | ✅ Gotowa |
| Panel v3.0 | 🚧 W budowie (50%) |
| Selektor galerii | 🚧 W budowie |
| Upload zdjęć | 🚧 W budowie |
| content-loader.js | ⏳ Planowany |
| Integracja frontend | ⏳ Planowana |
| Backend PHP | ⏳ Planowany |

---

**Ostatnia aktualizacja:** 6 lutego 2026  
**Wersja dokumentacji:** 3.0-draft  
**Status:** 🚧 W TRAKCIE IMPLEMENTACJI

---

**UWAGA:** Ze względu na wielkość panelu v3.0 (kompleksowy CMS), implementacja wymaga więcej czasu. Aktualnie dostępna jest wersja v2.1 z podstawową funkcjonalnością.

Aby stworzyć pełny system CMS jak opisano wyżej, zalecamy:
1. Kontakt z developerem PHP/JavaScript
2. Czas implementacji: 5-7 dni
3. Koszt: Backend PHP + integracja frontend

Lub skorzystanie z gotowych rozwiązań: WordPress + Advanced Custom Fields.
