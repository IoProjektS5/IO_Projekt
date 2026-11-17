**Wymagania funkcjonalne**

**Zarządzanie kontem i bezpieczeństwo**

1.1: Rejestracja 

- Jako nowy użytkownik może zarejestrować się w systemie podając swój  aby uzyskać dostęp do platformy.

- Priorytet: Must Have

- Kryteria akceptacji:

- System wysyła link aktywacyjny na podany e-mail.

- Konto jest nieaktywne do momentu kliknięcia w link.

US 1.2: Logowanie i role użytkowników

- Jako zarejestrowany użytkownik może logować się do systemu i mieć dostęp do przejazdów do których jest zapisany

- Priorytet: Must Have

- Kryteria akceptacji:

- Użytkownik może zalogować się za pomocą e-maila i hasła.

- System weryfikuje poprawność danych logowania.

- Po zalogowaniu użytkownik widzi panel odpowiedni dla wybranej roli

**2. Kierowca**

2.1: Dodawanie nowej oferty przejazdu

- Jako kierowca, chcę dodać nowy przejazd (podać trasę, czas, liczbę miejsc), aby znaleźć pasażerów i podzielić się kosztami.

- Priorytet: Must Have

- Kryteria akceptacji: 

- Formularz wymaga podania: punktu startu, punktu docelowego, daty, godziny i liczby wolnych miejsc.

- System weryfikuje poprawność trasy za pomocą usługi map.

- Po poprawnym dodaniu, oferta jest widoczna dla pasażerów.

 

2.2: Zarządzanie rezerwacjami

- Jako kierowca może akceptować lub odrzucać prośby o rezerwację.

- Priorytet: Must Have

- Kryteria akceptacji:

- System wyświetla listę oczekujących rezerwacji.

- Kierowca może kliknąć "Akceptuj" lub "Odrzuć".

- Pasażer otrzymuje natychmiastowe powiadomienie o decyzji kierowcy.

2.3: Edycja opublikowanego przejazdu

- Jako kierowca może edytować szczegóły przejazdu 

- Priorytet: Should Have

- Kryteria akceptacji:

- Jeśli przejazd ma pasażerów, system informuje ich o zmianach.

- Zmiany są weryfikowane pod kątem poprawności.

 

2.4: Odwołanie przejazdu

 

- Jako kierowca może odwołać przejazd w sytuacji awaryjnej, aby poinformować o tym fakcie zapisanych pasażerów. 

- Priorytet: Must Have

- Kryteria akceptacji:

- Kierowca może odwołać przejazd z poziomu panelu 

- System automatycznie wysyła powiadomienia do wszystkich zapisanych pasażerów. 

 

**3.** **Pasażer**

3.1: Wyszukiwanie przejazdów 

- Jako pasażer może wyszukiwać przejazdy według trasy i godziny, aby znaleźć dogodne połączenie.

- Priorytet: Must Have

- Kryteria akceptacji:

- Pasażer może filtrować przejazdy po dacie, godzinie (np. +/- 30 min) i trasie.

- System wyświetla wyniki na mapie oraz w formie listy.

- Jeśli brak wyników, system wyświetla komunikat i sugeruje zmianę filtrów.

3.2: Rezerwacja miejsca

- Jako pasażer może zarezerwować miejsce w wybranym przejeździe, aby mieć pewność, że dojadę na zajęcia.

- Priorytet: Must Have

- Kryteria akceptacji:

- Pasażer klika "Rezerwuj" na wybranym przejeździe.

- System blokuje miejsce (tymczasowo) i wysyła powiadomienie do kierowcy.

- Pasażer widzi status rezerwacji.

3.3: Anulowanie rezerwacji przez pasażera

- Jako pasażer, chcę anulować swoją rezerwację, aby zwolnić miejsce, jeśli zmienią się moje plany.

- Priorytet: Must Have

- Kryteria akceptacji:

- Pasażer może anulować rezerwację .

- System zezwala na anulowanie tylko do określonego czasu przed startem. Po tym czasie wyświetla komunikat błędu.

- System powiadamia kierowcę o zwolnieniu miejsca i przelicza nową trasę.

4. Oceny Administracja

4.1: System ocen i komentarzy

- Jako uczestnik przejazdu, chcę ocenić drugą stronę po zakończeniu podróży, aby budować zaufanie w społeczności akademickiej.

- Priorytet: Should Have

- Kryteria akceptacji:

- System wysyła prośbę o ocenę po zakończeniu przejazdu.

- Ocena wpływa na średnią ocenę użytkownika widoczną w jego profilu.

 5. Administracja

- Jako administrator może zarządzać użytkownikami i zgłoszeniami, aby dbać o bezpieczeństwo i przestrzeganie regulaminu. 

- Priorytet: Must Have

- Kryteria akceptacji:

- Admin może zablokować konto użytkownika łamiącego regulamin.

- Admin może usunąć nieodpowiedni przejazd.

- Admin widzi zgłoszenia od użytkowników.

 

**Wymagania niefunkcjonalne (NFRs)**

 

1. Wydajność

- System musi obsłużyć skokowy wzrost ruchu  bez utraty wydajności.

2. Bezpieczeństwo (Security)

- Wszystkie dane przesyłane między klientem a serwerem muszą być szyfrowane. 

Weryfikacja e-maili musi opierać się na bezpiecznym mechanizmie tokenów.

3. Niezawodność i Dostępność

- System wykonuje automatyczne kopie zapasowe (Backup) bazy danych.

4. Użyteczność (Usability)

- Interfejs musi być w pełni responsywny (RWD).

5. Wsparcie techniczne (Maintainability)

- Kod aplikacji musi być wersjonowany w systemie kontroli wersji. 

- System powinien być zaprojektowany w architekturze umożliwiającej łatwą integrację z API zewnętrznymi.
