# PLC-linia-produkcyjna

## Aplikacja sterująca dla symulowanego obiektu linii produkcyjnej

Obiekt sterowania składa się z generatora paczek (emitera), czterech głównych odcinków 
taśmociągów oraz układu transferów (sorterów) kierujących obiekty do czterech
koszy, czterech elementów usuwających paczki. Oraz czujników pozwalających zidentyfikować 
dany rodzaj paczki (Długa, Szeroka, Wysoka).

W ramach projektu zrealizowano następujące funkcjonalności (zgodnie z poleceniami):
  1. Sterowanie kierowaniem wszystkich paczek do wybranego kosza (1, 2, 3 lub 4).
  2. Sterowanie trybem sekwencyjnym – cykliczne kierowanie paczek do koszy 1, 2, 3, 4.
  3. Sortowanie warunkowe – wybrany typ paczki trafia do zadanego kosza, a pozostałe
     do kosza nr 1 (domyślnego).
  4. Sortowanie predefiniowane – paczki Długie, Szerokie i Wysokie trafiają do przypisanych
     im odgórnie koszy (1, 2, 3).
  6. Pełna konfiguracja – użytkownik decyduje, jakie typy paczek trafiają do których
     koszy za pomocą panelu.

W ramach projektu zrealizowano kompleksowy system sterowania linią sortującą.
Udało się zaimplementować wszystkie pięć wymaganych funkcjonalności, od prostego sterowania
ręcznego po macierzową konfigurację sortowania.

Przeprowadzone testy w środowisku symulacyjnym potwierdziły poprawność działania
algorytmów – paczki są praktycznie bezbłędnie rozpoznawane przez blok Kategoryk i
ponad 90 % przypadków kierowane do właściwych koszy zgodnie z logiką wybranego
zadania.
