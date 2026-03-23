# System (Pan-Tilt) śledzenia obiektów z uzyciem obrazu z kamery

## 📌 Opis
Konstrukcja i realizacja ukladu śledzenia obiektów. Składa się z kamery i lasera zamocowanych na platformie o 2 stopniach swobody napędzanej 2 silnikami krokowymi.
Wykrywanie oraz sledzenie realizowane jest poprzez analizę obrazu z uzyciem biblioteki OpenCV oraz YOLO.
Sterowanie jest oparte na algorytmie predykcyjnym, dzięki czemu mozliwe jest wyeliminowanie opoźnień i zrównanie osi lasera z celem podczas jego ruchu

<img width="436" height="495" alt="image" src="https://github.com/user-attachments/assets/0d5542f8-10fc-4622-b5b3-cfccec90ea6a" />


---

## 🎯 Cel projektu
- Zaprojektowanie oraz wykonanie konstrukcji
- dobór elementów elektronicznych oraz mikrokontrolera
- Algorytm rozpoznawania i śledzenia obiektów
- Precyzyjne śledzenie obiektów w osi kamery

---

## 🛠️ Narzędzia
- Matlab / Simulink
- Python (OpenCV, YOLO, NumPy)
- Arduino IDE (C++)
- Filtracja sygnału (Filtr kalmana)
- STM32Cube IDE


---

## 🧠 Co zrobiłem
- opracowałem model matematyczny układu oraz potwierdziłem skuteczność architektury układu sterowania
- Zaprojektowałem oraz wykonałem całą konstrukcję urządzenia
- zaimplementowałem sterowanie silnikami krokowymi
- Opracowałem algorytm wizyjny
- Wykorzystałem filtr Kalmana do poprawy jakości śledzenia
- Zaprojektowałem i zaimplementowałem układ regulacji predykcyjnej

---
Schemat układu sterowania:
<img width="1537" height="872" alt="image" src="https://github.com/user-attachments/assets/1930986f-356c-4dd5-bfc1-bfababd75abf" />



## 📊 Wyniki

### Wykrywanie obiektów
- czas regulacji: ~2 s dla skoku 25 mm
- test dla przejścia z (25,25) → (0,0)

<img width="400" src="https://github.com/user-attachments/assets/6be00de1-8fcb-4ea3-a438-ef2cae340720" />

---

### Odporność na zakłócenia
- układ stabilizuje kulkę po zaburzeniu (pchnięcie)

<img width="400" src="https://github.com/user-attachments/assets/662a6bfb-986c-46cd-9281-b41ddc3d0b15" />

---

### Trajektorie ruchu
- poprawna realizacja ruchu po okręgu i kwadracie
- zgodność z wartością zadaną

<img width="300" src="https://github.com/user-attachments/assets/6d6e8734-25c3-461f-b381-3cc0a7beb066" />

---

## 🌀 Demo wideo (kliknij, aby obejrzeć)


### Sledzenie czlowieka 
[![Trajektoria](https://img.youtube.com/vi/QgTJa6kDOz0/0.jpg)](https://www.youtube.com/watch?v=QgTJa6kDOz0)


---

## 📉 Ograniczenia
-zbyt wolna kamera

---

## 📄 Raport
[Pełny raport PDF](./raport.pdf)
