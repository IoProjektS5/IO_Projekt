# Stos technologiczny

- Frontend: React
- Backend: FastAPI
- Baza danych: MySQL (MariaDB)
- API tras: GraphHopper

# Uzasadnienie wyboru stosu technologicznego

FastAPI to framework do tworzenia API w języku Python, który ma wydajność na poziomie Node.js i Go. Obsługuje standard OpenAPI, co ułatwi tworzenie ścieżek operacji, ich parametrów oraz umożliwi automatyczne generowanie dokumentacji API przy użyciu JSON Schema. Zawiera komponent SQLModel (oparty na SQLAlchemy i Pydantic), który pozwala na łatwe mapowanie obiektowo-relacyjne (ORM) z bazą danych. Pydantic zapewnia walidację danych wejściowych i wyjściowych, co zwiększa bezpieczeństwo aplikacji. Wspiera schematy bezpieczeństwa takie jak OAuth2, klucze API oraz ciasteczka sesji. Jak większość nowoczesnych frameworków, FastAPI jest asynchroniczny, co pozwala na obsługę wielu żądań jednocześnie. Dzięki swojej dokumentacji, w tym przykładom, prostej strukturze (deklararowanie typów odbywa się jak we współczesnym Pythonie) powinien umożliwić szybkie napisanie backendu aplikacji.

MariaDB to otwartoźródłowy fork MySQL, który jest w pełni kompatybilny z MySQL. Funkcjonalności MariaDB w pełni wystarczą na zrealizowanie projektu, gdyż sama baza danych będzie zawierała użytkowników, grupy oraz współrzędne geograficzne, które będą wykorzystywane do wyznaczania tras poprzez odpytywanie API GraphHopper, a jego wynik – punkty odbioru, godziny odbioru, długość i czas przejazdu będzie również będą zapisywane. W przypadku gdyby baza danych miała też zawierać trasy w postaci geometrii, lepszym wyborem mógłby być PostgreSQL z rozszerzeniem PostGIS.

GraphHopper to silnik tras, który pozwala na wyznaczanie tras dla różnych środków transportu (w projekcie tylko samochód).
Istnieje jego oficjalny deployment, ale równie dobrze może być uruchomiony lokalnie – w celu uniknięcia opłat za korzystanie z API na podstawie naliczanych kredytów. Będzie wykorzystywany do wyznaczania podglądowych tras, obliczania ich czasu i długości przejazdu, a także do wyszukiwania najlepszych grup, do których może się dołączyć kolejny użytkownik.