## Najważniejsze zmiany w wersji 1.0.3

Wersja 1.0.3 dodaje możliwość edycji historii operacji magazynowych. Zapisane przyjęcia i wydania można poprawiać lub usuwać, a aplikacja odpowiednio przelicza stany magazynowe. Poniżej opisano zmiany względem wersji 1.0.2.

## Historia operacji

- W szczegółach przyjęcia i wydania dodano przyciski „Edytuj” i „Usuń operację”. Edycja obejmuje całą operację, również wielopozycyjną.
- Można zmienić ilość i wybór części w pozycji, dodać kolejne pozycje lub usunąć wybrane pozycje z operacji. Dodawane części wybiera się z istniejącej kartoteki Magazynu.
- Można edytować cztery dane wspólne: firmę klienta, numer protokołu, Przesunięcie MM oraz notatkę. Zmiany są stosowane do wszystkich pozycji danej operacji.
- Usunięcie całej operacji wymaga potwierdzenia. Komunikat informuje o wpływie usunięcia na stany magazynowe.
- Import i przywracanie kopii zapasowych pozostają poza edycją i usuwaniem historii.

## Aktualizacja stanów magazynowych

- Przy edycji wydania zwiększenie ilości lub dodanie pozycji zmniejsza stan magazynowy. Zmniejszenie ilości lub usunięcie pozycji zwraca odpowiednią ilość do magazynu. Usunięcie całego wydania zwraca ilości wszystkich jego pozycji.
- Przy edycji przyjęcia zwiększenie ilości lub dodanie pozycji zwiększa stan magazynowy. Zmniejszenie ilości lub usunięcie pozycji odejmuje odpowiednią ilość z magazynu. Usunięcie całego przyjęcia odejmuje ilości wszystkich jego pozycji.
- Zmiana samych danych wspólnych nie wpływa na ilości w magazynie.
- Korekta uwzględnia różnicę między dotychczasową i nową zawartością operacji oraz bieżący stan magazynu.

## Kontrola poprawności

- Aplikacja blokuje zapis lub usunięcie operacji, jeśli skutkiem byłby ujemny stan którejkolwiek części. Komunikat wskazuje część, dla której brakuje ilości; cała zmiana zostaje odrzucona.
- Ilości muszą być dodatnimi, prawidłowymi liczbami. Zapis pustej operacji jest blokowany — do usunięcia całego wpisu służy osobna funkcja.
- Przed zapisem aplikacja sprawdza, czy operacja nie zmieniła się od otwarcia formularza. Jeśli została zmieniona lub usunięta, konieczne jest ponowne otwarcie jej aktualnej wersji.
- Historia i stany magazynowe są aktualizowane razem w jednej transakcji. Błąd zapisu powoduje wycofanie całej zmiany.

## Zgodność danych

- Aktualizacja nie zmienia schematu bazy Room i nie wymaga migracji istniejących danych.
- Edytować można również starsze, pojedyncze przyjęcia i wydania. Dodanie kolejnych pozycji łączy je w jedną operację wielopozycyjną.
- Zachowano datę operacji oraz istniejące mechanizmy importu, kopii zapasowych, raportów PDF i aktualizacji aplikacji.

## Instalacja

Pobierz app-release.apk z załączników tego wydania. Zainstaluj jako aktualizację, bez odinstalowywania aplikacji.

## Dane techniczne

Wersja: 1.0.3
versionCode: 9
Pakiet: pl.magazynserwisanta
SHA-256 APK: A58505635C3375D47E06B9CE99B2369286034B74FC56C3FA00FE6C48E7567F0E
Certyfikat SHA-256: A11C0E278C952009D22C3A02A65EC7692C97231B7FE6721ABC7989D815F2C213
