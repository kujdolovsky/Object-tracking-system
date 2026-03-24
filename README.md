# 🎯 System śledzenia obiektów (Pan-Tilt) z wykorzystaniem wizji komputerowej

## 📌 Opis projektu
Projekt przedstawia system śledzenia obiektów w czasie rzeczywistym oparty na platformie typu **pan-tilt (2 DOF)**.  
Układ wykorzystuje kamerę oraz wskaźnik laserowy zamocowane na ruchomej konstrukcji napędzanej silnikami krokowymi.

Detekcja i śledzenie obiektów realizowane są z wykorzystaniem metod wizji komputerowej (**OpenCV + YOLO**), natomiast sterowanie opiera się na podejściu predykcyjnym, co pozwala ograniczyć opóźnienia i zwiększyć dokładność śledzenia.

<img width="436" height="495" alt="image" src="https://github.com/user-attachments/assets/0d5542f8-10fc-4622-b5b3-cfccec90ea6a" />

---

## 🎯 Cel projektu
- Projekt i wykonanie konstrukcji mechanicznej (2 DOF)
- Dobór elektroniki i mikrokontrolera
- Implementacja algorytmu detekcji i śledzenia obiektów
- Opracowanie układu sterowania zapewniającego płynne i precyzyjne śledzenie

---

## 🛠️ Wykorzystane narzędzia i technologie
- **Python** (OpenCV, YOLO, NumPy)
- **MATLAB / Simulink**
- **STM32 (STM32CubeIDE)**
- **Arduino IDE (C++)**
- **Filtr Kalmana**
- Sterowanie silnikami krokowymi

---

## 🧠 Zakres mojej pracy
- Opracowanie modelu matematycznego układu
- Projekt i wykonanie konstrukcji mechanicznej
- Implementacja sterowania silnikami krokowymi
- Opracowanie algorytmu wizyjnego (detekcja + tracking)
- Implementacja filtru Kalmana do estymacji położenia
- Projekt i implementacja regulatora predykcyjnego

---

## ⚙️ Architektura systemu
Schemat układu sterowania:

<img width="1576" height="891" alt="image" src="https://github.com/user-attachments/assets/bf109700-8189-4302-a185-9b1dec36c438" />


---
## Schemat modelu regulatora predykcyjnego 1 osi w Simulinku:
Regulator korzystając z danych o aktualnej pozycji obiektu oraz platformy wylicza błąd śledzenia jaki wystąpi po czasie opóźnień, błąd ten trafia następnie do regulatora PID, który steruje prędkością silnika.
Szczegóły dostępne przy kontakcie ze mną.

<img width="1706" height="639" alt="image" src="https://github.com/user-attachments/assets/2ab24032-dfab-4c39-b323-b9f10e0baa82" />

## 📊 Dotychczasowe wyniki
### Wyniki symulacji (sterowanie z predykcją), Simulink
Weryfikacja działania regulatora predykcyjnego, trajektoria z symulowanymi zakłóceniami.
W symulacji regulator spełnia swoją funkcję bardzo dobrze.

<img width="1919" height="923" alt="image" src="https://github.com/user-attachments/assets/859c2298-bada-4fa8-af31-b4bce74b52ea" />



## 🌀 Demo wideo (kliknij, aby obejrzeć)

### Śledzenie obiektu z uzyciem starego algorytmu predykcyjnego (bez kompensacji zakłóceń mechanicznych)
 System działa, wykrywa obiekty i już teraz jest w stanie śledzić je z zadowalającą dokładnością,
 aktualnie pracuję nad udoskonaleniem systemu sterowania poprzez implementację nowego regulatora predykcyjnego. 
 
[![Demo](https://img.youtube.com/vi/rupabkPK9xA/0.jpg)](https://youtu.be/rupabkPK9xA)

---

## 📉 Ograniczenia
- Ograniczona częstotliwość odświeżania kamery
- Niedoskonałości mechaniczne wpływające na precyzję
- Opóźnienia wynikające z przetwarzania obrazu

---

## 🚀 Dalszy rozwój
- Zastosowanie szybszej kamery global shutter
- Lepsza kalibracja i sztywniejsza konstrukcja
- Lepsza regulacja algorytmu sterowania predykcyjnego
- Optymalizacja kodu wizyjnego pod kątem wydajności
- Dodanie enkoderów absolutnych

---

## 📬 Kontakt
Jeśli masz pytania lub chcesz pogadać o projekcie — śmiało napisz 🙂
