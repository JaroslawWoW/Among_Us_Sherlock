# Among Us Sherlock – Movement Tracker & Visualizer 

Projekt companion do gry **Among Us**, który automatycznie śledzi pozycje graczy na mapie podczas rozgrywki i zapisuje ich ruchy.  
Docelowo aplikacja ma pomagać w analizie zachowań crewmatów i identyfikacji impostorów na podstawie trajektorii ruchu.

---

## 🚀 Cel projektu

- Automatyczne przechwytywanie pozycji graczy na ekranie w czasie rzeczywistym.
- Tworzenie historii ruchu (logów) dla każdej rundy.
- Wizualizacja trajektorii graczy na mapie (The Skeld, Mira HQ itd.).
- W przyszłości: analiza ruchów pod kątem wykrywania impostorów za pomocą modeli ML.

---

## 🛠️ Technologie

- Python 3.x
- OpenCV (do analizy obrazu i wykrywania kolorów graczy)
- MSS lub PyAutoGUI (do robienia screenshotów)
- Matplotlib / Plotly (do wizualizacji ruchu)
- Pandas (do zarządzania danymi)
- (Opcjonalnie) TensorFlow / PyTorch – na późniejszym etapie do ML

---

## 📅 Roadmapa

### Faza 1: Prototyp ręczny (W TRAKCIE)
- [x] Uzbieranie grafik (Gracz, Czapki, Wdzianka, Google)
- [x] Generowanie random playerow
- [ ] Kordynaty mapy + random rozmieszczenie na mapach (tworzenie zestawu danych dla YALO)
- [ ] Pobieranie i wyświetlanie statycznej mapy Among Us
- [ ] Ręczne logowanie pozycji graczy do pliku CSV
- [ ] Podstawowa wizualizacja trajektorii ruchu na mapie

### Faza 2: Automatyczne przechwytywanie ruchu ()

- [ ] Automatyczne robienie screenshotów w czasie gry
- [ ] Wykrywanie pozycji graczy na podstawie kolorów (maskowanie HSV)
- [ ] Zapis współrzędnych ruchu do logów

### Faza 3: Zaawansowana analiza i wizualizacja

- [ ] Dynamiczna wizualizacja ruchu (animacja trajektorii)
- [ ] Wykrywanie trybu security / kamery i odpowiednia obsługa danych
- [ ] Integracja z bazą danych rund do dalszej analizy

### Faza 4: Modele uczenia maszynowego (future)

- [ ] Ekstrakcja cech z trajektorii ruchu (prędkość, dystans, zachowania)
- [ ] Budowa klasyfikatorów impostorów na podstawie ruchu
- [ ] Automatyczne alerty i wsparcie podczas rozgrywki

---

1. Zainstaluj wymagane biblioteki:

```bash
pip install opencv-python mss pandas matplotlib pyautogui
