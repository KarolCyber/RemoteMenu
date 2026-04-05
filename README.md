# Zdalne Menu Falownika: DEYE SUN-15k-SG05LP3 (Home Assistant)

Projekt udostępnia wirtualny interfejs graficzny dla Home Assistant, który odwzorowuje fizyczny panel sterowania falownika DEYE. Umożliwia to sterowanie i podgląd parametrów bezpośrednio z poziomu Dashboardu.

---

## ⚙️ Sposób działania
* **Integracja:** Komunikacja odbywa się za pomocą integracji **Solarman**.
* **Interfejs:** Interaktywne encje (przyciski, pola odczytu) są precyzyjnie nałożone na zdjęcie menu falownika.
* **Funkcjonalność:** Zarządzanie opcjami i odczyt wartości w układzie identycznym jak na fizycznym ekranie urządzenia.

## 🛠 Wymagania
* **Home Assistant** (zaktualizowany do stabilnej wersji).
* **Integracja Solarman** (kod bazuje na nazwach encji generowanych przez tę integrację).

## 🚀 Instrukcja wdrożenia

### 1. Przygotowanie kodu
Otwórz plik `ha_view_code.txt` w tym repozytorium i skopiuj całą jego zawartość do schowka.

### 2. Konfiguracja karty w HA
Proces instalacji został przedstawiony w poniższych krokach wideo:

1.  **Dodanie karty:**
    * Obejrzyj film: `krok_1_dodanie_karty.mov`.
    * W Dashboardzie HA dodaj nową kartę typu **Manual**, a następnie wklej skopiowany wcześniej kod.

2.  **Dodanie grafik:**
    * Obejrzyj film: `krok_2_dodanie_zdjęć_do_karty.mov`.
    * Wgraj wymagane pliki graficzne (tła menu) do folderu `/www/` w swojej instancji Home Assistant, aby karta wyświetlała się poprawnie.

---
> [!IMPORTANT]
> Upewnij się, że nazwy encji w Twoim systemie są zgodne z tymi w pliku `ha_view_code.txt`. W przypadku różnic, należy je ręcznie skorygować w kodzie karty.
