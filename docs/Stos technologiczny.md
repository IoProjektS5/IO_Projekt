# Stos technologiczny

- Frontend: React
- Backend: FastAPI
- Baza danych: MySQL (MariaDB)

# Uzasadnienie wyboru stosu technologicznego

FastAPI to framework do tworzenia API w języku Python, który ma wydajność na poziomie Node.js i Go. Obsługuje standard OpenAPI, co ułatwi tworzenie ścieżek operacji, ich parametrów oraz umożliwi automatyczne generowanie dokumentacji API przy użyciu JSON Schema. Zawiera komponent SQLModel (oparty na SQLAlchemy i Pydantic), który pozwala na łatwe mapowanie obiektowo-relacyjne (ORM) z bazą danych. Pydantic zapewnia walidację danych wejściowych i wyjściowych, co zwiększa bezpieczeństwo aplikacji. Wspiera schematy bezpieczeństwa takie jak OAuth2, klucze API oraz ciasteczka sesji. Jak większość nowoczesnych frameworków, FastAPI jest asynchroniczny, co pozwala na obsługę wielu żądań jednocześnie. Dzięki swojej dokumentacji, w tym przykładom, prostej strukturze (deklararowanie typów odbywa się jak we współczesnym Pythonie) powinien umożliwić szybkie napisanie backendu aplikacji.