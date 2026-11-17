**Wymagania funkcjonalne**

**Zarządzanie kontem i bezpieczeństwo**

| Wymaganie | User story | Priorytet | Kryteria akceptacji |
|---|---|---|---|
| 1.1: Rejestracja | Jako nowy użytkownik może zarejestrować się w systemie podając swój  aby uzyskać dostęp do platformy. | Must Have | System wysyła link aktywacyjny na podany e-mail.<br>Konto jest nieaktywne do momentu kliknięcia w link. |
| 1.2: Logowanie i role użytkowników | Jako zarejestrowany użytkownik może logować się do systemu i mieć dostęp do przejazdów do których jest zapisany | Must Have | Użytkownik może zalogować się za pomocą e-maila i hasła.<br>System weryfikuje poprawność danych logowania.<br>Po zalogowaniu użytkownik widzi panel odpowiedni dla wybranej roli |

**2. Kierowca**

| Wymaganie | User story | Priorytet | Kryteria akceptacji |
|---|---|---|---|
| 2.1: Dodawanie nowej oferty przejazdu | Jako kierowca, chcę dodać nowy przejazd (podać trasę, czas, liczbę miejsc), aby znaleźć pasażerów i podzielić się kosztami. | Must Have | Formularz wymaga podania: punktu startu, punktu docelowego, daty, godziny i liczby wolnych miejsc.<br>System weryfikuje poprawność trasy za pomocą usługi map.<br>Po poprawnym dodaniu, oferta jest widoczna dla pasażerów. |
| 2.2: Zarządzanie rezerwacjami | Jako kierowca może akceptować lub odrzucać prośby o rezerwację. | Must Have | System wyświetla listę oczekujących rezerwacji.<br>Kierowca może kliknąć "Akceptuj" lub "Odrzuć".<br>Pasażer otrzymuje natychmiastowe powiadomienie o decyzji kierowcy. |
| 2.3: Edycja opublikowanego przejazdu | Jako kierowca może edytować szczegóły przejazdu  | Should Have | Jeśli przejazd ma pasażerów, system informuje ich o zmianach.<br>Zmiany są weryfikowane pod kątem poprawności. |
| 2.4: Odwołanie przejazdu | Jako kierowca może odwołać przejazd w sytuacji awaryjnej, aby poinformować o tym fakcie zapisanych pasażerów.  | Must Have | Kierowca może odwołać przejazd z poziomu panelu <br>System automatycznie wysyła powiadomienia do wszystkich zapisanych pasażerów.  |

**3.** **Pasażer**

| Wymaganie | User story | Priorytet | Kryteria akceptacji |
|---|---|---|---|
| 3.1: Wyszukiwanie przejazdów | Jako pasażer może wyszukiwać przejazdy według trasy i godziny, aby znaleźć dogodne połączenie. | Must Have | Pasażer może filtrować przejazdy po dacie, godzinie (np. +/- 30 min) i trasie.<br>System wyświetla wyniki na mapie oraz w formie listy.<br>Jeśli brak wyników, system wyświetla komunikat i sugeruje zmianę filtrów. |
| 3.2: Rezerwacja miejsca | Jako pasażer może zarezerwować miejsce w wybranym przejeździe, aby mieć pewność, że dojadę na zajęcia. | Must Have | Pasażer klika "Rezerwuj" na wybranym przejeździe.<br>System blokuje miejsce (tymczasowo) i wysyła powiadomienie do kierowcy.<br>Pasażer widzi status rezerwacji. |
| 3.3: Anulowanie rezerwacji przez pasażera | Jako pasażer, chcę anulować swoją rezerwację, aby zwolnić miejsce, jeśli zmienią się moje plany. | Must Have | Pasażer może anulować rezerwację .<br>System zezwala na anulowanie tylko do określonego czasu przed startem. Po tym czasie wyświetla komunikat błędu.<br>System powiadamia kierowcę o zwolnieniu miejsca i przelicza nową trasę. |

4. Oceny Administracja

| Wymaganie | User story | Priorytet | Kryteria akceptacji |
|---|---|---|---|
| 4.1: System ocen i komentarzy | Jako uczestnik przejazdu, chcę ocenić drugą stronę po zakończeniu podróży, aby budować zaufanie w społeczności akademickiej. | Should Have | System wysyła prośbę o ocenę po zakończeniu przejazdu.<br>Ocena wpływa na średnią ocenę użytkownika widoczną w jego profilu. |

 5. Administracja

| Wymaganie | User story | Priorytet | Kryteria akceptacji |
|---|---|---|---|
| 5. Administracja | Jako administrator może zarządzać użytkownikami i zgłoszeniami, aby dbać o bezpieczeństwo i przestrzeganie regulaminu. | Must Have | Admin może zablokować konto użytkownika łamiącego regulamin.<br>Admin może usunąć nieodpowiedni przejazd.<br>Admin widzi zgłoszenia od użytkowników. |

 

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
