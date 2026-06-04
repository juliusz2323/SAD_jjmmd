# SAD_jjmmd
2.06  Dodanie w pliku v2  porównania zbiorów surowego i wynikowego - po oczyszczeniu z braków i nieprawidłowych danych.

# Projekt SAD: Analiza cen laptopów

## 👥 Skład zespołu
1. Mirosław H.
2. Małgorzata B.
3. Juliusz M.
4. Dariusz F.

---

## 📝 Cel projektu
Oczyszczenie i analiza "brudnego" zbioru danych (ponad 1300 ofert laptopów z platformy e-commerce) w celu zbadania czynników realnie wpływających na ich cenę, jako fundament pod budowę modeli uczenia maszynowego.

---

## ⚙️ Zrealizowane etapy

* **Czyszczenie danych i imputacja:** Usunięcie błędnych znaków i jednostek ("GB", "kg") oraz uzupełnienie braków danych za pomocą algorytmu `KNNImputer`.
* **Inżynieria cech (Feature Engineering):** Zamiast zwykłego kodowania tekstu, wyciągnęliśmy z niego kluczowe parametry techniczne za pomocą wyrażeń regularnych (m.in. taktowanie procesora w GHz, pojemność dysków SSD i HDD, obecność ekranu dotykowego oraz matrycy IPS).
* **Wizualizacje:** Przygotowaliśmy przekroje danych obejmujące macierz korelacji, wykresy pudełkowe (*Boxplot*) oraz estetyczny wykres skrzypcowy (*Violin Plot*), pokazujący rozkład cen w zależności od przeznaczenia sprzętu.
* **Testy statystyczne:** Wykorzystując nieparametryczny test Kruskala-Wallisa udowodniliśmy, że system operacyjny współdzieli statystycznie istotną wariancję z ostateczną ceną laptopa (odrzucenie hipotezy zerowej, p-value < 0.05).
