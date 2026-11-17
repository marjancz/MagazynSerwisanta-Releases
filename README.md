# Magazyn Serwisanta 1.0.1

## Najważniejsze zmiany

# Zmiany w wersji 1.0.1

Poprawki wyglądu i obsługi w stosunku do wersji 1.0.0.

## Interfejs aplikacji

- Poprawiono proporcje pulpitu: równe kafelki, większe ikony, czytelne nazwy na ciemniejszych pasach oraz wyraźniejszy połysk i cienie 3D.
- Dosunięto podpis autora bezpośrednio pod tytuł. W ekranie „O aplikacji” usunięto niebieski podkład podpisu, zachowując odręczny krój i pomarańczowe podkreślenie.
- Odświeżono ekran „Magazyn”: podsumowania, wyszukiwarkę z lupą oraz karty części. Wartości całkowite są wyświetlane bez zbędnej części dziesiętnej, np. „1 szt.” zamiast „1,0 szt.”.
- Dopasowano ekran „Przyjęcia i wydania”: trzy wyśrodkowane kafelki na 60% szerokości ekranu, większe ilustracje i nazwy „Dodaj”, „Przyjęcie” oraz „Wydanie”.
- Poprawiono formularze: zaokrąglone pola o wysokości co najmniej 56 dp, podkład pływających etykiet, oddzielone sekcje pozycji i danych wspólnych oraz przyciski z efektem 3D. Usunięto nadmiar pustej przestrzeni w formularzu „Dodaj”.
- Ujednolicono wygląd ekranów „Import / eksport”, „Kopie zapasowe” i „Generator”. Dodano ilustracje formatów arkuszy, czytelne oznaczenia statusów kopii oraz daty w przystępnym formacie.
- Odświeżono kafelek sprawdzania aktualizacji: niebieski gradient, ikona odświeżania, połysk i cień. Zachowano komunikaty o wyniku oraz blokadę przycisku podczas sprawdzania lub zlecania pobrania.

## Nawigacja i obsługa

- Przycisk „Wróć” oraz systemowy Wstecz w formularzach „Dodaj”, „Przyjęcie” i „Wydanie” prowadzą do ekranu wyboru operacji „Przyjęcia i wydania”.
- Powrót z Generatora na pulpit czyści cztery pola wejściowe i wynik. Zachowano zastępowanie cyfr i automatyczne przechodzenie do kolejnego pola.

## Historia operacji

- Poprawiono wyszukiwarkę i układ filtrów: opcje zawijają się do kolejnego wiersza zamiast znikać poza krawędzią ekranu.
- Zmniejszono rozmiar podsumowań kart, zachowując kolorystyczne rozróżnienie operacji i rozwijane szczegóły. Nazwy techniczne zastąpiono czytelnymi opisami, np. „Korekta importu”.
- Przebudowano wybór własnego okresu: osobne pola „Od” i „Do”, każde z kalendarzem i krótkim nagłówkiem daty. Dodano kontrolę kolejności dat; cały ostatni dzień jest uwzględniany w wynikach.

## Zgodność danych

- Zmiany nie wymagają migracji bazy Room. Zachowano mechanizmy zapisu operacji, importu, kopii zapasowych, eksportu PDF i aktualizacji oraz algorytm Generatora.
- Aplikację należy instalować jako aktualizację dotychczasowej wersji, bez jej odinstalowywania i bez czyszczenia danych.

## Instalacja

Pobierz app-release.apk z załączników tego wydania. Zainstaluj jako aktualizację, bez odinstalowywania aplikacji.

## Dane techniczne

Magazyn Serwisanta
Wersja: 1.0.1
versionCode: 7
Pakiet: pl.magazynserwisanta
SHA-256 APK: 699FF0092F02EE7C37D40E863C63BD39975B3E9EC016217B2A3FB7DC31AE8038
Certyfikat SHA-256: A11C0E278C952009D22C3A02A65EC7692C97231B7FE6721ABC7989D815F2C213
