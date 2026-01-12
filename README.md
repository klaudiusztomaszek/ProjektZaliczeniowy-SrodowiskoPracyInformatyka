# TrendSpotter 📊

**ProjektZaliczeniowy-SrodowiskoPracyInformatyka**

TrendSpotter to intuicyjne narzędzie do wizualizacji danych, które przekształca statyczne i nieczytelne arkusze kalkulacyjne w interaktywne mapy ciepła (**heatmaps**). Aplikacja pozwala błyskawicznie zidentyfikować trendy, anomalie oraz kluczowe wyniki, które w tradycyjnej tabeli mogłyby umknąć uwadze.

---

## 🚀 O projekcie

Aplikacja rozwiązuje problem "szumu informacyjnego" w surowych danych liczbowych. Zamiast analizować każdą komórkę z osobna, użytkownik otrzymuje czytelny obraz, gdzie intensywność koloru bezpośrednio odpowiada wartościom danych.

### Dla kogo?
* **Nauczyciele:** Szybka analiza ocen klasy i identyfikacja tematów sprawiających trudność.
* **Managerowie:** Monitorowanie KPI i wydajności zespołów w czasie.
* **Studenci:** Wizualizacja postępów w nauce i gromadzonych danych badawczych.

---

## ✨ Główne Funkcje

1. **Inteligentny Import Danych:**
   - Wczytywanie danych w formacie siatki.
   - Obsługa układu: **Kolumny** (kategorie/czas) oraz **Wiersze** (obiekty/osoby).
2. **Dynamiczna Mapa Ciepła:**
   - Automatyczne kolorowanie komórek na podstawie zdefiniowanych progów wartości.
   - Możliwość interakcji z tabelą (hover, tooltipy).
3. **Wykresy pomocnicze:**
   - Generowanie prostych wykresów uzupełniających widok tabelaryczny.
4. **Raportowanie:**
   - Tworzenie prostego raportu podsumowującego najważniejsze trendy i statystyki.

---

## 🛠 Struktura danych

Aplikacja jest zoptymalizowana pod konkretny układ macierzy:
* **Komórki B1, C1, ... (Oś X):** Kategorie, ramy czasowe, przedmioty.
* **Komórki A2, A3, ... (Oś Y):** Obiekty, osoby, nazwy projektów.

| | Kat. 1 (np. Styczeń) | Kat. 2 (np. Luty) |
| :--- | :---: | :---: |
| **Obiekt A (np. Jan Kowalski)** | 85 | 42 |
| **Obiekt B (np. Anna Nowak)** | 12 | 95 |

---

## 💻 Technologie

* **Frontend:** React / HTML5 / JavaScript
* **Wizualizacja:** Chart.js / D3.js
* **Stylizacja:** Tailwind CSS / CSS Modules

---